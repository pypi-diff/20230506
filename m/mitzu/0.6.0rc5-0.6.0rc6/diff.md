# Comparing `tmp/mitzu-0.6.0rc5.tar.gz` & `tmp/mitzu-0.6.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc5.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc6.tar", max compression
```

## Comparing `mitzu-0.6.0rc5.tar` & `mitzu-0.6.0rc6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-05-04 19:30:11.338744 mitzu-0.6.0rc5/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-04 19:30:11.338744 mitzu-0.6.0rc5/README.md
--rw-r--r--   0        0        0     6148 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-05-04 19:31:10.975585 mitzu-0.6.0rc5/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39764 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/helper.py
--rw-r--r--   0        0        0    53852 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11926 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7022 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13737 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1403 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3056 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5802 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15464 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4527 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21140 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9846 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    14654 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21781 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0     9604 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1347 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4107 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5027 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10191 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11849 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9629 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    36159 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5155 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3185 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     5198 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    20635 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25830 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     3949 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2943 2023-05-04 19:31:10.975585 mitzu-0.6.0rc5/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-06 19:51:27.994575 mitzu-0.6.0rc6/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-06 19:51:27.994575 mitzu-0.6.0rc6/README.md
+-rw-r--r--   0        0        0     6148 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-05-06 19:52:36.707001 mitzu-0.6.0rc6/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39764 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/helper.py
+-rw-r--r--   0        0        0    53852 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11926 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7022 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-06 19:51:28.462606 mitzu-0.6.0rc6/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13737 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1403 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3088 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5802 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15464 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4527 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21140 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9846 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14654 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-05-06 19:51:28.466606 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21781 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0     9604 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1347 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4107 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5027 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10191 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11849 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9629 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    36159 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5155 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3185 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4719 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    21352 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25830 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4625 2023-05-06 19:51:28.470607 mitzu-0.6.0rc6/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2943 2023-05-06 19:52:36.707001 mitzu-0.6.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc6/PKG-INFO
```

### Comparing `mitzu-0.6.0rc5/LICENSE.txt` & `mitzu-0.6.0rc6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/README.md` & `mitzu-0.6.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/.DS_Store` & `mitzu-0.6.0rc6/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/__init__.py` & `mitzu-0.6.0rc6/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.5"
+__version__ = "0.6.0-rc.6"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc6/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/helper.py` & `mitzu-0.6.0rc6/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc6/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/helper.py` & `mitzu-0.6.0rc6/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/model.py` & `mitzu-0.6.0rc6/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc6/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/project_discovery.py` & `mitzu-0.6.0rc6/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/project_serialization.py` & `mitzu-0.6.0rc6/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/samples/__init__.py` & `mitzu-0.6.0rc6/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc6/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc6/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/serialization.py` & `mitzu-0.6.0rc6/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/charts.py` & `mitzu-0.6.0rc6/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/common.py` & `mitzu-0.6.0rc6/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/labels.py` & `mitzu-0.6.0rc6/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/plot.py` & `mitzu-0.6.0rc6/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/titles.py` & `mitzu-0.6.0rc6/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc6/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc6/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc6/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc6/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc6/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc6/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc6/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc6/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc6/mitzu/webapp/auth/authorizer.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc6/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc6/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc6/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/cache.py` & `mitzu-0.6.0rc6/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc6/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/configs.py` & `mitzu-0.6.0rc6/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc6/mitzu/webapp/dependencies.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,31 @@
     navbar_service: NB.NavbarService
     secret_service: SS.SecretService
     user_service: U.UserService
     notification_service: NS.NotificationService
 
     @classmethod
     def from_configs(
-        cls, notification_service: Optional[NS.NotificationService] = None
+        cls,
+        notification_service: Optional[NS.NotificationService] = None,
     ) -> Dependencies:
         if notification_service is None:
             notification_service = NS.DummyNotificationService()
 
         delegate_cache: C.MitzuCache
         if configs.CACHE_REDIS_URL is not None:
             delegate_cache = C.RedisMitzuCache(global_prefix=configs.CACHE_PREFIX)
         else:
             delegate_cache = C.DiskMitzuCache(
                 "cache", global_prefix=configs.CACHE_PREFIX
             )
         cache = C.RequestCache(delegate_cache)
-        storage = S.MitzuStorage(connection_string=configs.STORAGE_CONNECTION_STRING)
+        storage = S.MitzuStorage(
+            connection_string=configs.STORAGE_CONNECTION_STRING,
+        )
 
         oauth_config = None
         if configs.AUTH_BACKEND == "cognito":
             from mitzu.webapp.auth.cognito import Cognito
 
             oauth_config = Cognito.get_config()
         elif configs.AUTH_BACKEND == "google":
```

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/helper.py` & `mitzu-0.6.0rc6/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/model.py` & `mitzu-0.6.0rc6/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc6/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc6/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc6/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc6/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.0rc6/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc6/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc6/mitzu/webapp/service/user_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional, Tuple
 import random
 import string
 import hashlib
 import mitzu.webapp.storage as S
-import mitzu.webapp.configs as configs
 import mitzu.webapp.model as WM
 import mitzu.webapp.service.notification_service as NS
-import mitzu.helper as H
 
 
 class UserNotFoundException(Exception):
     """
     Raised when the user is not found in the local user store
     """
 
@@ -60,25 +58,14 @@
         self._storage = storage
 
         if notification_service:
             self._notification_service = notification_service
         else:
             self._notification_service = NS.DummyNotificationService()
 
-        try:
-            if configs.AUTH_ROOT_USER_EMAIL:
-                self.new_user(
-                    configs.AUTH_ROOT_USER_EMAIL,
-                    configs.AUTH_ROOT_PASSWORD,
-                    configs.AUTH_ROOT_PASSWORD,
-                    role=WM.Role.ADMIN,
-                )
-        except UserAlreadyExists:
-            H.LOGGER.info(f"Root user {configs.AUTH_ROOT_USER_EMAIL} already exists.")
-
     def list_users(self) -> List[WM.User]:
         return self._storage.list_users()
 
     def get_user_by_id(self, user_id: str) -> Optional[WM.User]:
         return self._storage.get_user_by_id(user_id)
 
     def get_user_by_email(self, email: str) -> Optional[WM.User]:
```

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/storage.py` & `mitzu-0.6.0rc6/mitzu/webapp/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+import multiprocessing
 from typing import Dict, List, Optional
 
-
+from mitzu.helper import LOGGER
 import mitzu.model as M
 import mitzu.webapp.model as WM
 import mitzu.webapp.storage_model as SM
 from mitzu.samples.data_ingestion import create_and_ingest_sample_project
 import sqlalchemy as SA
 from sqlalchemy.orm import Session
 
@@ -74,38 +75,53 @@
 
 
 class MitzuStorage:
     def __init__(
         self,
         connection_string: str = "sqlite://?check_same_thread=False",
     ) -> None:
-        self._engine = SA.create_engine(connection_string, pool_pre_ping=True)
-        self._is_sqlite = connection_string.startswith("sqlite")
-        self.__init_schema()
+        self.__pid = None
+        self.__is_sqlite = connection_string.startswith("sqlite")
+        self.__connection_string = connection_string
+
+    def __create_new_db_session(self) -> Session:
+        session = SA.orm.sessionmaker(bind=self._engine)()
+        if self.__is_sqlite:
+            session.execute("PRAGMA foreign_keys = ON;")
+            session.commit()
+        return session
+
+    def __create_engine_when_needed(self):
+        # we need to make sure that the engine is created by the current process and not by the parent process
+        pid = multiprocessing.current_process().pid
+        if self.__pid != pid:
+            LOGGER.debug(
+                f"Engine needs to be recreated, previous instance created by pid: {self.__pid}, current pid: {pid}"
+            )
+            self._engine = SA.create_engine(
+                self.__connection_string, pool_pre_ping=True
+            )
+            self.__pid = pid
+            if flask.has_app_context() and "request_session_cache" in flask.g:
+                flask.g.request_session_cache = self.__create_new_db_session()
 
     @property
     def _session(self) -> Session:
+        self.__create_engine_when_needed()
         if flask.has_app_context():
             if "request_session_cache" not in flask.g:
-                session = SA.orm.sessionmaker(bind=self._engine)()
-                if self._is_sqlite:
-                    session.execute("PRAGMA foreign_keys = ON;")
-                    session.commit()
-                flask.g.request_session_cache = session
-                return session
-            else:
-                return flask.g.request_session_cache
+                flask.g.request_session_cache = self.__create_new_db_session()
+
+            return flask.g.request_session_cache
         else:
-            session = SA.orm.sessionmaker(bind=self._engine)()
-            if self._is_sqlite:
-                session.execute("PRAGMA foreign_keys = ON;")
-                session.commit()
-            return session
+            return self.__create_new_db_session()
 
-    def __init_schema(self):
+    def init_db_schema(self):
+        LOGGER.info("Initializing the database schema")
+        self.__create_engine_when_needed()
         tables = []
         for storage_record in [
             SM.UserStorageRecord,
             SM.DiscoverySettingsStorageRecord,
             SM.WebappSettingsStorageRecord,
             SM.ConnectionStorageRecord,
             SM.ProjectStorageRecord,
```

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc6/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc5/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc6/mitzu/webapp/webapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
 import flask
 from dash import Dash, DiskcacheManager, dcc, html, page_container
 from dash.long_callback.managers import BaseLongCallbackManager
 import mitzu.webapp.cache as C
+import mitzu.webapp.model as WM
+import mitzu.helper as H
 
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 import mitzu.webapp.offcanvas as OC
 import mitzu.webapp.pages.explore.explore_page as EXP
 import mitzu.webapp.pages.paths as P
+import mitzu.webapp.service.user_service as US
 from mitzu.helper import LOGGER
 import json
 import traceback
 from mitzu.webapp.helper import MITZU_LOCATION
 
 MAIN = "main"
 
@@ -57,14 +60,27 @@
     def after_request(response: flask.Response):
         request = flask.request
         if dependencies is not None:
             return dependencies.authorizer.refresh_auth_token(request, response)
         return response
 
     with server.app_context():
+        dependencies.storage.init_db_schema()
+        try:
+            if configs.AUTH_ROOT_USER_EMAIL:
+                dependencies.user_service.new_user(
+                    configs.AUTH_ROOT_USER_EMAIL,
+                    configs.AUTH_ROOT_PASSWORD,
+                    configs.AUTH_ROOT_PASSWORD,
+                    role=WM.Role.ADMIN,
+                )
+                H.LOGGER.info(f"Root user {configs.AUTH_ROOT_USER_EMAIL} is created.")
+        except US.UserAlreadyExists:
+            H.LOGGER.info(f"Root user {configs.AUTH_ROOT_USER_EMAIL} already exists.")
+
         flask.current_app.config[DEPS.CONFIG_KEY] = dependencies
         if configs.SETUP_SAMPLE_PROJECT:
             S.setup_sample_project(dependencies.storage)
 
     dependencies.navbar_service.register_navbar_item_provider(
         "left",
         EXP.metric_type_navbar_provider,
```

### Comparing `mitzu-0.6.0rc5/pyproject.toml` & `mitzu-0.6.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.5"
+version = "0.6.0-rc.6"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc5/PKG-INFO` & `mitzu-0.6.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc5
+Version: 0.6.0rc6
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

