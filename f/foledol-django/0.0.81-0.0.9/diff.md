# Comparing `tmp/foledol-django-0.0.81.tar.gz` & `tmp/foledol-django-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/lde/foledol/django/dist/.tmp-twj9cgt5/foledol-django-0.0.81.tar", last modified: Sat May  6 16:54:00 2023, max compression
+gzip compressed data, was "/Users/lde/foledol/django/dist/tmp6a857d0g/foledol-django-0.0.9.tar", last modified: Fri Feb 11 12:46:32 2022, max compression
```

## Comparing `foledol-django-0.0.81.tar` & `foledol-django-0.0.9.tar`

### file list

```diff
@@ -1,116 +1,104 @@
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/
--rw-r--r--   0 lde        (502) staff       (20)     1073 2022-02-04 10:23:15.000000 foledol-django-0.0.81/LICENSE
--rw-r--r--   0 lde        (502) staff       (20)      129 2022-02-07 21:01:06.000000 foledol-django-0.0.81/MANIFEST.in
--rw-r--r--   0 lde        (502) staff       (20)      437 2023-05-06 16:54:00.000000 foledol-django-0.0.81/PKG-INFO
--rw-r--r--   0 lde        (502) staff       (20)       59 2022-02-06 15:03:04.000000 foledol-django-0.0.81/README.md
--rw-r--r--   0 lde        (502) staff       (20)      136 2022-02-04 21:46:36.000000 foledol-django-0.0.81/pyproject.toml
--rw-r--r--   0 lde        (502) staff       (20)      502 2023-05-06 16:54:00.000000 foledol-django-0.0.81/setup.cfg
--rw-r--r--   0 lde        (502) staff       (20)      211 2022-02-04 22:20:16.000000 foledol-django-0.0.81/setup.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/__init__.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)       87 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/apps.py
--rw-r--r--   0 lde        (502) staff       (20)     1056 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/auth.py
--rw-r--r--   0 lde        (502) staff       (20)     1292 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/logger.py
--rw-r--r--   0 lde        (502) staff       (20)     5401 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/meta.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/migrations/
--rw-r--r--   0 lde        (502) staff       (20)     1724 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0001_initial.py
--rw-r--r--   0 lde        (502) staff       (20)     2142 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0002_auto_20220211_0730.py
--rw-r--r--   0 lde        (502) staff       (20)     1810 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0003_auto_20220212_1614.py
--rw-r--r--   0 lde        (502) staff       (20)      603 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0004_auto_20220212_1620.py
--rw-r--r--   0 lde        (502) staff       (20)      415 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0005_grid_filter.py
--rw-r--r--   0 lde        (502) staff       (20)      681 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0006_auto_20220610_0534.py
--rw-r--r--   0 lde        (502) staff       (20)      360 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0007_auto_20220610_0642.py
--rw-r--r--   0 lde        (502) staff       (20)     2600 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0008_auto_20230210_1029.py
--rw-r--r--   0 lde        (502) staff       (20)      772 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0009_auto_20230210_1430.py
--rw-r--r--   0 lde        (502) staff       (20)      456 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0010_auto_20230210_1447.py
--rw-r--r--   0 lde        (502) staff       (20)      379 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/0011_auto_20230211_1150.py
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/migrations/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)    13530 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/models.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/reports/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/reports/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)     2914 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/reports/grid.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/static/
--rw-r--r--   0 lde        (502) staff       (20)     4963 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/static/foledol-django.js
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/templates/
--rw-r--r--   0 lde        (502) staff       (20)     6148 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/.DS_Store
--rw-r--r--   0 lde        (502) staff       (20)     2497 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/column.html
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/templates/common/
--rw-r--r--   0 lde        (502) staff       (20)      852 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/common/archive.html
--rw-r--r--   0 lde        (502) staff       (20)      911 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/common/delete.html
--rw-r--r--   0 lde        (502) staff       (20)      127 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/common/error.html
--rw-r--r--   0 lde        (502) staff       (20)     1121 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/common/print.html
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/templates/components/
--rw-r--r--   0 lde        (502) staff       (20)      341 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/banners.html
--rw-r--r--   0 lde        (502) staff       (20)      436 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_check.html
--rw-r--r--   0 lde        (502) staff       (20)      469 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_check_short.html
--rw-r--r--   0 lde        (502) staff       (20)     1339 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_city.html
--rw-r--r--   0 lde        (502) staff       (20)     1661 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_country.html
--rw-r--r--   0 lde        (502) staff       (20)      559 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_date.html
--rw-r--r--   0 lde        (502) staff       (20)      447 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_date_short.html
--rw-r--r--   0 lde        (502) staff       (20)      682 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_select.html
--rw-r--r--   0 lde        (502) staff       (20)      847 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_select_short.html
--rw-r--r--   0 lde        (502) staff       (20)      573 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_text.html
--rw-r--r--   0 lde        (502) staff       (20)      565 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_text_area.html
--rw-r--r--   0 lde        (502) staff       (20)      598 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_text_area_short.html
--rw-r--r--   0 lde        (502) staff       (20)     2597 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_text_short.html
--rw-r--r--   0 lde        (502) staff       (20)     1339 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/field_zip.html
--rw-r--r--   0 lde        (502) staff       (20)     3443 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/grid.html
--rw-r--r--   0 lde        (502) staff       (20)     1104 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/grid_column.html
--rw-r--r--   0 lde        (502) staff       (20)     3307 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/grid_condition_group.html
--rw-r--r--   0 lde        (502) staff       (20)      779 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/grid_row.html
--rw-r--r--   0 lde        (502) staff       (20)      258 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/list.html
--rw-r--r--   0 lde        (502) staff       (20)      722 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/logs.html
--rw-r--r--   0 lde        (502) staff       (20)      466 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/meta.html
--rw-r--r--   0 lde        (502) staff       (20)     1235 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/navigator.html
--rw-r--r--   0 lde        (502) staff       (20)      450 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/navigator_inputs.html
--rw-r--r--   0 lde        (502) staff       (20)     2869 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/paginator.html
--rw-r--r--   0 lde        (502) staff       (20)      260 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/report.html
--rw-r--r--   0 lde        (502) staff       (20)     9328 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/table.html
--rw-r--r--   0 lde        (502) staff       (20)      184 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/table_column.html
--rw-r--r--   0 lde        (502) staff       (20)      497 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/table_header.html
--rw-r--r--   0 lde        (502) staff       (20)     1912 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/components/upload.html
--rw-r--r--   0 lde        (502) staff       (20)     3360 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/condition.html
--rw-r--r--   0 lde        (502) staff       (20)     7800 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/grid.html
--rw-r--r--   0 lde        (502) staff       (20)     2377 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/log.html
--rw-r--r--   0 lde        (502) staff       (20)      509 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/log_events.html
--rw-r--r--   0 lde        (502) staff       (20)     1014 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/table_view.html
--rw-r--r--   0 lde        (502) staff       (20)      716 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/user_login.html
--rw-r--r--   0 lde        (502) staff       (20)       63 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templates/user_logout.html
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/templatetags/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templatetags/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)      703 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templatetags/custom.py
--rw-r--r--   0 lde        (502) staff       (20)      561 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templatetags/date_extras.py
--rw-r--r--   0 lde        (502) staff       (20)     2744 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/templatetags/form_extras.py
--rw-r--r--   0 lde        (502) staff       (20)     4418 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/test.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/tools/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)      987 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/barcode.py
--rw-r--r--   0 lde        (502) staff       (20)     1632 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/canvas.py
--rw-r--r--   0 lde        (502) staff       (20)     1317 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/chart.py
--rw-r--r--   0 lde        (502) staff       (20)     7488 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/field.py
--rw-r--r--   0 lde        (502) staff       (20)      362 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/filter.py
--rw-r--r--   0 lde        (502) staff       (20)     2007 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/form.py
--rw-r--r--   0 lde        (502) staff       (20)      942 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/handlers.py
--rw-r--r--   0 lde        (502) staff       (20)     1056 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/readers.py
--rw-r--r--   0 lde        (502) staff       (20)     4119 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/report.py
--rw-r--r--   0 lde        (502) staff       (20)     3822 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/table.py
--rw-r--r--   0 lde        (502) staff       (20)     2414 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/tools/writer.py
--rw-r--r--   0 lde        (502) staff       (20)     1605 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/urls.py
--rw-r--r--   0 lde        (502) staff       (20)    14592 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/utils.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol/django/views/
--rw-r--r--   0 lde        (502) staff       (20)        0 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/__init__.py
--rw-r--r--   0 lde        (502) staff       (20)     3293 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/column.py
--rw-r--r--   0 lde        (502) staff       (20)      728 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/columns.py
--rw-r--r--   0 lde        (502) staff       (20)     4618 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/condition.py
--rw-r--r--   0 lde        (502) staff       (20)      856 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/conditions.py
--rw-r--r--   0 lde        (502) staff       (20)    19300 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/grid.py
--rw-r--r--   0 lde        (502) staff       (20)     1218 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/grids.py
--rw-r--r--   0 lde        (502) staff       (20)     4908 2023-05-06 16:53:48.000000 foledol-django-0.0.81/src/foledol/django/views/logs.py
-drwxr-xr-x   0 lde        (502) staff       (20)        0 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol_django.egg-info/
--rw-r--r--   0 lde        (502) staff       (20)      437 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol_django.egg-info/PKG-INFO
--rw-r--r--   0 lde        (502) staff       (20)     4384 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol_django.egg-info/SOURCES.txt
--rw-r--r--   0 lde        (502) staff       (20)        1 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol_django.egg-info/dependency_links.txt
--rw-r--r--   0 lde        (502) staff       (20)        8 2023-05-06 16:54:00.000000 foledol-django-0.0.81/src/foledol_django.egg-info/top_level.txt
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/
+-rw-r--r--   0 lde        (502) staff       (20)     1073 2022-02-04 10:23:15.000000 foledol-django-0.0.9/LICENSE
+-rw-r--r--   0 lde        (502) staff       (20)      129 2022-02-07 21:01:06.000000 foledol-django-0.0.9/MANIFEST.in
+-rw-r--r--   0 lde        (502) staff       (20)      472 2022-02-11 12:46:32.000000 foledol-django-0.0.9/PKG-INFO
+-rw-r--r--   0 lde        (502) staff       (20)       59 2022-02-06 15:03:04.000000 foledol-django-0.0.9/README.md
+-rw-r--r--   0 lde        (502) staff       (20)      136 2022-02-04 21:46:36.000000 foledol-django-0.0.9/pyproject.toml
+-rw-r--r--   0 lde        (502) staff       (20)      501 2022-02-11 12:46:32.000000 foledol-django-0.0.9/setup.cfg
+-rw-r--r--   0 lde        (502) staff       (20)      211 2022-02-04 22:20:16.000000 foledol-django-0.0.9/setup.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/__init__.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)       87 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/apps.py
+-rw-r--r--   0 lde        (502) staff       (20)     1269 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/auth.py
+-rw-r--r--   0 lde        (502) staff       (20)      868 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/logger.py
+-rw-r--r--   0 lde        (502) staff       (20)     4869 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/meta.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/migrations/
+-rw-r--r--   0 lde        (502) staff       (20)     1724 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/migrations/0001_initial.py
+-rw-r--r--   0 lde        (502) staff       (20)     2142 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/migrations/0002_auto_20220211_0730.py
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/migrations/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)     7438 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/models.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/reports/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/reports/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)     2937 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/reports/grid.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/templates/
+-rw-r--r--   0 lde        (502) staff       (20)     6148 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/.DS_Store
+-rw-r--r--   0 lde        (502) staff       (20)     2601 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/column.html
+-rw-r--r--   0 lde        (502) staff       (20)      374 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/columns.html
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/templates/common/
+-rw-r--r--   0 lde        (502) staff       (20)      852 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/common/archive.html
+-rw-r--r--   0 lde        (502) staff       (20)      911 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/common/delete.html
+-rw-r--r--   0 lde        (502) staff       (20)      127 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/common/error.html
+-rw-r--r--   0 lde        (502) staff       (20)     1121 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/common/print.html
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/templates/components/
+-rw-r--r--   0 lde        (502) staff       (20)      341 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/banners.html
+-rw-r--r--   0 lde        (502) staff       (20)      395 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_check.html
+-rw-r--r--   0 lde        (502) staff       (20)      284 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_check_new.html
+-rw-r--r--   0 lde        (502) staff       (20)      414 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_check_short.html
+-rw-r--r--   0 lde        (502) staff       (20)     1191 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_city.html
+-rw-r--r--   0 lde        (502) staff       (20)     1661 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_country.html
+-rw-r--r--   0 lde        (502) staff       (20)      541 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_date.html
+-rw-r--r--   0 lde        (502) staff       (20)      441 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_date_short.html
+-rw-r--r--   0 lde        (502) staff       (20)      652 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_select.html
+-rw-r--r--   0 lde        (502) staff       (20)      835 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_select_short.html
+-rw-r--r--   0 lde        (502) staff       (20)      632 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_text.html
+-rw-r--r--   0 lde        (502) staff       (20)      547 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_text_area.html
+-rw-r--r--   0 lde        (502) staff       (20)      586 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_text_area_short.html
+-rw-r--r--   0 lde        (502) staff       (20)     2519 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_text_short.html
+-rw-r--r--   0 lde        (502) staff       (20)     1192 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/field_zip.html
+-rw-r--r--   0 lde        (502) staff       (20)     2716 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/grid.html
+-rw-r--r--   0 lde        (502) staff       (20)     1090 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/grid_column.html
+-rw-r--r--   0 lde        (502) staff       (20)      779 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/grid_row.html
+-rw-r--r--   0 lde        (502) staff       (20)      258 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/list.html
+-rw-r--r--   0 lde        (502) staff       (20)      700 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/logs.html
+-rw-r--r--   0 lde        (502) staff       (20)      466 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/meta.html
+-rw-r--r--   0 lde        (502) staff       (20)     1235 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/navigator.html
+-rw-r--r--   0 lde        (502) staff       (20)      450 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/navigator_inputs.html
+-rw-r--r--   0 lde        (502) staff       (20)     2869 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/paginator.html
+-rw-r--r--   0 lde        (502) staff       (20)      260 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/report.html
+-rw-r--r--   0 lde        (502) staff       (20)     6617 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/table.html
+-rw-r--r--   0 lde        (502) staff       (20)      135 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/table_column.html
+-rw-r--r--   0 lde        (502) staff       (20)      497 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/table_header.html
+-rw-r--r--   0 lde        (502) staff       (20)     1912 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/components/upload.html
+-rw-r--r--   0 lde        (502) staff       (20)     4625 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/grid.html
+-rw-r--r--   0 lde        (502) staff       (20)      372 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/grids.html
+-rw-r--r--   0 lde        (502) staff       (20)     2379 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/log.html
+-rw-r--r--   0 lde        (502) staff       (20)      509 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/log_events.html
+-rw-r--r--   0 lde        (502) staff       (20)      681 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/logs.html
+-rw-r--r--   0 lde        (502) staff       (20)      716 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/user_login.html
+-rw-r--r--   0 lde        (502) staff       (20)       63 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templates/user_logout.html
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/templatetags/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templatetags/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)      703 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templatetags/custom.py
+-rw-r--r--   0 lde        (502) staff       (20)      564 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templatetags/date_extras.py
+-rw-r--r--   0 lde        (502) staff       (20)     1780 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/templatetags/form_extras.py
+-rw-r--r--   0 lde        (502) staff       (20)     4418 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/test.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/tools/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)      960 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/barcode.py
+-rw-r--r--   0 lde        (502) staff       (20)     1632 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/canvas.py
+-rw-r--r--   0 lde        (502) staff       (20)     1317 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/chart.py
+-rw-r--r--   0 lde        (502) staff       (20)     6834 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/field.py
+-rw-r--r--   0 lde        (502) staff       (20)      293 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/filter.py
+-rw-r--r--   0 lde        (502) staff       (20)     1970 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/form.py
+-rw-r--r--   0 lde        (502) staff       (20)      942 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/handlers.py
+-rw-r--r--   0 lde        (502) staff       (20)     1056 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/readers.py
+-rw-r--r--   0 lde        (502) staff       (20)     4119 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/report.py
+-rw-r--r--   0 lde        (502) staff       (20)     1166 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/table.py
+-rw-r--r--   0 lde        (502) staff       (20)     2414 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/tools/writer.py
+-rw-r--r--   0 lde        (502) staff       (20)     1237 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/urls.py
+-rw-r--r--   0 lde        (502) staff       (20)    12733 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/utils.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol/django/views/
+-rw-r--r--   0 lde        (502) staff       (20)        0 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/__init__.py
+-rw-r--r--   0 lde        (502) staff       (20)     4575 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/column.py
+-rw-r--r--   0 lde        (502) staff       (20)     1179 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/columns.py
+-rw-r--r--   0 lde        (502) staff       (20)    12811 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/grid.py
+-rw-r--r--   0 lde        (502) staff       (20)     1374 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/grids.py
+-rw-r--r--   0 lde        (502) staff       (20)     5260 2022-02-11 12:45:12.000000 foledol-django-0.0.9/src/foledol/django/views/logs.py
+drwxr-xr-x   0 lde        (502) staff       (20)        0 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol_django.egg-info/
+-rw-r--r--   0 lde        (502) staff       (20)      472 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol_django.egg-info/PKG-INFO
+-rw-r--r--   0 lde        (502) staff       (20)     3784 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol_django.egg-info/SOURCES.txt
+-rw-r--r--   0 lde        (502) staff       (20)        1 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol_django.egg-info/dependency_links.txt
+-rw-r--r--   0 lde        (502) staff       (20)        8 2022-02-11 12:46:32.000000 foledol-django-0.0.9/src/foledol_django.egg-info/top_level.txt
```

### Comparing `foledol-django-0.0.81/LICENSE` & `foledol-django-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/auth.py` & `foledol-django-0.0.9/src/foledol/django/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # -*- coding: utf-8 -*-
 
+import json
+import urllib
+import urllib.request
+import uuid
+
 from django.conf import settings
 from django.contrib.auth import authenticate, login, logout
 from django.contrib.auth.models import User
+from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.urls import reverse
 
+from .models import Log
+from foledol.django.utils import get_param, check_length, send_mail2
+
 
 def user_login(request):
     error = None
     if 'username' in request.POST and 'password' in request.POST:
         username = request.POST['username']
         password = request.POST['password']
         user = authenticate(request, username=username, password=password)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/logger.py` & `foledol-django-0.0.9/src/foledol/django/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,32 @@
-from datetime import datetime
-
 from django.contrib.auth.models import User
 
 from .meta import get_user_or_superuser
 from .models import Log, LogItem
-from .utils import get_local_date
 
 
 def log(ref, model, action, user=None, old='', new='', transaction=None):
-
-    def too_big(value):
-        return value and isinstance(value, str) and len(value) > 126
-
     _log = Log(user=get_user_or_superuser(user))
-    _log.date = get_local_date()
     _log.ref = ref
     _log.model = model
     _log.action = action
     _log.transaction = transaction
     _log.save()
 
     if old and new:
         diff = {}
         for key in new.keys():
             if old[key] != new[key]:
                 diff[key] = (old[key], new[key])
         for key in diff.keys():
-            if not too_big(diff[key][0]) and not too_big(diff[key][1]):
-                try:
-                    _log_item = LogItem()
-                    _log_item.log = _log
-                    _log_item.key = key
-                    _log_item.old = diff[key][0]
-                    _log_item.new = diff[key][1]
-                    _log_item.save()
-                except Exception as ex:
-                    print("Exception:" + str(ex))
+            _log_item = LogItem()
+            _log_item.log = _log
+            _log_item.key = key
+            _log_item.old = diff[key][0]
+            _log_item.new = diff[key][1]
+            _log_item.save()
 
 
 def logs(ref, model):
     return Log.objects.all().filter(ref=ref).filter(model=model).order_by('-date')
```

### Comparing `foledol-django-0.0.81/src/foledol/django/meta.py` & `foledol-django-0.0.9/src/foledol/django/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,69 +99,55 @@
 def write_headers(fields, worksheet, row, format):
     i = 0
     for field in fields:
         worksheet.write(row, i, field.label, format)
         i += 1
 
 
-def write_value(worksheet, row, i, value, format=None):
-    if format:
-        worksheet.write(row, i, value, format)
-    else:
-        worksheet.write(row, i, value)
-
-
-def write_values(fields, values, worksheet, row, format=None, date_format=None):
+def write_values(fields, values, worksheet, row, format=None):
     i = 0
     for field in fields:
         value = values[field.name]
         if field.format == FORMAT_BOOLEAN and field.values and value in field.values:
             value = field.values[value]
-        if field.format == FORMAT_DATE and value:
-            value = value.strftime("%d/%m/%Y")
-            write_value(worksheet, row, i, value, date_format)
+        if format:
+            worksheet.write(row, i, value, format)
         else:
-            write_value(worksheet, row, i, value, format)
+            worksheet.write(row, i, value)
         i += 1
 
 
 def export_to_worksheet(workbook, items, fields, title):
     format_header = workbook.add_format()
     format_header.set_bold(True)
     format_header.set_align('top')
     format_header.set_align('center')
     format_header.set_text_wrap(True)
 
-    date_format = workbook.add_format({'num_format': 'dd/mm/yyyy'})
-
     worksheet = workbook.add_worksheet(title)
     worksheet.set_landscape()
 
     write_headers(fields, worksheet, 0, format_header)
     row = 1
     for item in items:
         values = get_fields(item, fields)
-        write_values(fields, values, worksheet, row, format=None, date_format=date_format)
+        write_values(fields, values, worksheet, row)
         row += 1
 
     workbook.close()
 
 
-def export_to_workbook_buffer(items, fields, title):
+def export_to_workbook(items, fields, filename, title):
     output = io.BytesIO()
 
     workbook = xlsxwriter.Workbook(output, {'in_memory': True})
     export_to_worksheet(workbook, items, fields, title)
 
     output.seek(0)
-    return output
-
 
-def export_to_workbook(items, fields, filename, title):
-    output = export_to_workbook_buffer(items, fields, title)
     response = HttpResponse(
         output,
         content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
     )
     response['Content-Disposition'] = 'attachment; filename="' + filename + '.xlsx"'
     return response
```

### Comparing `foledol-django-0.0.81/src/foledol/django/migrations/0001_initial.py` & `foledol-django-0.0.9/src/foledol/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/migrations/0002_auto_20220211_0730.py` & `foledol-django-0.0.9/src/foledol/django/migrations/0002_auto_20220211_0730.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/reports/grid.py` & `foledol-django-0.0.9/src/foledol/django/reports/grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from io import BytesIO
 
 from reportlab.lib.pagesizes import landscape, letter
 
-from foledol.django.templatetags.form_extras import value, value_as_str
+from foledol.django.templatetags.form_extras import value
 from foledol.django.tools.canvas import NumberedPageCanvas
 from foledol.django.tools.report import Report, ReportColumn
 
 
 class GridReport(Report):
     def __init__(self, title, grid, fields):
         self.title = title
         self.grid = grid
         self.fields = fields
         self.columns = []
         for column in self.grid.column_set.all().order_by('order'):
             field = self.get_field(column.label)
-            if field:
+            if field and not column.hidden:
                 width = column.width if column.width and column.width > 0 else 60
                 self.columns.append(
                     ReportColumn(width, field.label)
                 )
 
     def get_field(self, key):
         for field in self.fields:
@@ -51,16 +51,16 @@
         y = 540
         page.setFont(self.font, 8)
         for row in rows:
 
             values = []
             for column in self.grid.column_set.all():
                 field = self.get_field(column.label)
-                if field:
-                    values.append(str(row[column.label] if self.grid.group_by else value_as_str(row, column.label)))
+                if field and not column.hidden:
+                    values.append(str(row[column.label] if self.grid.group_by else value(row, column.label)))
 
             i = 0
             max_height = 0
             for column in self.columns:
                 height = self.get_height(values[i], self.font, 8, column.width)
                 if height > max_height:
                     max_height = height
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/.DS_Store` & `foledol-django-0.0.9/src/foledol/django/templates/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 00000260: 08d9 8914 29ce d9c3 4100 0000 0600 6300  ....)...A.....c.
 00000270: 6f00 6d00 6d00 6f00 6e6d 6f64 4462 6c6f  o.m.m.o.nmodDblo
 00000280: 6200 0000 08d9 8914 29ce d9c3 4100 0000  b.......)...A...
 00000290: 0600 6300 6f00 6d00 6d00 6f00 6e70 6831  ..c.o.m.m.o.nph1
 000002a0: 5363 6f6d 7000 0000 0000 0040 0000 0000  Scomp......@....
 000002b0: 0a00 6300 6f00 6d00 7000 6f00 6e00 6500  ..c.o.m.p.o.n.e.
 000002c0: 6e00 7400 736c 6731 5363 6f6d 7000 0000  n.t.slg1Scomp...
-000002d0: 0000 0090 5600 0000 0a00 6300 6f00 6d00  ....V.....c.o.m.
+000002d0: 0000 007d d700 0000 0a00 6300 6f00 6d00  ...}......c.o.m.
 000002e0: 7000 6f00 6e00 6500 6e00 7400 736d 6f44  p.o.n.e.n.t.smoD
-000002f0: 4462 6c6f 6200 0000 0832 b271 742e d1c4  Dblob....2.qt...
+000002f0: 4462 6c6f 6200 0000 0884 c617 29ce d9c3  Dblob.......)...
 00000300: 4100 0000 0a00 6300 6f00 6d00 7000 6f00  A.....c.o.m.p.o.
 00000310: 6e00 6500 6e00 7400 736d 6f64 4462 6c6f  n.e.n.t.smodDblo
-00000320: 6200 0000 0832 b271 742e d1c4 4100 0000  b....2.qt...A...
+00000320: 6200 0000 0884 c617 29ce d9c3 4100 0000  b.......)...A...
 00000330: 0a00 6300 6f00 6d00 7000 6f00 6e00 6500  ..c.o.m.p.o.n.e.
 00000340: 6e00 7400 7370 6831 5363 6f6d 7000 0000  n.t.sph1Scomp...
 00000350: 0000 01e0 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/column.html` & `foledol-django-0.0.9/src/foledol/django/templates/column.html`

 * *Files 18% similar despite different names*

```diff
@@ -26,27 +26,29 @@
                             {% endfor %}
                         </select>
                     </div>
                 </div>
 
                 <div class="form-group">
                     <div class="col-sm-4">
-                        <label>Tri</label>
+                        <label>Critère</label>
                     </div>
                     <div class="col-sm-8">
-                        <select name="order_by" class="form-control">
-                            <option value="0" {% if order_by == 0 %}selected{% endif %}>(Aucun)</option>
-                            <option value="1" {% if order_by == 1 %}selected{% endif %}>Ascendant</option>
-                            <option value="2" {% if order_by == 2 %}selected{% endif %}>Descendant</option>
+                        <select name="criteria" class="form-control">
+                            {% for key, value in criteria_set.items %}
+                            <option value="{{key}}" {% if criteria == key %}selected{% endif %}>{{value}}</option>
+                            {% endfor %}
                         </select>
                     </div>
                 </div>
 
+                {% include "components/field_text_short.html" with field=form|field:'value' %}
                 {% include "components/field_text_short.html" with field=form|field:'order' %}
                 {% include "components/field_text_short.html" with field=form|field:'width' %}
+                {% include "components/field_check_short.html" with field=form|field:'hidden' %}
 
             </div>
             <div class="panel-footer">
                 <button type="button" class="btn btn-default" onclick="go_back('{{ back }}')">Annuler</button>
                 <button type="submit" class="btn btn-primary">Enregistrer</button>
                 {% if user.is_staff and column %}
                 <button type="button" class="btn btn-danger" onclick="open2('{% url 'django:column_delete' column.id %}')">Supprimer</button>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/common/archive.html` & `foledol-django-0.0.9/src/foledol/django/templates/common/archive.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/common/delete.html` & `foledol-django-0.0.9/src/foledol/django/templates/common/delete.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/common/print.html` & `foledol-django-0.0.9/src/foledol/django/templates/common/print.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_city.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_zip.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 <div class="{{class}}">
     <div class="form-group">
-        <label id="label_auto_ci" name="label_auto_ci"></label>
-        <input id="auto_ci" name="auto_ci"
+        <label id="label_auto_zi" name="label_auto_zi"></label>
+        <input id="auto_zi" name="auto_zi"
                class="form-control"
                type="text"
-               value="{{city}}"
+               value="{{zip}}"
                 {% if tabindex %} tabindex="{{tabindex}}"{% endif %}
                spellcheck="false" autocorrect="off" autocomplete="off"/>
-        <input type="hidden" id="city" name="city" value="{{city}}"/>
+        <input type="hidden" id="zip" name="zip" value="{{zip}}"/>
     </div>
 </div>
 
 <script>
     $(document).ready(function(){
-        setLabel('label_auto_ci', "Commune");
-        $("#auto_ci").change( function () {
-          document.getElementById('city').value = document.getElementById('auto_ci').value;
-        });
-        $("#auto_ci").autocomplete({
-            source: "/city_autocomplete/",
+        setLabel('label_auto_zi', "Code postal");
+        $("#auto_zi").autocomplete({
+            source: "/zip_autocomplete/",
             minLength: 1,
             open: function(){
                 setTimeout(function () {
                     $('.ui-autocomplete').css('z-index', 99);
                 }, 0);
             },
             select: function (event, ui) {
-                setZipAndCity(ui.item.zip, ui.item.value);
+                setZipAndCity(ui.item.value, ui.item.city);
             },
             focus: function (event, ui) {
-                setZipAndCity(ui.item.zip, ui.item.value);
+                setZipAndCity(ui.item.value, ui.item.city);
                 event.cancelled = true
             }
         });
-        registerZipAndCity('auto_ci');
+        registerZipAndCity('auto_zi');
     });
 </script>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_country.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_country.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_date.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_date.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <div class="{{class}}">
     <div class="form-group">
-        <label for="{{field.full_name}}">{{field.label}}</label>
-        <input id="{{field.full_name}}"
-               name="{{field.full_name}}"
+        <label for="{{field.key}}">{{field.label}}</label>
+        <input id="{{field.key}}"
+               name="{{field.key}}"
                class="form-control"
                type="text"
                value="{{field.value_as_str}}"
                {% if tabindex %} tabindex="{{tabindex}}"{% endif %}
                {% if field.disabled %}disabled{% endif %}/>
         {% for error in field.errors %}
         <div class="red">{{ error }}</div>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_select.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_select.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div class="{{class}}">
     <div class="form-group">
-        <label for="{{field.full_name}}">{{field.label}}</label>
+        <label for="{{field.key}}">{{field.label}}</label>
         {% if field.disabled %}
-        <input id="{{field.full_name}}" name="{{field.full_name}}" class="form-control" type="text" value="{{field.value}}" disabled/>
+        <input id="{{field.key}}" name="{{field.key}}" class="form-control" type="text" value="{{field.value}}" disabled/>
         {% else %}
-        <select id="{{field.full_name}}" name="{{field.full_name}}" class="form-control" {% if tabindex %} tabindex="{{tabindex}}"{% endif %}>
+        <select id="{{field.key}}" name="{{field.key}}" class="form-control" {% if tabindex %} tabindex="{{tabindex}}"{% endif %}>
             {% for value in field.values %}
             <option value="{{ value }}" {% if field.value == value %}selected{% endif %}>{{ value }}</option>
             {% endfor %}
         </select>
         {% endif %}
     </div>
 </div>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_select_short.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_select_short.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div class="form-group">
     <div class="col-sm-4"><label>{{field.label}}</label></div>
     <div class="col-sm-8">
         {% if field.disabled %}
-        <input name="{{field.full_name}}" class="form-control" type="text" value="{{field.value}}" disabled/>
+        <input name="{{field.key}}" class="form-control" type="text" value="{{field.value}}" disabled/>
         {% else %}
-        <select name="{{field.full_name}}" class="form-control">
+        <select name="{{field.key}}" class="form-control">
             {% if field.pairs %}
             {% for value, label in field.pairs.items %}
             <option value="{{ value }}" {% if field.value == value %}selected{% endif %}>{{ label }}</option>
             {% endfor %}
             {% else %}
             {% for value in field.values %}
             <option value="{{ value }}" {% if field.value == value %}selected{% endif %}>{{ value }}</option>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_text.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_text.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-<div class="form-group {{class}}">
-    <label for="{{field.full_name}}">{{field.label}}</label>
-    <input id="{{field.full_name}}"
-           name="{{field.full_name}}"
-           class="form-control"
-           type="text"
-           value="{{field.value_as_str}}"
-           {% if tabindex %} tabindex="{{tabindex}}"{% endif %}
-           {% if field.disabled %}disabled{% endif %}
-           {% if field.autocomplete %}autocomplete="{{field.autocomplete}}"{% endif %}/>
-    {% for error in field.errors %}
-    <div class="red">{{ error }}</div>
-    {% endfor %}
+<div class="{{class}}">
+    <div class="form-group">
+        <label for="{{field.key}}">{{field.label}}</label>
+        <input id="{{field.key}}"
+               name="{{field.key}}"
+               class="form-control"
+               type="text"
+               value="{{field.value_as_str}}"
+               {% if tabindex %} tabindex="{{tabindex}}"{% endif %}
+               {% if field.disabled %}disabled{% endif %}
+               {% if field.autocomplete %}autocomplete="{{field.autocomplete}}"{% endif %}/>
+        {% for error in field.errors %}
+        <div class="red">{{ error }}</div>
+        {% endfor %}
+    </div>
 </div>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_text_area_short.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_text_area_short.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <div class="form-group">
     <div class="col-sm-4">
         <label>
             {{field.label}}
         </label>
     </div>
     <div class="col-sm-8">
-        <textarea id="{{field.full_name}}"
-            name="{{field.full_name}}"
+        <textarea id="{{field.key}}"
+            name="{{field.key}}"
             class="form-control"
             type="text" rows="3"
             {% if field.disabled %}disabled{% endif %}
             {% if field.autocomplete %}autocomplete="{{field.autocomplete}}"{% endif %}>{{field.value_as_str}}</textarea>
         {% for error in field.errors %}
         <div class="red">{{ error }}</div>
         {% endfor %}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_text_short.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_text_short.html`

 * *Files 25% similar despite different names*

```diff
@@ -10,53 +10,53 @@
                 {{field.label}}
                 {% endif %}
             {% endif %}
         </label>
     </div>
     {% if field.autocomplete_url %}
     <div class="col-sm-8">
-        <input id="{{field.full_name}}" name="{{field.full_name}}"
+        <input id="{{field.key}}" name="{{field.key}}"
                class="form-control"
                type="text"
                value="{{field.value_as_str}}"
                {% if field.disabled %}disabled{% endif %}
                {% if field.autocomplete %}autocomplete="{{field.autocomplete}}"{% endif %}/>
         {% for error in field.errors %}
         <div class="red">{{ error }}</div>
         {% endfor %}
     </div>
     <script>
         $(document).ready(function(){
-            $("#{{field.full_name}}").autocomplete({
+            $("#{{field.key}}").autocomplete({
                 source: "/{{field.autocomplete_url}}/",
                 minLength: 2,
                 open: function(){
                     setTimeout(function () {
                         $('.ui-autocomplete').css('z-index', 99);
                     }, 0);
                 }
               });
-            {{field.full_name}}_old_value = null;
-            document.getElementById('{{field.full_name}}').onfocus = function() {
-                {{field.full_name}}_old_value = document.getElementById('{{field.full_name}}').value
+            {{field.key}}_old_value = null;
+            document.getElementById('{{field.key}}').onfocus = function() {
+                {{field.key}}_old_value = document.getElementById('{{field.key}}').value
             };
-            document.getElementById('{{field.full_name}}').addEventListener('keydown', function(event){
+            document.getElementById('{{field.key}}').addEventListener('keydown', function(event){
                 if (event.key === "Escape") {
-                    value = {{field.full_name}}_old_value
-                    if (value != null && value != document.getElementById("{{field.full_name}}").value) {
-                        document.getElementById('{{field.full_name}}').value = {{field.full_name}}_old_value
+                    value = {{field.key}}_old_value
+                    if (value != null && value != document.getElementById("{{field.key}}").value) {
+                        document.getElementById('{{field.key}}').value = {{field.key}}_old_value
                         event.stopPropagation();
                     }
                 }
             });
         });
     </script>
     {% else %}
     <div class="col-sm-8">
-        <input name="{{field.full_name}}"
+        <input name="{{field.key}}"
                class="form-control"
                type="text"
                value="{{field.value_as_str}}"
                {% if field.disabled %}disabled{% endif %}
                {% if field.autocomplete %}autocomplete="{{field.autocomplete}}"{% endif %}/>
         {% for error in field.errors %}
         <div class="red">{{ error }}</div>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/field_zip.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/field_city.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 <div class="{{class}}">
     <div class="form-group">
-        <label id="label_auto_zi" name="label_auto_zi"></label>
-        <input id="auto_zi" name="auto_zi"
+        <label id="label_auto_ci" name="label_auto_ci"></label>
+        <input id="auto_ci" name="auto_ci"
                class="form-control"
                type="text"
-               value="{{zip}}"
+               value="{{city}}"
                 {% if tabindex %} tabindex="{{tabindex}}"{% endif %}
                spellcheck="false" autocorrect="off" autocomplete="off"/>
-        <input type="hidden" id="zip" name="zip" value="{{zip}}"/>
+        <input type="hidden" id="city" name="city" value="{{city}}"/>
     </div>
 </div>
 
 <script>
     $(document).ready(function(){
-        setLabel('label_auto_zi', "Code postal");
-        $("#auto_zi").change( function () {
-          document.getElementById('zip').value = document.getElementById('auto_zi').value;
-        });
-        $("#auto_zi").autocomplete({
-            source: "/zip_autocomplete/",
+        setLabel('label_auto_ci', "Commune");
+        $("#auto_ci").autocomplete({
+            source: "/city_autocomplete/",
             minLength: 1,
             open: function(){
                 setTimeout(function () {
                     $('.ui-autocomplete').css('z-index', 99);
                 }, 0);
             },
             select: function (event, ui) {
-                setZipAndCity(ui.item.value, ui.item.city);
+                setZipAndCity(ui.item.zip, ui.item.value);
             },
             focus: function (event, ui) {
-                setZipAndCity(ui.item.value, ui.item.city);
+                setZipAndCity(ui.item.zip, ui.item.value);
                 event.cancelled = true
             }
         });
-        registerZipAndCity('auto_zi');
+        registerZipAndCity('auto_ci');
     });
 </script>
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/grid.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/grid.html`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 <div class="panel panel-default">
     <div class="panel-body">
 
         <table class="table" style="border-collapse: unset">
             <thead>
             {% for column in columns %}
-                {% if sort_columns %}
-                    {% if column.label in sort_columns_asc %}
-                        <th>{{column.label_as_str}}<span style="color: gray;" class="glyphicon glyphicon-sort-by-attributes"></span></th>
-                    {% elif column.label in sort_columns_desc %}
-                        <th>{{column.label_as_str}}<span style="color: gray;" class="glyphicon glyphicon-sort-by-attributes-alt"></span></th>
+                {% if not column.hidden %}
+                    {% include "components/table_header.html" with sort=sort key=column.label name=column.label_as_str %}
+                {% else %}
+                    {% if column.sortable %}
+                        {% include "components/table_header.html" with sort=sort key=column.label name=column.label_as_str %}
                     {% else %}
-                        <th>{{column.label_as_str}}</th>
+                    <th>{{column.label_as_str}}</th>
                     {% endif %}
-                {% else %}
-                    {% include "components/table_header.html" with sort=sort key=column.label name=column.label_as_str %}
                 {% endif %}
             {% endfor %}
             </thead>
             {% for row in rows %}
                 {% include "components/grid_row.html" with form=row|editor:fields row=row columns=columns %}
             {% endfor %}
         </table>
@@ -60,21 +58,10 @@
                 {% endif %}
                 {% endfor %}
             </ul>
         </div>
         {% endif %}
         <button type="button" class="btn btn-primary" onclick="send('export');">Exporter</button>
         <button type="button" class="btn btn-primary" onclick="copy_grid_to_clipboard('{{grid_url}}');">Copier</button>
-        {% if mailings %}
-        <div class="dropdown dropup">
-            <button class="btn btn-primary dropdown-toggle" type="button" data-toggle="dropdown">
-            Mailing&nbsp;<span class="caret"></span></button>
-            <ul class="dropdown-menu">
-                {% for mailing in mailings %}
-                <li><a onclick="open2('{{mailing_url}}/{{mailing.id}}');">{{mailing.label}}</a></li>
-                {% endfor %}
-            </ul>
-        </div>
-        {% endif %}
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -9,13 +9,8 @@
 %}
 
     * {% for report in reports %} {% if report.route %}
     * {{report.label}}
     * {% elif report.key %}
     * {{report.label}}
     * {% endif %} {% endfor %}
-{% endif %} Exporter Copier {% if mailings %}
- Mailing 
-    * {% for mailing in mailings %}
-    * {{mailing.label}}
-    * {% endfor %}
-{% endif %}
+{% endif %} Exporter Copier
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/grid_column.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/grid_column.html`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                    type="text"
                    value="{{ row|value:column.label }}"/>
         {% endif %}
     </td>
     {% else %}
     <td>
         {% if field|class_name == 'BooleanField' %}
-            {{ row|value_as_str:column.label }}
+            {{ row|value:column.label }}
         {% else %}
-            {{ row|value_as_str:column.label }}
+            {{ row|value:column.label }}
         {% endif %}
     </td>
     {% endif %}
 
 {% endif %}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/grid_row.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/grid_row.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/logs.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/logs.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 {% load i18n %}
-{% load date_extras %}
-
 {% if logs %}
 <div class="panel panel-default">
     <div class="panel-heading">{% trans 'logs_title' %}</div>
     <div class="panel-body">
         <table class="table">
             <thead>
             <th>{% trans 'logs_date' %}</th>
             <th>{% trans 'logs_user' %}</th>
             <th>{% trans 'logs_action' %}</th>
             </thead>
             {% for log in logs %}
             <tr onclick="goto('{% url 'django:log_update' log.id %}')">
-                <td>{{ log.date|short_datetime }}</td>
+                <td>{{ log.date|date:'d/m/Y H:i' }}</td>
                 <td>{{ log.author }}</td>
                 <td>{{ log.action }}</td>
             </tr>
             {% endfor %}
         </table>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
-{% load i18n %} {% load date_extras %} {% if logs %}
+{% load i18n %} {% if logs %}
 {% trans 'logs_title' %}
-{{ log.date|short_datetime }} {{ log.author }} {{ log.action }}
+{{ log.date|date:'d/m/Y H:i' }} {{ log.author }} {{ log.action }}
 {% endif %}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/navigator.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/navigator.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/paginator.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/paginator.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/table.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/table.html`

 * *Files 18% similar despite different names*

```diff
@@ -73,31 +73,15 @@
                           </ul>
                     </div>
                 </td>
                 {% endif %}
 
                 {% for button in table.buttons %}
                 <td>
-                    {% if button|class_name == 'TableButtonGroup' %}
-                    <div class="dropdown">
-                        <button class="btn btn-primary dropdown-toggle" type="button" data-toggle="dropdown">{{button.label}}
-                        <span class="caret"></span></button>
-                        <ul class="dropdown-menu">
-                            {% for item in button.items %}
-                                {% if item|class_name == 'TableButton' %}
-                                <li><a onclick="{{item.action}}">{{item.label}}</a></li>
-                                {% elif item|class_name == 'TableButtonDivider' %}
-                                <li role="separator" class="divider"></li>
-                                {% endif %}
-                            {% endfor %}
-                        </ul>
-                    </div>
-                    {% else %}
                     <button class="btn btn-primary mls" onclick="{{button.action}}">{{button.label}}</button>
-                    {% endif %}
                 </td>
                 {% endfor %}
             </tr>
         </table>
         {% endif %}
         {% if filter_title %}
         <div style="margin-top: 15px; margin-bottom: 10px; color: #2a437d;">{{filter_title}}</div>
@@ -130,44 +114,15 @@
                         {% include "components/table_column.html" with type=column.type value=row|get:column%}
                         {% endif %}
                         </a>
                     {% else %}
                         {% if column.method %}
                         {{ row|method:column.method }}
                         {% else %}
-                            {% if column.buttons %}
-                                {% for button in column.buttons %}
-                                    {% if button|class_name == 'TableButton' %}
-                                        <button type="button" class="btn {% if button.style %} {{button.style}} {% endif %}"
-                                            {% if not button|enabled:row %}disabled{% endif %}
-                                            {% if button|has_attr:'on_click' %}
-                                            onclick="{{button|on_click:row}}"
-                                            {% else %}
-                                            onclick="goto('{% url button.action row.id %}')"
-                                            {% endif %}
-                                        >
-                                            {% if button.label %}
-                                            {{ button.label }}
-                                            {% endif %}
-                                            {% if button.icon %}
-                                                <span class="{{button.icon}}"></span>
-                                            {% endif %}
-                                        </button>
-                                    {% endif %}
-
-                                    {% if button|class_name == 'TableButtonIcon' %}
-                                        {%if button|visible:row %}
-                                            <span class="{{button.icon}}"></span>
-                                        {% endif %}
-                                    {% endif %}
-
-                                {% endfor %}
-                            {% else %}
-                            {% include "components/table_column.html" with type=column.type value=row|get:column%}
-                            {% endif %}
+                        {% include "components/table_column.html" with type=column.type value=row|get:column%}
                         {% endif %}
                         {% endif %}
                     </td>
                 {% endfor %}
                 </tr>
             {% endfor %}
             {% endif %}
```

#### html2text {}

```diff
@@ -2,47 +2,36 @@
 table.placeholder and table.create %}
 {{table.placeholder}}
 {% else %}
 {% if table.heading %}
 {{table.heading}} {% if table.count %}({{table.count}}){% endif %}
 {% endif %}
  {% if table.search %}
-                                                                                                              {% if button|class_name ==
-                                                                                                              'TableButtonGroup' %}
-                                                                  Actions               Imprimer              {{button.label}}
-                                                                      * {% for module       * {% for report       * {% for item in
-               {% for key, value                                        in                    in                    button.items %} {%
-               in                                                       table.modules         table.reports         if item|class_name
-               table.filters.items [{                                   %} {% if              %} {% if              == 'TableButton' %}
-{% trans       %}                  {        {% trans                    module.route %}       report.route %}     * {{item.label}}
-'table_search' % if filter_key ==  search   'table_search_action'     * {                   * {                   * {% elif
-%}:            key %}selected{%    }}       %}                          {module.label}}       {report.label}}       item|class_name ==
-               endif %}>{{ value   ]                                  * {% else %}          * {% else %}            'TableButtonDivider'
-               }}                                                     * {                   * {                     %}
-               {% endfor %}                                             {module.label}}       {report.label}}     * {% endif %} {%
-                                                                      * {% endif %} {%      * {% endif %} {%        endfor %}
-                                                                        endfor %}             endfor %}       {% else %} {
-                                                                                                              {button.label}} {% endif
-                                                                                                              %}
+                                                                  Actions               Imprimer
+                                                                      * {% for module       * {% for report
+               {% for key, value                                        in                    in
+               in                                                       table.modules         table.reports
+               table.filters.items [{                                   %} {% if              %} {% if
+{% trans       %}                  {        {% trans                    module.route %}       report.route %} {
+'table_search' % if filter_key ==  search   'table_search_action'     * {                   * {               {button.label}}
+%}:            key %}selected{%    }}       %}                          {module.label}}       {report.label}}
+               endif %}>{{ value   ]                                  * {% else %}          * {% else %}
+               }}                                                     * {                   * {
+               {% endfor %}                                             {module.label}}       {report.label}}
+                                                                      * {% endif %} {%      * {% endif %} {%
+                                                                        endfor %}             endfor %}
 {% endif %} {% if filter_title %}
 {{filter_title}}
 {% endif %}
 {% if column.link %} {% if column.method %} {{ row|method:column.method }} {%
 else %} {% include "components/table_column.html" with type=column.type
 value=row|get:column%} {% endif %} {% else %} {% if column.method %} {
-{ row|method:column.method }} {% else %} {% if column.buttons %} {% for button
-in column.buttons %} {% if button|class_name == 'TableButton' %}
-% if not button|enabled:row %}disabled{% endif %} {% if button|has_attr:
-'on_click' %} onclick="{{button|on_click:row}}" {% else %} onclick="goto('{%
-url button.action row.id %}')" {% endif %} > {% if button.label %} {
-{ button.label }} {% endif %} {% if button.icon %}  {% endif %}  {% endif %} {%
-if button|class_name == 'TableButtonIcon' %} {%if button|visible:row %}  {%
-endif %} {% endif %} {% endfor %} {% else %} {% include "components/
+{ row|method:column.method }} {% else %} {% include "components/
 table_column.html" with type=column.type value=row|get:column%} {% endif %} {%
-endif %} {% endif %}
+endif %}
 {% if page_count and not no_paginate %}
  {% if pagination %}
 {% include "components/paginator.html" %}
 {% endif %}
  {{ page_count }} Ã©lÃ©ment(s)
 {% endif %}
 {% if table.create %}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/components/upload.html` & `foledol-django-0.0.9/src/foledol/django/templates/components/upload.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/condition.html` & `foledol-django-0.0.9/src/foledol/django/templates/grid.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,124 @@
 {% extends base %}
 {% load form_extras %}
+{% load custom %}
 
 {% block content %}
 
     <script>
-        function set_values_for(key) {
-            html="";
-            {% for field in fields %}
-                {% if field.pairs %}
-                    if (key == '{{field.key}}') {
-                        html += "<ul>";
-                        {% for key, value in field.pairs.items %}
-                        html += "<li>{{key}}-{{value}}</li>";
-                        {% endfor %}
-                        html += "</ul>";
-                    }
-                {% endif %}
-            {% endfor %}
-            document.getElementById('values').innerHTML = html;
+        function group_by(query) {
+            open2("{{ group_by_url }}?" + query)
         }
-        function set_values() {
-            set_values_for(document.getElementById('field_key').value);
+        function copy_grid_to_clipboard(url) {
+
+            url = url + '?copy';
+
+            //sort = document.getElementById('sort').value;
+            //if (sort != '')
+            //    url = url + '&sort=' + sort
+
+            //search = document.getElementById('search').value;
+            //if (search != '')
+            //    url = url + '&search=' + search
+
+            //filter_key = document.getElementById('filter_key').value;
+            //if (filter_key != '')
+            //    url = url + '&filter_key=' + filter_key
+
+            $.ajax({
+                url: url,
+                dataType: 'text',
+                async: false,
+                processData: false,
+                contentType: false,
+                type: 'GET',
+                success: function(data) {
+                    navigator.clipboard.writeText(data);
+                }
+            });
         }
     </script>
 
     <form id="form" method="post">
         {% csrf_token %}
         <input type="hidden" id="action" name="action" value="{{action}}"/>
         <input type="hidden" name="path" value="{{path}}"/>
         <input type="hidden" name="back" value="{{back}}"/>
-        <input type="hidden" name="condition_group_id" value="{{condition_group_id}}"/>
+        <input type="hidden" name="edit" value="{{edit}}"/>
+        <input type="hidden" id="sort" name="sort" value="{{sort}}"/>
+        <input type="hidden" name="grid_id" value="{{grid.id}}"/>
 
         {% include "components/banners.html" %}
 
+        {% if not read_only %}
+
         <div class="panel panel-default">
             <div class="panel-body">
+                {% include "components/field_text_short.html" with field=form|field:'name' %}
 
                 <div class="form-group">
                     <div class="col-sm-4">
-                        <label>Champs</label>
+                        <label>Table</label>
                     </div>
                     <div class="col-sm-8">
-                        <select id="field_key" name="label" class="form-control" onchange="set_values();">
-                            {% for field in fields %}
-                            <option value="{{field.key}}" {% if field.key == condition.label %}selected{% endif %}>{{field.label}}</option>
+                        {% if grid %}
+                            {% for key, grid_table in tables.items %}
+                                {% if table == key %}
+                                <input name="table"
+                                       class="form-control"
+                                       type="text"
+                                       value="{{grid_table.label}}"
+                                       disabled/>
+                                {% endif %}
                             {% endfor %}
-                        </select>
-                    </div>
-                </div>
-
-                <div class="form-group">
-                    <div class="col-sm-4">
-                        <label>Critère</label>
-                    </div>
-                    <div class="col-sm-8">
-                        <select name="criteria" class="form-control">
-                            {% for key, value in criteria_set.items %}
-                            <option value="{{key}}" {% if criteria == key %}selected{% endif %}>{{value}}</option>
+                        {% else %}
+                        <select name="table" class="form-control">
+                            {% for key, grid_table in tables.items %}
+                            <option value="{{key}}" {% if table == key %}selected{% endif %}>{{grid_table.label}}</option>
                             {% endfor %}
                         </select>
+                        {% endif %}
                     </div>
                 </div>
 
-                {% include "components/field_text_short.html" with field=form|field:'value' %}
+                {% include "components/field_text_area_short.html" with field=form|field:'filter_by' %}
 
-                <div class="form-group">
-                    <div class="col-sm-4"></div>
-                    <div class="col-sm-8" id="values"></div>
-                </div>
+                {% include "components/field_text_short.html" with field=form|field:'comment' %}
+
+                {% include "components/field_check_short.html" with field=form|field:'group_by' %}
+                {% include "components/field_check_short.html" with field=form|field:'distinct' %}
+                {% include "components/field_check_short.html" with field=form|field:'show_on_home' %}
 
             </div>
             <div class="panel-footer">
                 <button type="button" class="btn btn-default" onclick="go_back('{{ back }}')">Annuler</button>
                 <button type="submit" class="btn btn-primary">Enregistrer</button>
-                {% if user.is_staff and condition %}
-                <button type="button" class="btn btn-danger" onclick="open2('{% url 'django:condition_delete' condition.id %}')">Supprimer</button>
+                {% if user.is_staff and grid %}
+                <button type="button" class="btn btn-danger" onclick="open2('{% url 'django:grid_delete' grid.id %}')">Supprimer</button>
                 {% endif %}
             </div>
         </div>
 
-    </form>
+        {% if action == 'update' %}
 
-    <script>
-        set_values_for("{{condition.label}}");
-    </script>
+        {% include "components/table.html" with table=table_columns no_paginate=True %}
+
+        {% endif %}
+
+        {% endif %}
+
+        {% if action == 'update' %}
+
+        {% if read_only %}
+            <div style="margin-top: 15px; margin-bottom: 10px; color: #2a437d;">{{grid.name}}</div>
+            {% if grid.comment %}
+            <div style="margin-bottom: 10px; color: #a0a0a0;">{{grid.comment}}</div>
+            {% endif %}
+        {% endif %}
+
+        {% include "components/grid.html" with columns=columns rows=rows fields=fields %}
+
+        {% endif %}
+
+    </form>
 
 {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,13 +1,25 @@
-{% extends base %} {% load form_extras %} {% block content %}
-{% csrf_token %}     {% include "components/banners.html" %}
-Champs
-{% for field in fields %}
-% if field.key == condition.label %}selected{% endif %}>{{field.label}}
+{% extends base %} {% load form_extras %} {% load custom %} {% block content %}
+{% csrf_token %}       {% include "components/banners.html" %} {% if not
+read_only %}
+{% include "components/field_text_short.html" with field=form|field:'name' %}
+Table
+{% for key, grid_table in tables.items %}
+% if table == key %}selected{% endif %}>{{grid_table.label}}
 {% endfor %}
-CritÃ¨re
-{% for key, value in criteria_set.items %}
-% if criteria == key %}selected{% endif %}>{{value}}
-{% endfor %}
-{% include "components/field_text_short.html" with field=form|field:'value' %}
-Annuler Enregistrer {% if user.is_staff and condition %} Supprimer {% endif %}
- {% endblock %}
+ {% endif %}
+{% include "components/field_text_area_short.html" with field=form|field:
+'filter_by' %} {% include "components/field_text_short.html" with
+field=form|field:'comment' %} {% include "components/field_check_short.html"
+with field=form|field:'group_by' %} {% include "components/
+field_check_short.html" with field=form|field:'distinct' %} {% include
+"components/field_check_short.html" with field=form|field:'show_on_home' %}
+Annuler Enregistrer {% if user.is_staff and grid %} Supprimer {% endif %}
+{% if action == 'update' %} {% include "components/table.html" with
+table=table_columns no_paginate=True %} {% endif %} {% endif %} {% if action ==
+'update' %} {% if read_only %}
+{{grid.name}}
+{% if grid.comment %}
+{{grid.comment}}
+{% endif %} {% endif %} {% include "components/grid.html" with columns=columns
+rows=rows fields=fields %} {% endif %}
+{% endblock %}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/log.html` & `foledol-django-0.0.9/src/foledol/django/templates/log.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <input type="hidden" name="log_id" value="{{log.id}}"/>
     {% include "components/navigator_inputs.html" %}
 
     <div class="panel panel-default">
         <div class="panel-body">
             <div class="form-group">
                 <div class="col-sm-4"><label>Date</label></div>
-                <div class="col-sm-8"><input class="form-control" type="text" name="date" value="{{ log.date|short_datetime }}" disabled/></div>
+                <div class="col-sm-8"><input class="form-control" type="text" name="date" value="{{ log.date|date:'d/m/Y H:i' }}" disabled/></div>
             </div>
             <div class="form-group">
                 <div class="col-sm-4"><label>Table</label></div>
                 <div class="col-sm-8"><input class="form-control" type="text" name="model" value="{{ log.model }}" disabled/></div>
             </div>
             <div class="form-group">
                 <div class="col-sm-4"><label>Ref</label></div>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends base %} {% load date_extras %} {% load staticfiles %} {% block
 navigation %} {% include "components/navigator.html" with space='django:
 log_update' %} {% endblock %} {% block content %}
 {% csrf_token %}     {% include "components/navigator_inputs.html" %}
 Date
-[{{ log.date|short_datetime }}]
+[{{ log.date|date:'d/m/Y H:i' }}]
 Table
 [{{ log.model }}     ]
 Ref
 [{{ log.ref }}       ]
 Utilisateur
 [{{ log.author }}    ]
 Action
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templates/user_login.html` & `foledol-django-0.0.9/src/foledol/django/templates/user_login.html`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templatetags/custom.py` & `foledol-django-0.0.9/src/foledol/django/templatetags/custom.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/templatetags/date_extras.py` & `foledol-django-0.0.9/src/foledol/django/templatetags/date_extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 @register.filter
 def long_datetime(value):
     return get_long_datetime(value)
 
 
 @register.filter
 def short_datetime(value):
-    return value.astimezone(tz).strftime('%d/%m/%Y %H:%M')
+    return value.astimezone(tz).strftime('%d/%m/%Y à %H:%M')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foledol-django-0.0.81/src/foledol/django/templatetags/form_extras.py` & `foledol-django-0.0.9/src/foledol/django/templatetags/form_extras.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,53 +26,24 @@
         return None
 
 
 @register.filter
 def value(obj, name):
     split = name.split('.', 1)
     if len(split) > 1:
-        return value(getattr(obj, split[0]), split[1]) if (obj and hasattr(obj, split[0])) else None
-    return getattr(obj, name) if (obj and hasattr(obj, name)) else None
-
-
-@register.filter
-def value_as_str(obj, name):
-    split = name.split('.', 1)
-    if len(split) > 1:
-        return value(getattr(obj, split[0]), split[1]) if (obj and hasattr(obj, split[0])) else None
-    as_str = value(obj, name + '_as_str')
-    return as_str() if as_str else value(obj, name)
+        return value(getattr(obj, split[0]), split[1])
+    return getattr(obj, name) if obj else None
 
 
 @register.filter
 def method(obj, name):
     split = name.split('.', 1)
     if len(split) > 1:
-        return method(getattr(obj, split[0]), split[1]) if (obj and hasattr(obj, split[0])) else None
-    return getattr(obj, name)() if (obj and hasattr(obj, name)) else None
-
-
-@register.filter
-def has_attr(obj, attr):
-    return hasattr(obj, attr)
-
-
-@register.filter
-def visible(obj, row):
-    return getattr(obj, 'visible')(row) if (hasattr(obj, 'visible') and getattr(obj, 'visible')) else True
-
-
-@register.filter
-def enabled(obj, row):
-    return getattr(obj, 'enabled')(row) if (hasattr(obj, 'enabled') and getattr(obj, 'enabled')) else True
-
-
-@register.filter
-def on_click(obj, row):
-    return getattr(obj, 'on_click')(row) if (hasattr(obj, 'on_click') and getattr(obj, 'on_click')) else None
+        return method(getattr(obj, split[0]), split[1])
+    return getattr(obj, name)() if obj else None
 
 
 @register.filter
 def formatter(table, row):
     return table.formatter(row)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/test.py` & `foledol-django-0.0.9/src/foledol/django/test.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/barcode.py` & `foledol-django-0.0.9/src/foledol/django/tools/barcode.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from django.conf import settings
 
 from ..utils import remove_file
 
 
 class BarCode:
 
-    def __init__(self, uid, name, value, folder):
-        path = os.path.join(settings.MEDIA_ROOT, folder, uid.replace('/', '-'))
+    def __init__(self, uid, value):
+        path = os.path.join(settings.STATIC_FILES, 'bc39', uid.replace('/', '-'))
         self.path_bc = path + '.png'
         remove_file(self.path_bc)
 
-        bc39 = barcode.get(name, value, writer=ImageWriter(), options={'add_checksum': False})
+        bc39 = barcode.get('code39', value, writer=ImageWriter(), options={'add_checksum': False})
         bc39.save(path, {"module_width": 0.3})
 
         bc39 = Image.open(self.path_bc)
         w, h = bc39.size
         bc39 = bc39.crop((0, 0, w, h - 110))
         bc39_rotated = bc39.rotate(-90, expand=True)
         self.path_bc_rotated = path + "_rotated.png"
@@ -27,9 +27,8 @@
 
     def remove(self):
         remove_file(self.path_bc)
         remove_file(self.path_bc_rotated)
 
 
 def create_bc39(uid, value):
-    return BarCode(uid, 'code39', value, 'bc39') if uid and value else None
-
+    return BarCode(uid, value) if uid and value else None
```

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/canvas.py` & `foledol-django-0.0.9/src/foledol/django/tools/canvas.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/chart.py` & `foledol-django-0.0.9/src/foledol/django/tools/chart.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/field.py` & `foledol-django-0.0.9/src/foledol/django/tools/field.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,14 @@
         self.errors = []
         self.key = key
         self.label = label
         self.disabled = disabled
         self.errors = []
         self.value_as_str = ''
         self.external = False
-        self.form = None
-
-    def attach(self, form):
-        self.form = form
-
-    def namespace(self):
-        return self.form.namespace if self.form else None
-
-    def full_name(self):
-        namespace = self.namespace()
-        return namespace + "_" + self.key if namespace else self.key
 
     def set(self, value):
         pass
 
     def read(self, context, default):
         pass
 
@@ -59,16 +48,15 @@
         self.autocomplete_url = autocomplete_url
 
     def set(self, value):
         self.value = value if value is not None else None
         self.value_as_str = value if value is not None else ''
 
     def read(self, context, default):
-        key = self.full_name()
-        self.set(context[key] if key in context else default)
+        self.set(context[self.key] if self.key in context else default)
 
     def validate(self):
         self.errors = []
         length = len(str(self.value)) if self.value else 0
         if self.value is None and not self.blank:
             self.errors.append("Le champ est obligatoire")
         elif self.min_length and length < self.min_length:
@@ -90,23 +78,15 @@
         self.value = None
 
     def set(self, value):
         self.value = None if value is None else value
         self.value_as_str = str(self.value)
 
     def read(self, context, default):
-        key = self.full_name()
-        self.set(context[key] if key in context else default)
-
-    def get_value(self, value):
-        if self.pairs:
-            keys = [k for k, v in self.pairs.items() if re.search(v, value, re.IGNORECASE)]
-            if len(keys) == 1:
-                return keys[0]
-        return value
+        self.set(context[self.key] if self.key in context else default)
 
 
 class IntegerField(Field):
     def __init__(self, key, label, min_value=None, max_value=None, blank=True, disabled=False):
         super().__init__(key, label, disabled=disabled)
         self.min_value = min_value
         self.max_value = max_value
@@ -114,21 +94,20 @@
         self.value = None
 
     def set(self, value):
         self.value = value if value != '' else None
         self.value_as_str = '' if value is None else str(value)
 
     def read(self, context, default):
-        key = self.full_name()
-        if key in context:
+        if self.key in context:
             try:
-                self.value = int(context[key])
+                self.value = int(context[self.key])
             except ValueError:
                 self.value = None
-            self.value_as_str = str(context[key])
+            self.value_as_str = str(context[self.key])
         else:
             self.set(default)
 
     def validate(self):
         self.errors = []
         if len(self.value_as_str) < 1 and not self.blank:
             self.errors.append("Le champ est obligatoire")
@@ -150,18 +129,17 @@
         self.value = None
 
     def set(self, value):
         self.value = value
         self.value_as_str = '' if value is None else str(value).replace('.', ',')
 
     def read(self, context, default):
-        key = self.full_name()
-        if key in context:
-            self.value = to_float(context[key])
-            self.value_as_str = str(context[key])
+        if self.key in context:
+            self.value = to_float(context[self.key])
+            self.value_as_str = str(context[self.key])
         else:
             self.set(default)
 
     def validate(self):
         self.errors = []
         if len(self.value_as_str) < 1 and not self.blank:
             self.errors.append("Le champ est obligatoire")
@@ -182,21 +160,20 @@
         self.format = format
 
     def set(self, value):
         self.value = value
         self.value_as_str = value.strftime(self.format) if value else ''
 
     def read(self, context, default):
-        key = self.full_name()
-        if key in context:
+        if self.key in context:
             try:
-                self.value = datetime.strptime(context[key], self.format)
+                self.value = datetime.strptime(context[self.key], self.format)
             except ValueError:
                 self.value = None
-            self.value_as_str = str(context[key])
+            self.value_as_str = str(context[self.key])
         else:
             self.set(default)
 
     def validate(self):
         self.errors = []
         if len(self.value_as_str) < 1 and not self.blank:
             self.errors.append("Le champ est obligatoire")
@@ -214,10 +191,9 @@
         if isinstance(value, str):
             self.value = value == 'on'
         else:
             self.value = value
         self.value_as_str = str(value)
 
     def read(self, context, default):
-        key = self.full_name()
         default_value = default if default is not None else False
-        self.set(key in context if len(context) > 0 else default_value)
+        self.set(True if self.key in context else default_value)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/form.py` & `foledol-django-0.0.9/src/foledol/django/tools/form.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from foledol.django.logger import log
 
 
 class Form:
     def __init__(self, context, fields, namespace=None):
         self.context = context
         self.fields = fields
-        for field in fields:
-            field.attach(self)
         self.namespace = namespace
         self.old_values = None
         self.new_values = None
 
     def field(self, key):
         try:
             return next(field for field in self.fields if field.key == key)
         except StopIteration:
             raise Exception("Invalid field '" + key + "'")
 
     def read(self, values, sibling=None, defaults=None):
         self.old_values = {}
         for field in self.fields:
-            self.context[field.full_name] = field.value
             default_value = None
             if defaults and field.key in defaults:
                 default_value = defaults[field.key]
             elif sibling and field.key in sibling.__dict__:
                 default_value = sibling.__dict__[field.key]
             self.old_values[field.key] = default_value
+            self.context[field.key] = field.value #if field.value else default_value
             # TODO: move this before the self.context
             field.read(values, default_value)
         self.context['form'] = self
 
     def validate(self):
         self.context['error'] = False
         for field in self.fields:
             field.validate()
-            self.context[field.full_name] = field.value
+            self.context[field.key] = field.value
             self.context['errors_on_' + field.key] = None
             if len(field.errors) > 0:
                 self.context['errors_on_' + field.key] = field.errors
             self.context['error'] |= field.has_error()
 
     def save(self, sibling):
         self.new_values = {}
```

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/handlers.py` & `foledol-django-0.0.9/src/foledol/django/tools/handlers.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/readers.py` & `foledol-django-0.0.9/src/foledol/django/tools/readers.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/report.py` & `foledol-django-0.0.9/src/foledol/django/tools/report.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/tools/writer.py` & `foledol-django-0.0.9/src/foledol/django/tools/writer.py`

 * *Files identical despite different names*

### Comparing `foledol-django-0.0.81/src/foledol/django/utils.py` & `foledol-django-0.0.9/src/foledol/django/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # -*- coding: utf-8 -*-
 import io
 import os
-import pathlib
 import re
 import shutil
 import smtplib
 import sys
-import uuid
 from datetime import datetime
-from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 
 import pytz
 from PIL import Image
 from django.conf import settings
-from django.core.files.storage import FileSystemStorage
-from django.core.paginator import Paginator, EmptyPage
+from django.core.paginator import Paginator
 from django.http import HttpResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.translation import LANGUAGE_SESSION_KEY
 
 
 DAYS = [
@@ -111,14 +107,21 @@
 
 def get_param2(request, label, value):
     if label in request.GET:
         return request.GET[label]
     return get_param(request, label, value)
 
 
+def get_filtered_items(request, context, space, items, filters):
+    filter_key = get_param_from_request(request, context, space, 'filter_key', '')
+    if filter_key and filter_key in filters:
+        items = filters[filter_key].filter(items)
+    return items
+
+
 def get_param_from_request(request, context, space, label, value):
     full_name = space + "." + label
     if label in request.POST:
         context[label] = request.POST[label]
     else:
         context[label] = request.session[full_name] if full_name in request.session else value
     request.session[full_name] = context[label]
@@ -181,37 +184,28 @@
 
 #
 # Navigation
 #
 
 
 can_navigate_params = ['sort', 'search']
-can_navigate_params_from_grid = [
-    'grid_id',
-    'grid_sort'
-]
 
 
 def can_navigate(request, context, back):
-    #if context and 'back' in context and context['back'] != back:
-    #    return False
-    def has_params(params):
-        for param in params:
-            if param not in request.POST:
-                return False
-        return True
-
-    return has_params(can_navigate_params) or has_params(can_navigate_params_from_grid)
+    if context and 'back' in context and context['back'] != back:
+        return False
+    for param in can_navigate_params:
+        if param not in request.POST:
+            return False
+    return True
 
 
 def navigate(request, context, items, id):
     for param in can_navigate_params:
         get_param(request, context, param, '')
-    for param in can_navigate_params_from_grid:
-        get_param(request, context, param, '')
 
     if items.first():
 
         paginator_size = None
         if 'paginator_size' in request.POST and request.POST['paginator_size']:
             context['paginator_size'] = request.POST['paginator_size']
             paginator_size = int(context['paginator_size'])
@@ -222,18 +216,15 @@
             paginator_page = int(context['paginator_page'])
 
         index = 0
         if paginator_page and paginator_size:
             size = (paginator_size * 3)
             index = ((paginator_page - 1) * paginator_size)
             page = int(index / size) + 1
-            try:
-                items = Paginator(items, size).page(page)
-            except EmptyPage:
-                page = 0
+            items = Paginator(items, size).page(page)
             index_prev = index
             index_next = index + paginator_size - 1
             index = ((page - 1) * size)
 
         item_index = -1
         prev_item = next_item = None
         for item in items:
@@ -267,20 +258,14 @@
     page = 1
     if 'paginator_page' in request.POST and request.POST['paginator_page']:
         page = int(request.POST['paginator_page'])
     elif space:
         full_name = space + '.page'
         page = request.session[full_name] if full_name in request.session else 1
 
-    if isinstance(page, str):
-        try:
-            page = int(page)
-        except ValueError:
-            page = 0
-
     size = length
     if 'paginator_size' in request.POST and request.POST['paginator_size']:
         size = int(request.POST['paginator_size'])
     elif paginate:
         full_name = 'paginator_size'
         size = request.session[full_name] if full_name in request.session else length
     elif space:
@@ -312,56 +297,25 @@
 
 def clean_html(raw_html):
     cleanr = re.compile('<.*?>')
     cleantext = re.sub(cleanr, '', raw_html)
     return cleantext
 
 
-class MailAttachment:
-    def __init__(self, name, path):
-        self.name = name
-        self.path = path
-
-    def get_buffer(self):
-        return open(self.path, 'rb').read()
-
-
-class MailAttachmentFromBuffer:
-    def __init__(self, name, buffer):
-        self.name = name
-        self.buffer = buffer
-
-    def get_buffer(self):
-        return self.buffer
-
-
-def send_mail2(to, subject, body, host=None, port=None, username=None, password=None, sender=None, attachments=None):
-    sender = sender if sender else settings.MAIL_USERNAME
-    username = username if username else settings.MAIL_USERNAME
-    password = password if password else settings.MAIL_PASSWORD
-
+def send_mail2(to, subject, body):
     msg = MIMEMultipart()
-    msg['From'] = sender
+    msg['From'] = settings.MAIL_USERNAME
     msg['To'] = to
     msg['Subject'] = subject
     msg.attach(MIMEText(body, 'html'))
 
-    if attachments:
-        for attachment in attachments:
-            part = MIMEApplication(
-                attachment.get_buffer(),
-                Name=attachment.name
-            )
-            part['Content-Disposition'] = 'attachment; filename="%s"' % attachment.name
-            msg.attach(part)
-
-    server = smtplib.SMTP(host if host else 'smtp.gmail.com', port if port else 587)
+    server = smtplib.SMTP('smtp.gmail.com', 587)
     server.starttls()
-    server.login(username, password)
-    server.sendmail(sender, to, msg.as_string())
+    server.login(settings.MAIL_USERNAME, settings.MAIL_PASSWORD)
+    server.sendmail(settings.MAIL_USERNAME, to, msg.as_string())
     server.quit()
 
 
 def print_report(pdf, filename):
     response = HttpResponse(pdf, content_type='application/pdf')
     response['Content-Disposition'] = 'attachment; filename="' + filename + '"'
     return response
@@ -418,22 +372,19 @@
     context['back'] = path.split(':')[-1]
     context['path'] = path
     return action
 
 
 def get_path(request, context, obj, prefix, space=settings.DEFAULT_SPACE):
     path = get_path_from_request(request)
-
-    if 'back' in request.GET and 'path' in request.session:
-        path = request.session['path']
-        request.session.pop('path')
-        path = path.rsplit(':', 1)[0]
-
     action = get_action(request)
-    if action in ['back', 'open_item']:
+    if action == 'open_item':
+        path = path.rsplit(':', 1)[0]
+        action = ''
+    if action == 'back':
         path = path.rsplit(':', 1)[0]
         action = ''
     else:
         if obj:
             item = reverse(space + ':' + prefix + "_update", kwargs={'pk': obj.id})
         else:
             item = reverse(space + ':' + prefix + "_create")
@@ -532,26 +483,7 @@
         with open(path, mode='w') as file:
             output.seek(0)
             file.write(output.getvalue())
         return
     with open(path, mode='wb') as file:
         output.seek(0)
         shutil.copyfileobj(output, file, length=4096)
-
-
-def upload(request, context, loader):
-    file = request.FILES['upload']
-
-    extension = pathlib.Path(file.name).suffix
-
-    uid = uuid.uuid4().hex
-    path = os.path.join(settings.MEDIA_ROOT, 'temp', uid + extension)
-    fs = FileSystemStorage()
-    fs.save(path, file)
-
-    try:
-        loader(path)
-        log_success("Le fichier a été chargé avec succès.", context)
-    except Exception as ex:
-        log_error(str(ex), context)
-    finally:
-        remove_file(path)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/views/column.py` & `foledol-django-0.0.9/src/foledol/django/views/column.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,99 @@
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseRedirect, HttpResponseForbidden
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.translation import gettext as _
-
 from foledol.django.logger import log
-from foledol.django.tools.field import TextField, IntegerField
+from foledol.django.tools.field import TextField, IntegerField, BooleanField, DateField, FloatField
 from foledol.django.tools.form import Form
 from foledol.django.tools.handlers import confirm
-from foledol.django.utils import pop_path, get_path, get_integer, error, new_context
+from foledol.django.utils import pop_path, get_path, get_param, get_integer, error, new_context
+from .grid import get_field
 from .grids import grid_renumber
-from ..models import Column, Grid
+
+from ..models import Column, Grid, COLUMN_CRITERIA_SET, COLUMN_TEXT_CRITERIA_SET, COLUMN_DATE_CRITERIA_SET, \
+    COLUMN_NUMBER_CRITERIA_SET, COLUMN_BOOLEAN_CRITERIA_SET
 
 
 class ColumnForm(Form):
     def __init__(self, context):
         super().__init__(context, [
             TextField('label', "Libellé", min_length=1),
-            IntegerField('order_by', "Tri"),
+            IntegerField('criteria', "Critère"),
+            TextField('value', "Valeur"),
             IntegerField('order', "Ordre"),
             IntegerField('width', "Largeur"),
+            BooleanField('hidden', "Masquer"),
         ])
 
 
 def column_form(request, column):
     if not request.user.is_staff:
         return HttpResponseForbidden()
 
     context = new_context()
     context['base'] = settings.DEFAULT_SPACE + '/base.html'
 
     action = get_path(request, context, column, 'column', space='django')
 
-    grid = None
-
     grid_id = get_integer(request, 'grid_id', 0)
     if grid_id > 0:
         grid = Grid.objects.all().get(id=grid_id)
-    context['grid_id'] = grid.id if grid else 0
-
-    order_by = get_integer(request, 'order_by', column.order_by if column else 0)
+    context['grid_id'] = grid.id
 
     if column:
         context['column'] = column
 
     fields = grid.fields() if grid else []
     context['fields'] = fields
 
-    form = ColumnForm(context)
-    form.read(request.POST if action else {}, column, defaults={
-        'order_by': 0
-    })
+    context['criteria_set'] = COLUMN_CRITERIA_SET
 
-    context['order_by'] = order_by
+    form = ColumnForm(context)
+    form.read(request.POST, column)
+    if action == 'update':
+        # TODO: fix the issue on BooleanField (Read)
+        form.field('hidden').value = 'hidden' in request.POST
 
     order = (grid.column_set.count() + 1) * 10 if grid else 10
 
+    criteria = get_integer(request, 'criteria', column.criteria if column else 0)
+    context['criteria'] = criteria
+
     if len(action) > 0:
         form.validate()
 
     if context['error']:
         context['error'] = "Veuillez corriger les erreurs ci-dessous"
 
+    label = get_param(request, context, 'label', None)
+    if label and column:
+        field = get_field(column.label, fields)
+        if isinstance(field, TextField):
+            if criteria not in COLUMN_TEXT_CRITERIA_SET:
+                context['error'] = "Le critère n'est pas compatible avec un texte"
+        if isinstance(field, DateField):
+            if criteria not in COLUMN_DATE_CRITERIA_SET:
+                context['error'] = "Le critère n'est pas compatible avec une date"
+        if isinstance(field, FloatField) or isinstance(field, IntegerField):
+            if criteria not in COLUMN_NUMBER_CRITERIA_SET:
+                context['error'] = "Le critère n'est pas compatible avec un nombre"
+        if isinstance(field, BooleanField):
+            if criteria not in COLUMN_BOOLEAN_CRITERIA_SET:
+                context['error'] = "Le critère n'est pas compatible avec un booléen"
+
     if not action or context['error']:
         context['action'] = 'update' if column else 'create'
         return render(request, 'column.html', context)
 
     if action == 'create':
         column = Column(grid=grid)
     form.save(column)
-    column.order_by = order_by
     if not column.order:
         column.order = order
     column.save()
     if grid:
         grid_renumber(grid)
     log(column.id, 'column', action, request.user, form.old_values, form.new_values)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/views/conditions.py` & `foledol-django-0.0.9/src/foledol/django/views/columns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,37 @@
+from django.conf import settings
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
-from foledol.django.tools.table import TableColumn, TableView
+from django.shortcuts import render
+from foledol.django.tools.table import Table, TableColumn
+from foledol.django.utils import get_search, paginate, new_context
 
-from ..models import Condition
+from ..models import Column
 
 
-class ConditionTables(TableView):
-    def __init__(self):
-        super().__init__(Condition, [
+class ColumnTables(Table):
+    def __init__(self, rows):
+        super().__init__(rows, [
             TableColumn('label', "Libellé"),
             TableColumn('criteria', "Critère"),
             TableColumn('value', "Valeur")
-        ], path='django:conditions', search=True)
-        self.update = 'django:condition_update'
-        self.create = 'django:condition_create'
-
-    def select(self, conditions, search, order_by):
-        return conditions.filter(label=search) if len(search) > 0 else conditions
+        ])
+        self.update = 'django:column_update'
+        self.create = 'django:column_create'
+        self.search = True
 
 
 @login_required
 @staff_member_required
-def condition_list(request):
-    return ConditionTables().render(request)
+def column_list(request):
+    context = new_context()
+    context['base'] = settings.DEFAULT_SPACE + '/base.html'
+
+    columns = Column.objects.all()
+
+    search = get_search(request).strip()
+    if len(search) > 0:
+        columns = Column.objects.filter(label=search)
+    context['search'] = search
+    context['table'] = ColumnTables(paginate(request, context, columns))
+
+    return render(request, 'columns.html', context)
```

### Comparing `foledol-django-0.0.81/src/foledol/django/views/logs.py` & `foledol-django-0.0.9/src/foledol/django/views/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 import datetime
 import os
 
 import matplotlib.pyplot as plt
 from django.conf import settings
-from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
 from django.db.models import Q
 from django.http import HttpResponseForbidden, FileResponse
 from django.shortcuts import render
 from django.urls import reverse
 
-from foledol.django.tools.table import TableColumn, TableButton, TableView
-from foledol.django.utils import new_context, can_navigate, navigate, get_path
+from foledol.django.tools.table import Table, TableColumn, TableButton
+from foledol.django.utils import get_param, paginate, get_param_from_request, new_context, can_navigate, navigate, \
+    get_path
 from foledol.django.utils import remove_file, get_color, get_local_date
 from ..models import Log
 
 
-class LogTable(TableView):
-    def __init__(self):
-        super().__init__(Log, [
-            TableColumn('date', "Date", sortable=True, method='date_as_str'),
+class LogTable(Table):
+    def __init__(self, rows):
+        super().__init__(rows, [
+            TableColumn('date', "Date", sortable=True),
             TableColumn('user', "Utilisateur"),
             TableColumn('model', "Table"),
             TableColumn('action', "Action")
-        ], path='django:logs', search=True, sort='date_desc')
+        ])
         self.update = 'django:log_update'
         self.buttons = [
-            TableButton("Calculer", "send('compute')")
+            TableButton("Calculer", "send('compute')"),
         ]
+        self.search = True
 
-    def select(self, logs, search, order_by):
-        if len(search) > 0:
-            logs = logs.filter(
-                Q(user__email__icontains=search) |
-                Q(user__username__icontains=search) |
-                Q(user__last_name__icontains=search) |
-                Q(user__first_name__icontains=search) |
-                Q(model__icontains=search) |
-                Q(action__icontains=search)
-            )
-        return logs.order_by('date' if order_by == 'date_asc' else '-date')
+
+def get_logs(request, context):
+    logs = Log.objects.all()
+
+    search = get_param_from_request(request, context, 'logs', 'search', '').strip()
+    if len(search) > 0:
+        logs = logs.filter(
+            Q(user__email__icontains=search) |
+            Q(user__username__icontains=search) |
+            Q(user__last_name__icontains=search) |
+            Q(user__first_name__icontains=search) |
+            Q(model__icontains=search) |
+            Q(action__icontains=search)
+        )
+    context['search'] = search
+
+    sort = get_param(request, context, 'sort', 'date_desc')
+    return logs.order_by('date' if sort == 'date_asc' else '-date')
 
 
 @login_required
-@staff_member_required
 def log_list(request):
-    return LogTable().render(request)
+    if not request.user.is_staff:
+        return HttpResponseForbidden()
+    context = new_context()
+    context['base'] = settings.DEFAULT_SPACE + '/base.html'
+
+    logs = get_logs(request, context)
+
+    context['table'] = LogTable(paginate(request, context, logs, space='logs'))
+
+    return render(request, 'logs.html', context)
 
 
 @login_required
 def log_events(request):
     if not request.user.is_staff:
         return HttpResponseForbidden()
     context = new_context()
```

### Comparing `foledol-django-0.0.81/src/foledol_django.egg-info/SOURCES.txt` & `foledol-django-0.0.9/src/foledol_django.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,57 +12,48 @@
 src/foledol/django/meta.py
 src/foledol/django/models.py
 src/foledol/django/test.py
 src/foledol/django/urls.py
 src/foledol/django/utils.py
 src/foledol/django/migrations/0001_initial.py
 src/foledol/django/migrations/0002_auto_20220211_0730.py
-src/foledol/django/migrations/0003_auto_20220212_1614.py
-src/foledol/django/migrations/0004_auto_20220212_1620.py
-src/foledol/django/migrations/0005_grid_filter.py
-src/foledol/django/migrations/0006_auto_20220610_0534.py
-src/foledol/django/migrations/0007_auto_20220610_0642.py
-src/foledol/django/migrations/0008_auto_20230210_1029.py
-src/foledol/django/migrations/0009_auto_20230210_1430.py
-src/foledol/django/migrations/0010_auto_20230210_1447.py
-src/foledol/django/migrations/0011_auto_20230211_1150.py
 src/foledol/django/migrations/__init__.py
 src/foledol/django/reports/__init__.py
 src/foledol/django/reports/grid.py
-src/foledol/django/static/foledol-django.js
 src/foledol/django/templates/.DS_Store
 src/foledol/django/templates/column.html
-src/foledol/django/templates/condition.html
+src/foledol/django/templates/columns.html
 src/foledol/django/templates/grid.html
+src/foledol/django/templates/grids.html
 src/foledol/django/templates/log.html
 src/foledol/django/templates/log_events.html
-src/foledol/django/templates/table_view.html
+src/foledol/django/templates/logs.html
 src/foledol/django/templates/user_login.html
 src/foledol/django/templates/user_logout.html
 src/foledol/django/templates/common/archive.html
 src/foledol/django/templates/common/delete.html
 src/foledol/django/templates/common/error.html
 src/foledol/django/templates/common/print.html
 src/foledol/django/templates/components/banners.html
 src/foledol/django/templates/components/field_check.html
+src/foledol/django/templates/components/field_check_new.html
 src/foledol/django/templates/components/field_check_short.html
 src/foledol/django/templates/components/field_city.html
 src/foledol/django/templates/components/field_country.html
 src/foledol/django/templates/components/field_date.html
 src/foledol/django/templates/components/field_date_short.html
 src/foledol/django/templates/components/field_select.html
 src/foledol/django/templates/components/field_select_short.html
 src/foledol/django/templates/components/field_text.html
 src/foledol/django/templates/components/field_text_area.html
 src/foledol/django/templates/components/field_text_area_short.html
 src/foledol/django/templates/components/field_text_short.html
 src/foledol/django/templates/components/field_zip.html
 src/foledol/django/templates/components/grid.html
 src/foledol/django/templates/components/grid_column.html
-src/foledol/django/templates/components/grid_condition_group.html
 src/foledol/django/templates/components/grid_row.html
 src/foledol/django/templates/components/list.html
 src/foledol/django/templates/components/logs.html
 src/foledol/django/templates/components/meta.html
 src/foledol/django/templates/components/navigator.html
 src/foledol/django/templates/components/navigator_inputs.html
 src/foledol/django/templates/components/paginator.html
@@ -86,16 +77,14 @@
 src/foledol/django/tools/readers.py
 src/foledol/django/tools/report.py
 src/foledol/django/tools/table.py
 src/foledol/django/tools/writer.py
 src/foledol/django/views/__init__.py
 src/foledol/django/views/column.py
 src/foledol/django/views/columns.py
-src/foledol/django/views/condition.py
-src/foledol/django/views/conditions.py
 src/foledol/django/views/grid.py
 src/foledol/django/views/grids.py
 src/foledol/django/views/logs.py
 src/foledol_django.egg-info/PKG-INFO
 src/foledol_django.egg-info/SOURCES.txt
 src/foledol_django.egg-info/dependency_links.txt
 src/foledol_django.egg-info/top_level.txt
```

