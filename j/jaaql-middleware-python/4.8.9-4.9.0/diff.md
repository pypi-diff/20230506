# Comparing `tmp/jaaql-middleware-python-4.8.9.tar.gz` & `tmp/jaaql-middleware-python-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.8.9.tar", last modified: Tue May  2 21:12:32 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.9.0.tar", last modified: Sat May  6 14:31:55 2023, max compression
```

## Comparing `jaaql-middleware-python-4.8.9.tar` & `jaaql-middleware-python-4.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.519459 jaaql-middleware-python-4.8.9/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-02 21:12:32.519459 jaaql-middleware-python-4.8.9/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.459461 jaaql-middleware-python-4.8.9/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.462494 jaaql-middleware-python-4.8.9/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4496 2023-05-02 21:03:49.000000 jaaql-middleware-python-4.8.9/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.467458 jaaql-middleware-python-4.8.9/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.8.9/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.8.9/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.9/jaaql/db/db_utils.py
--rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.8.9/jaaql/db/db_utils_no_circ.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.471458 jaaql-middleware-python-4.8.9/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.475460 jaaql-middleware-python-4.8.9/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.8.9/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-05-02 18:34:17.000000 jaaql-middleware-python-4.8.9/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.479458 jaaql-middleware-python-4.8.9/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.8.9/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.8.9/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.480459 jaaql-middleware-python-4.8.9/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.8.9/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.8.9/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.483461 jaaql-middleware-python-4.8.9/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.8.9/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0     8574 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.8.9/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.494459 jaaql-middleware-python-4.8.9/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    32609 2023-05-02 17:45:39.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.496458 jaaql-middleware-python-4.8.9/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.8.9/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.8.9/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.503458 jaaql-middleware-python-4.8.9/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.8.9/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.507461 jaaql-middleware-python-4.8.9/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.8.9/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0     2047 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.8.9/jaaql/services/migrations_manager_service.py
--rw-rw-rw-   0        0        0      296 2023-05-02 12:09:59.000000 jaaql-middleware-python-4.8.9/jaaql/services/patch_mms.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.513459 jaaql-middleware-python-4.8.9/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.8.9/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:32.518459 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-02 21:12:32.000000 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-02 21:12:32.000000 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:12:32.000000 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-05-02 21:12:32.000000 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 21:12:32.000000 jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 21:12:32.519459 jaaql-middleware-python-4.8.9/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.280793 jaaql-middleware-python-4.9.0/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.284795 jaaql-middleware-python-4.9.0/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4496 2023-05-06 14:31:29.000000 jaaql-middleware-python-4.9.0/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.289792 jaaql-middleware-python-4.9.0/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.9.0/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_utils.py
+-rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_utils_no_circ.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.293792 jaaql-middleware-python-4.9.0/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.297812 jaaql-middleware-python-4.9.0/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.9.0/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     7331 2023-05-03 00:21:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.302792 jaaql-middleware-python-4.9.0/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.303792 jaaql-middleware-python-4.9.0/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.9.0/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.9.0/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.306792 jaaql-middleware-python-4.9.0/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8620 2023-05-03 01:48:38.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.318793 jaaql-middleware-python-4.9.0/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32856 2023-05-04 13:15:14.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.319807 jaaql-middleware-python-4.9.0/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.9.0/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.9.0/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.326793 jaaql-middleware-python-4.9.0/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1960 2023-05-06 14:31:29.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.330792 jaaql-middleware-python-4.9.0/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.9.0/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2096 2023-05-03 01:33:07.000000 jaaql-middleware-python-4.9.0/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-03 01:25:04.000000 jaaql-middleware-python-4.9.0/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.337792 jaaql-middleware-python-4.9.0/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.342792 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/setup.py
```

### Comparing `jaaql-middleware-python-4.8.9/LICENSE.txt` & `jaaql-middleware-python-4.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/PKG-INFO` & `jaaql-middleware-python-4.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.9
+Version: 4.9.0
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/constants.py` & `jaaql-middleware-python-4.9.0/jaaql/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,9 +125,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.8.9"
+VERSION = "4.9.0"
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.9.0/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.9.0/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.9.0/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/db/db_utils_no_circ.py` & `jaaql-middleware-python-4.9.0/jaaql/db/db_utils_no_circ.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.9.0/jaaql/email/email_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,36 +71,34 @@
                 if not re.match(REGEX__object_name, col):
                     raise HttpStatusException(ERR__invalid_object_name % col)
 
             cols = ", ".join(['"' + key + '"' for key in parameters.keys()])
             vals = ", ".join([':' + key for key in parameters.keys()])
 
             ins_query = ins_query % (template[KG__email_template__data_validation_table], cols, vals)
-            submit(vault, config, db_crypt_key, jaaql_connection, {
+            parameter_id = submit(vault, config, db_crypt_key, jaaql_connection, {
                 KEY__application: application,
                 KEY__schema: template[KG__email_template__validation_schema],
                 KEY_query: ins_query,
                 KEY_parameters: parameters,
                 KEY_assert: ASSERT_one
-            }, account_id)
-            parameter_id = execute_supplied_statement_singleton(jaaql_connection, ins_query, parameters, as_objects=True)[KEY__id]
+            }, account_id, as_objects=True, singleton=True)[KEY__id]
 
             sel_table = \
                 template[KG__email_template__data_validation_table] if template[KG__email_template__data_validation_view] is None \
-                else template[KG__email_template__data_validation_view]
+                    else template[KG__email_template__data_validation_view]
 
             sel_query = "SELECT * FROM %s WHERE id = :id" % sel_table
-            submit(vault, config, db_crypt_key, jaaql_connection, {
+            parameters = submit(vault, config, db_crypt_key, jaaql_connection, {
                 KEY__application: application,
                 KEY__schema: template[KG__email_template__validation_schema],
                 KEY_query: sel_query,
-                KEY_parameters: parameters,
+                KEY_parameters: {KEY__id: parameter_id},
                 KEY_assert: ASSERT_one
-            }, account_id)
-            parameters = execute_supplied_statement_singleton(jaaql_connection, sel_query, {KEY__id: parameter_id}, as_objects=True)
+            }, account_id, as_objects=True, singleton=True)
         else:
             parameters = {}
 
         none_sanitized_parameters[EMAIL_PARAM__app_url] = application_base_url
         none_sanitized_parameters[EMAIL_PARAM__email_address] = account[KG__account__username]
         parameters = {**parameters, **none_sanitized_parameters}
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.9.0/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.9.0/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.9.0/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/jaaql.py` & `jaaql-middleware-python-4.9.0/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.9.0/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.9.0/jaaql/migrations/migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import listdir, environ
 from jaaql.interpreter.interpret_jaaql import InterpretJAAQL
 from jaaql.exceptions.http_status_exception import HttpStatusException
 from jaaql.utilities.crypt_utils import encrypt_raw, AES__iv_length
 from jaaql.utilities.utils_no_project_imports import objectify
 import re
 from monitor.main import initialise, MARKER__bypass, MARKER__jaaql_bypass
-from jaaql.constants import USERNAME__jaaql, USERNAME__super_db, DB__jaaql, DB__postgres
+from jaaql.constants import USERNAME__jaaql, USERNAME__super_db, DB__jaaql, DB__postgres, USERNAME__superuser
 
 
 MIGRATION_HISTORY = "migration_history"
 
 
 QUERY_LOAD_TABLE = "SELECT * FROM %s WHERE project_name = :project_name" % MIGRATION_HISTORY
 ATTR_PROJECT_NAME = "project_name"
@@ -151,22 +151,22 @@
             checksum = hashlib.md5(hash_content.encode("UTF-8")).digest()
             checksum = int.from_bytes(checksum[0:3], byteorder="little")
             if full_name not in installed_scripts:
                 config_loc = os.environ.get("JAAQL_CONFIG_LOC", "monitor_config")
                 configs = []
                 for fname in os.listdir(config_loc):
                     config_name = ".".join(fname.split(".")[0:-1])
-                    configs.append([config_name, fname])
+                    configs.append([config_name, join(config_loc, fname)])
 
-                encoded_configs = [[USERNAME__jaaql, host, USERNAME__jaaql, MARKER__bypass + bypass_super, DB__jaaql],
-                                   [USERNAME__super_db, host, USERNAME__super_db, MARKER__jaaql_bypass + bypass_jaaql, DB__postgres]]
+                encoded_configs = [[USERNAME__jaaql, host, USERNAME__jaaql, MARKER__jaaql_bypass + bypass_jaaql, DB__jaaql],
+                                   [USERNAME__superuser, host, USERNAME__super_db, MARKER__bypass + bypass_super, DB__postgres]]
 
                 start_time = datetime.now()
 
-                initialise(actual_file_name, content, configs, encoded_configs)
+                initialise(actual_file_name, content, configs, encoded_configs, host)
 
                 execution_time = time_delta_ms(start_time, datetime.now())
                 version = script_file.split("__")[0][1:]
                 description = " ".join(script_file.split(VERSION_SPLIT)[1].split(EXTENSION_JAAQL)[0].split(WORD_SPLIT))
                 ij.transform({
                     "query": QUERY_INS_TABLE,
                     "parameters": {
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/base_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,24 @@
     "false": False
 }
 
 IPS__local = [
     "127.0.0.1", "localhost"
 ]
 
+
 class BaseJAAQLController:
 
     sentinel_errors = None
     internal_sentinel = False
+    base_url = None
 
     def __init__(self, model: JAAQLModel, is_prod: bool, base_url: str, do_profiling: bool = False):
         super().__init__()
+        BaseJAAQLController.base_url = base_url
         self.app = Flask(__name__, instance_relative_config=True)
         self.app.config[FLASK__json_sort_keys] = False
         self.app.config[FLASK__max_content_length] = 1024 * 1024 * 2  # 2 MB
         self._init_error_handlers(self.app)
         self.model = model
         self.do_profiling = do_profiling
         self.documentation_memory = {}
@@ -430,22 +433,25 @@
                     is_public = None
                     verification_hook = None
                     if method.parallel_verification:
                         verification_hook = Queue()
 
                     ip_addr = request.headers.get(HEADER__real_ip, request.remote_addr).split(",")[0]
 
+                    if ip_addr is None or ip_addr == "":
+                        ip_addr = "127.0.0.1"
+
                     if swagger_documentation.security:
                         bypass_super = request.headers.get(HEADER__security_bypass)
                         bypass_jaaql = request.headers.get(HEADER__security_bypass_jaaql)
                         if bypass_super or bypass_jaaql:
                             if ip_addr not in IPS__local:
-                                raise HttpStatusException("Bypass used in none local context", HTTPStatus.UNAUTHORIZED)
+                                raise HttpStatusException("Bypass used in none local context: " + ip_addr, HTTPStatus.UNAUTHORIZED)
                             miss_super_bypass = bypass_super and bypass_super != self.model.local_super_access_key
-                            miss_jaaql_bypass = bypass_jaaql and bypass_jaaql != self.model.local_super_access_key
+                            miss_jaaql_bypass = bypass_jaaql and bypass_jaaql != self.model.local_jaaql_access_key
                             if miss_super_bypass or miss_jaaql_bypass:
                                 raise HttpStatusException("Invalid bypass key", HTTPStatus.UNAUTHORIZED)
 
                             is_public = False
                             username = USERNAME__super_db if bypass_super else USERNAME__jaaql
                             account_id, ip_id = self.model.get_bypass_user(username, ip_addr)
 
@@ -615,14 +621,15 @@
                 tb_frame = sys.exc_info()[2]
                 while tb_frame.tb_next:
                     tb_frame = tb_frame.tb_next
                 source_file = tb_frame.tb_frame.f_code.co_filename[len(os.getcwd()) + 1:]
                 source_file = source_file.replace("\\", "/")
 
                 BaseJAAQLController.sentinel_errors.put({
+                    "location": BaseJAAQLController.base_url,
                     "error_condensed": str(orig),
                     "version": VERSION,
                     "source_system": "Sentinel" if BaseJAAQLController.internal_sentinel else "JAAQL",
                     "source_file": source_file,
                     "file_line_number": tb_frame.tb_lineno,
                     "stacktrace": ''.join(traceback.format_exception(etype=type(orig), value=orig, tb=orig.__traceback__))
                 })
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/mvc/model.py` & `jaaql-middleware-python-4.9.0/jaaql/mvc/model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.9.0/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.9.0/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.9.0/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.9.0/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 $$ language plpgsql;
 
 create or replace function configure_database_for_use_with_jaaql(database object_name) returns void as
 $$
 BEGIN
     if does_user_own_this_database(session_user, database) then
         PERFORM dblink_exec('dbname=' || database, 'CREATE EXTENSION IF NOT EXISTS pgcrypto;');
+        PERFORM dblink_exec('dbname=' || database, 'CREATE EXTENSION IF NOT EXISTS plpgsql_check;');
         PERFORM dblink_exec('dbname=' || database, 'CREATE EXTENSION IF NOT EXISTS jaaql;');
     else
         raise notice 'You do not own this database'
                  'You cannot install the jaaql extension';
 
         raise notice '% %', SQLERRM, SQLSTATE;
         return;
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.9.0/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.9.0/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.9.0/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.9.0/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/services/migrations_manager_service.py` & `jaaql-middleware-python-4.9.0/jaaql/services/migrations_manager_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,12 +42,13 @@
             json_data["db_connection_string"] = "postgresql://postgres:123456@localhost:5434/"
         requests.post(base_url + ENDPOINT__install, json=json_data)
 
     await_jaaql_installation(config, is_gunicorn)
     vault = Vault(vault_key, DIR__vault)
 
     bypass_header = {HEADER__security_bypass: vault.get_obj(VAULT_KEY__super_local_access_key)}
-    requests.post(base_url + ENDPOINT__execute_migrations, headers=bypass_header)
+    res = requests.post(base_url + ENDPOINT__execute_migrations, headers=bypass_header)
 
-    flask_app = create_app()
-    print("Created migration manager app host, running flask", file=sys.stderr)
-    flask_app.run(port=PORT__mms, host="0.0.0.0", threaded=True)
+    if res.status_code == 200:
+        flask_app = create_app()
+        print("Created migration manager app host, running flask", file=sys.stderr)
+        flask_app.run(port=PORT__mms, host="0.0.0.0", threaded=True)
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.9.0/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/utilities/options.py` & `jaaql-middleware-python-4.9.0/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.9.0/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.9.0/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.9.0/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.8.9
+Version: 4.9.0
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.8.9/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.8.9/setup.py` & `jaaql-middleware-python-4.9.0/setup.py`

 * *Files identical despite different names*

