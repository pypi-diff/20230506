# Comparing `tmp/nautobot_golden_config-1.4.0.tar.gz` & `tmp/nautobot_golden_config-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_golden_config-1.4.0.tar", max compression
+gzip compressed data, was "nautobot_golden_config-1.4.1.tar", max compression
```

## Comparing `nautobot_golden_config-1.4.0.tar` & `nautobot_golden_config-1.4.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      591 2023-05-05 15:54:12.999758 nautobot_golden_config-1.4.0/LICENSE
--rw-r--r--   0        0        0     6560 2023-05-05 15:54:12.999758 nautobot_golden_config-1.4.0/README.md
--rw-r--r--   0        0        0     1957 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/__init__.py
--rw-r--r--   0        0        0       57 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/__init__.py
--rw-r--r--   0        0        0     5450 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/serializers.py
--rw-r--r--   0        0        0      935 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/urls.py
--rw-r--r--   0        0        0     4706 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/views.py
--rw-r--r--   0        0        0      358 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/choices.py
--rw-r--r--   0        0        0     9137 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/datasources.py
--rw-r--r--   0        0        0      402 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/exceptions.py
--rw-r--r--   0        0        0     9369 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/filters.py
--rw-r--r--   0        0        0    12220 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/forms.py
--rw-r--r--   0        0        0    10715 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/jobs.py
--rw-r--r--   0        0        0      906 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_backup.py
--rw-r--r--   0        0        0      930 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_compliance.py
--rw-r--r--   0        0        0      944 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_generate_config.py
--rw-r--r--   0        0        0    12457 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0001_initial.py
--rw-r--r--   0        0        0      508 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0002_custom_data.py
--rw-r--r--   0        0        0     1814 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
--rw-r--r--   0        0        0     1824 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
--rw-r--r--   0        0        0     1514 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0005_json_compliance_rule.py
--rw-r--r--   0        0        0     1794 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
--rw-r--r--   0        0        0     2555 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
--rw-r--r--   0        0        0      665 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
--rw-r--r--   0        0        0     2558 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
--rw-r--r--   0        0        0      929 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
--rw-r--r--   0        0        0     1486 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
--rw-r--r--   0        0        0      909 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
--rw-r--r--   0        0        0      463 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
--rw-r--r--   0        0        0      429 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
--rw-r--r--   0        0        0      705 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
--rw-r--r--   0        0        0      769 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
--rw-r--r--   0        0        0     1645 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
--rw-r--r--   0        0        0      327 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
--rw-r--r--   0        0        0      678 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
--rw-r--r--   0        0        0     1186 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
--rw-r--r--   0        0        0      663 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
--rw-r--r--   0        0        0      389 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
--rw-r--r--   0        0        0        0 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/__init__.py
--rw-r--r--   0        0        0    25184 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/models.py
--rw-r--r--   0        0        0     4331 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/navigation.py
--rw-r--r--   0        0        0     5843 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_backup.py
--rw-r--r--   0        0        0     7182 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_compliance.py
--rw-r--r--   0        0        0     5641 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_intended.py
--rw-r--r--   0        0        0     1525 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/processor.py
--rwxr-xr-x   0        0        0      719 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/signals.py
--rw-r--r--   0        0        0     4941 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css
--rw-r--r--   0        0        0    67546 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js
--rw-r--r--   0        0        0    16129 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tables.py
--rw-r--r--   0        0        0     4714 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/template_content.py
--rw-r--r--   0        0        0     7593 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html
--rw-r--r--   0        0        0     3680 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html
--rw-r--r--   0        0        0     1568 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html
--rw-r--r--   0        0        0     1123 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
--rw-r--r--   0        0        0     1100 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
--rw-r--r--   0        0        0     3902 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html
--rw-r--r--   0        0        0     1961 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html
--rw-r--r--   0        0        0     1127 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html
--rw-r--r--   0        0        0      950 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
--rw-r--r--   0        0        0      951 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
--rw-r--r--   0        0        0     4142 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
--rw-r--r--   0        0        0      365 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/dff2html_base.html
--rw-r--r--   0        0        0     3616 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
--rw-r--r--   0        0        0     3487 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
--rw-r--r--   0        0        0     1393 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
--rw-r--r--   0        0        0      181 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/manytomany.html
--rw-r--r--   0        0        0       35 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templatetags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templatetags/json_helpers.py
--rw-r--r--   0        0        0       52 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/__init__.py
--rw-r--r--   0        0        0    14003 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/conftest.py
--rw-r--r--   0        0        0       51 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/forms/__init__.py
--rw-r--r--   0        0        0     3228 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/forms/test_golden_config_settings.py
--rw-r--r--   0        0        0       83 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/jinja_filters.py
--rw-r--r--   0        0        0    12405 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_api.py
--rw-r--r--   0        0        0      995 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_basic.py
--rw-r--r--   0        0        0     3503 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_datasources.py
--rw-r--r--   0        0        0    12768 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_filters.py
--rw-r--r--   0        0        0    12960 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_graphql.py
--rw-r--r--   0        0        0     5464 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_helpers.py
--rw-r--r--   0        0        0    12194 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_models.py
--rw-r--r--   0        0        0       58 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/__init__.py
--rw-r--r--   0        0        0     1018 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
--rw-r--r--   0        0        0       55 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/__init__.py
--rw-r--r--   0        0        0     2899 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_git.py
--rw-r--r--   0        0        0     1247 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_graphql.py
--rw-r--r--   0        0        0    15214 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_helpers.py
--rw-r--r--   0        0        0     1284 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_utils.py
--rw-r--r--   0        0        0    12883 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_views.py
--rw-r--r--   0        0        0     1963 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/urls.py
--rw-r--r--   0        0        0       17 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/__init__.py
--rw-r--r--   0        0        0     8758 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/config_postprocessing.py
--rw-r--r--   0        0        0      627 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/constant.py
--rw-r--r--   0        0        0      607 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/db_management.py
--rw-r--r--   0        0        0     2990 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/git.py
--rw-r--r--   0        0        0     1771 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/graphql.py
--rw-r--r--   0        0        0     5407 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/helper.py
--rw-r--r--   0        0        0     3401 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/management.py
--rw-r--r--   0        0        0     1079 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/utils.py
--rw-r--r--   0        0        0    33739 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/views.py
--rw-r--r--   0        0        0     3753 2023-05-05 15:54:23.583909 nautobot_golden_config-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 nautobot_golden_config-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-05 22:42:27.075207 nautobot_golden_config-1.4.1/LICENSE
+-rw-r--r--   0        0        0     6560 2023-05-05 22:42:27.075207 nautobot_golden_config-1.4.1/README.md
+-rw-r--r--   0        0        0     1957 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/api/__init__.py
+-rw-r--r--   0        0        0     5450 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/api/serializers.py
+-rw-r--r--   0        0        0      935 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/api/urls.py
+-rw-r--r--   0        0        0     4706 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/api/views.py
+-rw-r--r--   0        0        0      358 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/choices.py
+-rw-r--r--   0        0        0     9137 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/datasources.py
+-rw-r--r--   0        0        0      402 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/exceptions.py
+-rw-r--r--   0        0        0     9369 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/filters.py
+-rw-r--r--   0        0        0    12220 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/forms.py
+-rw-r--r--   0        0        0    10715 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/jobs.py
+-rw-r--r--   0        0        0      906 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_config_backup.py
+-rw-r--r--   0        0        0      930 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_config_compliance.py
+-rw-r--r--   0        0        0      944 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_generate_config.py
+-rw-r--r--   0        0        0    12457 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0001_initial.py
+-rw-r--r--   0        0        0      508 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0002_custom_data.py
+-rw-r--r--   0        0        0     1814 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
+-rw-r--r--   0        0        0     1824 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
+-rw-r--r--   0        0        0     1514 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0005_json_compliance_rule.py
+-rw-r--r--   0        0        0     1794 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
+-rw-r--r--   0        0        0     2555 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
+-rw-r--r--   0        0        0      665 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
+-rw-r--r--   0        0        0     2558 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
+-rw-r--r--   0        0        0      929 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
+-rw-r--r--   0        0        0     1486 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
+-rw-r--r--   0        0        0      909 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
+-rw-r--r--   0        0        0      463 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
+-rw-r--r--   0        0        0      429 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
+-rw-r--r--   0        0        0      705 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
+-rw-r--r--   0        0        0      769 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
+-rw-r--r--   0        0        0     1645 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
+-rw-r--r--   0        0        0      327 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
+-rw-r--r--   0        0        0      678 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
+-rw-r--r--   0        0        0     1186 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
+-rw-r--r--   0        0        0      663 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
+-rw-r--r--   0        0        0      389 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
+-rw-r--r--   0        0        0        0 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/__init__.py
+-rw-r--r--   0        0        0    25184 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/models.py
+-rw-r--r--   0        0        0     4331 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/navigation.py
+-rw-r--r--   0        0        0     5843 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_backup.py
+-rw-r--r--   0        0        0     7182 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_compliance.py
+-rw-r--r--   0        0        0     5641 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_intended.py
+-rw-r--r--   0        0        0     1525 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/processor.py
+-rwxr-xr-x   0        0        0      719 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/signals.py
+-rw-r--r--   0        0        0     4941 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css
+-rw-r--r--   0        0        0    67546 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js
+-rw-r--r--   0        0        0    16129 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tables.py
+-rw-r--r--   0        0        0     4714 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/template_content.py
+-rw-r--r--   0        0        0     7593 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html
+-rw-r--r--   0        0        0     3680 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html
+-rw-r--r--   0        0        0     1568 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html
+-rw-r--r--   0        0        0     1123 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
+-rw-r--r--   0        0        0     1100 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
+-rw-r--r--   0        0        0     3902 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html
+-rw-r--r--   0        0        0     1961 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html
+-rw-r--r--   0        0        0     1127 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html
+-rw-r--r--   0        0        0      950 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
+-rw-r--r--   0        0        0      951 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
+-rw-r--r--   0        0        0     4142 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
+-rw-r--r--   0        0        0      365 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/dff2html_base.html
+-rw-r--r--   0        0        0     3616 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
+-rw-r--r--   0        0        0     3922 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
+-rw-r--r--   0        0        0     1393 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
+-rw-r--r--   0        0        0      181 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/manytomany.html
+-rw-r--r--   0        0        0       35 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templatetags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/templatetags/json_helpers.py
+-rw-r--r--   0        0        0       52 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/__init__.py
+-rw-r--r--   0        0        0    14003 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/conftest.py
+-rw-r--r--   0        0        0       51 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/forms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/forms/test_golden_config_settings.py
+-rw-r--r--   0        0        0       83 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/jinja_filters.py
+-rw-r--r--   0        0        0    12405 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_api.py
+-rw-r--r--   0        0        0      995 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_basic.py
+-rw-r--r--   0        0        0     3503 2023-05-05 22:42:27.103207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_datasources.py
+-rw-r--r--   0        0        0    12768 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_filters.py
+-rw-r--r--   0        0        0    12960 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_graphql.py
+-rw-r--r--   0        0        0     5464 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_helpers.py
+-rw-r--r--   0        0        0    12194 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_models.py
+-rw-r--r--   0        0        0       58 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_nornir_plays/__init__.py
+-rw-r--r--   0        0        0     1018 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
+-rw-r--r--   0        0        0       55 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/__init__.py
+-rw-r--r--   0        0        0     2899 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_git.py
+-rw-r--r--   0        0        0     1247 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_graphql.py
+-rw-r--r--   0        0        0    15214 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_helpers.py
+-rw-r--r--   0        0        0     1284 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_utils.py
+-rw-r--r--   0        0        0    12883 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_views.py
+-rw-r--r--   0        0        0     1963 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/urls.py
+-rw-r--r--   0        0        0       17 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/__init__.py
+-rw-r--r--   0        0        0     8758 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/config_postprocessing.py
+-rw-r--r--   0        0        0      627 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/constant.py
+-rw-r--r--   0        0        0      607 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/db_management.py
+-rw-r--r--   0        0        0     2990 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/git.py
+-rw-r--r--   0        0        0     1771 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/graphql.py
+-rw-r--r--   0        0        0     5407 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/helper.py
+-rw-r--r--   0        0        0     3401 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/management.py
+-rw-r--r--   0        0        0     1079 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/utils.py
+-rw-r--r--   0        0        0    33739 2023-05-05 22:42:27.107207 nautobot_golden_config-1.4.1/nautobot_golden_config/views.py
+-rw-r--r--   0        0        0     3753 2023-05-05 22:42:38.731317 nautobot_golden_config-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 nautobot_golden_config-1.4.1/PKG-INFO
```

### Comparing `nautobot_golden_config-1.4.0/LICENSE` & `nautobot_golden_config-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/README.md` & `nautobot_golden_config-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/__init__.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/api/serializers.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/api/urls.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/api/views.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/datasources.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/filters.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/forms.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/jobs.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_backup.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_config_backup.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_compliance.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_generate_config.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/management/commands/run_generate_config.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0001_initial.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0003_auto_20210510_2356.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0003_auto_20210510_2356.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0004_auto_20210616_2234.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0004_auto_20210616_2234.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0005_json_compliance_rule.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0005_json_compliance_rule.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0008_multi_repo_support_final.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0008_multi_repo_support_final.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/models.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/navigation.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_backup.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_backup.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_compliance.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_intended.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/config_intended.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/processor.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/nornir_plays/processor.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/signals.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css` & `nautobot_golden_config-1.4.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js` & `nautobot_golden_config-1.4.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tables.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/template_content.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/content_template.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/content_template.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 {% extends 'generic/object_detail.html' %}
 {% load helpers %}
+{% load buttons %}
+
+{% block buttons %}
+    {% if perms.nautobot_golden_config.add_goldenconfigsetting %}
+        {% clone_button object %}
+    {% endif %}
+    {% if perms.nautobot_golden_config.change_goldenconfigsetting %}
+        {% edit_button object key="pk" %}
+    {% endif %}
+    {% if perms.nautobot_golden_config.delete_goldenconfigsetting %}
+        {% delete_button object key="pk" %}
+    {% endif %}
+{% endblock buttons %}
 
 {% block content_left_page %}
 <div class="panel panel-default">
   <div class="panel-heading">
     <strong>General Settings</strong>
   </div>
   <table class="table table-hover panel-body attr-table">
```

#### html2text {}

```diff
@@ -1,8 +1,14 @@
-{% extends 'generic/object_detail.html' %} {% load helpers %} {% block
+{% extends 'generic/object_detail.html' %} {% load helpers %} {% load buttons
+%} {% block buttons %} {% if
+perms.nautobot_golden_config.add_goldenconfigsetting %} {% clone_button object
+%} {% endif %} {% if perms.nautobot_golden_config.change_goldenconfigsetting %}
+{% edit_button object key="pk" %} {% endif %} {% if
+perms.nautobot_golden_config.delete_goldenconfigsetting %} {% delete_button
+object key="pk" %} {% endif %} {% endblock buttons %} {% block
 content_left_page %}
 General Settings
 Weight             {{ object.weight }}
 Description        {{ object.description|placeholder }}
 Dynamic Group      {{_object.dynamic_group.name_}}
 Filter Query Logic {{ object.scope|render_json }}
 Scope of Devices   {{_object.get_url_to_filtered_device_list_|_length_}}
```

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html` & `nautobot_golden_config-1.4.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/conftest.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/forms/test_golden_config_settings.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/forms/test_golden_config_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_api.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_basic.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_datasources.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_filters.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_graphql.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_helpers.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_models.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_git.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_graphql.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_helpers.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_utils.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_views.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/urls.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/config_postprocessing.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/config_postprocessing.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/constant.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/constant.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/db_management.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/db_management.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/git.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/graphql.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/helper.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/management.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/management.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/utils.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/nautobot_golden_config/views.py` & `nautobot_golden_config-1.4.1/nautobot_golden_config/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.4.0/pyproject.toml` & `nautobot_golden_config-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-golden-config"
-version = "v1.4.0"
+version = "v1.4.1"
 description = "A plugin for configuration on nautobot"
 authors = ["Network to Code, LLC", "<opensource@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-golden-config"
```

### Comparing `nautobot_golden_config-1.4.0/PKG-INFO` & `nautobot_golden_config-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-golden-config
-Version: 1.4.0
+Version: 1.4.1
 Summary: A plugin for configuration on nautobot
 Home-page: https://github.com/nautobot/nautobot-plugin-golden-config
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-golden-config Version: 1.4.0 Summary: A
+Metadata-Version: 2.1 Name: nautobot-golden-config Version: 1.4.1 Summary: A
 plugin for configuration on nautobot Home-page: https://github.com/nautobot/
 nautobot-plugin-golden-config License: Apache-2.0 Keywords: nautobot,nautobot-
 plugin Author: Network to Code, LLC Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

