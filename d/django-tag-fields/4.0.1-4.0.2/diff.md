# Comparing `tmp/django-tag-fields-4.0.1.tar.gz` & `tmp/django-tag-fields-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tag-fields-4.0.1.tar", last modified: Thu May  4 08:41:56 2023, max compression
+gzip compressed data, was "django-tag-fields-4.0.2.tar", last modified: Sat May  6 09:16:09 2023, max compression
```

## Comparing `django-tag-fields-4.0.1.tar` & `django-tag-fields-4.0.2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
--rw-r--r--   0        0        0      235 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.coveragerc
--rw-r--r--   0        0        0     1983 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/.git-commit-template.txt
--rw-r--r--   0        0        0      907 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      136 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/chore.md
--rw-r--r--   0        0        0      424 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/documentation-request.md
--rw-r--r--   0        0        0      619 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      841 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/semantic.yaml
--rw-r--r--   0        0        0      923 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1503 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1198 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.gitignore
--rw-r--r--   0        0        0     1389 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      751 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/AUTHORS
--rw-r--r--   0        0        0    13599 2023-05-04 08:41:51.398888 django-tag-fields-4.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0     5488 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5244 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1574 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/LICENSE
--rw-r--r--   0        0        0      205 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/MANIFEST.in
--rw-r--r--   0        0        0     2739 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/README.rst
--rw-r--r--   0        0        0      853 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/codecov.yml
--rw-r--r--   0        0        0     1525 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/admin.rst
--rw-r--r--   0        0        0     4396 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/api.rst
--rw-r--r--   0        0        0       30 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/changelog.rst
--rw-r--r--   0        0        0      471 2023-05-04 08:41:51.410888 django-tag-fields-4.0.1/docs/conf.py
--rw-r--r--   0        0        0       33 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/contributing.rst
--rw-r--r--   0        0        0     8972 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/custom_tagging.rst
--rw-r--r--   0        0        0     2251 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/external_apps.rst
--rw-r--r--   0        0        0     1040 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/faq.rst
--rw-r--r--   0        0        0     2378 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/forms.rst
--rw-r--r--   0        0        0     1903 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/getting_started.rst
--rw-r--r--   0        0        0      705 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/index.rst
--rw-r--r--   0        0        0      983 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/docs/serializers.rst
--rw-r--r--   0        0        0     1855 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/requirements/docs.txt
--rw-r--r--   0        0        0       36 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/requirements/test.txt
--rw-r--r--   0        0        0       38 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/setup.py
--rw-r--r--   0        0        0      259 2023-05-04 08:41:51.410888 django-tag-fields-4.0.1/tag_fields/__init__.py
--rw-r--r--   0        0        0      382 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/admin.py
--rw-r--r--   0        0        0      253 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/apps.py
--rw-r--r--   0        0        0     1442 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/forms.py
--rw-r--r--   0        0        0     1299 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2206 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1042 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2005 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1033 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1941 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1068 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1839 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      991 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2188 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1738 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1131 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1873 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1058 2023-05-04 08:41:50.534880 django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2021 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1203 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2162 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1047 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1928 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1105 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2073 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      828 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1955 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      945 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1904 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1142 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1908 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      993 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1947 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      933 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1739 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1045 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1897 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1870 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2544 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1051 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2014 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1211 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2144 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      992 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1982 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26666 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/managers.py
--rw-r--r--   0        0        0     2694 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0001_initial.py
--rw-r--r--   0        0        0      280 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0002_auto_20150616_2121.py
--rw-r--r--   0        0        0      374 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0003_taggeditem_add_unique_index.py
--rw-r--r--   0        0        0     1232 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
--rw-r--r--   0        0        0      502 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/0005_auto_20220424_2025.py
--rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/migrations/__init__.py
--rw-r--r--   0        0        0     7780 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/models.py
--rw-r--r--   0        0        0     4386 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/serializers.py
--rw-r--r--   0        0        0     4295 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/utils.py
--rw-r--r--   0        0        0     1583 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tag_fields/views.py
--rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/__init__.py
--rw-r--r--   0        0        0       89 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/admin.py
--rw-r--r--   0        0        0      168 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/custom_parser.py
--rw-r--r--   0        0        0      834 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/forms.py
--rw-r--r--   0        0        0    39683 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0     3529 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0002_auto_20200214_1129.py
--rw-r--r--   0        0        0     3015 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0003_auto_20210310_0918.py
--rw-r--r--   0        0        0     4440 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0004_auto_20210619_0826.py
--rw-r--r--   0        0        0     1025 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/0005_auto_20210713_2301.py
--rw-r--r--   0        0        0        0 2023-05-04 08:41:50.538880 django-tag-fields-4.0.1/tests/migrations/__init__.py
--rw-r--r--   0        0        0    10311 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/models.py
--rw-r--r--   0        0        0      329 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/serializers.py
--rw-r--r--   0        0        0     1333 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/settings.py
--rw-r--r--   0        0        0      124 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/templates/tests/food_tag_list.html
--rw-r--r--   0        0        0     1394 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_admin.py
--rw-r--r--   0        0        0     1849 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_forms.py
--rw-r--r--   0        0        0     2339 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_models.py
--rw-r--r--   0        0        0     3366 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_serializers.py
--rw-r--r--   0        0        0      984 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/test_utils.py
--rw-r--r--   0        0        0    54037 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/tests.py
--rw-r--r--   0        0        0      294 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/urls.py
--rw-r--r--   0        0        0      182 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tests/views.py
--rw-r--r--   0        0        0     1174 2023-05-04 08:41:50.542880 django-tag-fields-4.0.1/tox.ini
--rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 django-tag-fields-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      235 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.coveragerc
+-rw-r--r--   0        0        0     1983 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/.git-commit-template.txt
+-rw-r--r--   0        0        0      907 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      136 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/chore.md
+-rw-r--r--   0        0        0      424 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/documentation-request.md
+-rw-r--r--   0        0        0      619 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      841 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/semantic.yaml
+-rw-r--r--   0        0        0      923 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1503 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1198 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.gitignore
+-rw-r--r--   0        0        0     1389 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      751 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/AUTHORS
+-rw-r--r--   0        0        0    13299 2023-05-06 09:16:04.401654 django-tag-fields-4.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    13597 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     5488 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5382 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1574 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/LICENSE
+-rw-r--r--   0        0        0      205 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     2739 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/README.rst
+-rw-r--r--   0        0        0      853 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/codecov.yml
+-rw-r--r--   0        0        0     1525 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/admin.rst
+-rw-r--r--   0        0        0     4396 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/api.rst
+-rw-r--r--   0        0        0       29 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0      471 2023-05-06 09:16:04.417654 django-tag-fields-4.0.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0     8990 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/custom_tagging.rst
+-rw-r--r--   0        0        0     2251 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/external_apps.rst
+-rw-r--r--   0        0        0     1040 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/faq.rst
+-rw-r--r--   0        0        0     2378 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/forms.rst
+-rw-r--r--   0        0        0     1902 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/getting_started.rst
+-rw-r--r--   0        0        0      705 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/index.rst
+-rw-r--r--   0        0        0      810 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/serializers.rst
+-rw-r--r--   0        0        0     1854 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/requirements/docs.txt
+-rw-r--r--   0        0        0       36 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/requirements/test.txt
+-rw-r--r--   0        0        0       38 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/setup.py
+-rw-r--r--   0        0        0      259 2023-05-06 09:16:04.421654 django-tag-fields-4.0.2/tag_fields/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/admin.py
+-rw-r--r--   0        0        0      253 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/apps.py
+-rw-r--r--   0        0        0     1442 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/forms.py
+-rw-r--r--   0        0        0     1299 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2206 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1042 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2005 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1033 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1941 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1068 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1839 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      991 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2188 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1738 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1131 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1873 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1058 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2021 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1203 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2162 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1047 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1928 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1105 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2073 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      828 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1955 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      945 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1904 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1142 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1908 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      993 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1947 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      933 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1739 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1045 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1897 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1870 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2544 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1051 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2014 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1211 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2144 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      992 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1982 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    30372 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/managers.py
+-rw-r--r--   0        0        0     2694 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0001_initial.py
+-rw-r--r--   0        0        0      280 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0002_auto_20150616_2121.py
+-rw-r--r--   0        0        0      374 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0003_taggeditem_add_unique_index.py
+-rw-r--r--   0        0        0     1232 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
+-rw-r--r--   0        0        0      502 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0005_auto_20220424_2025.py
+-rw-r--r--   0        0        0        0 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/__init__.py
+-rw-r--r--   0        0        0     7778 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/models.py
+-rw-r--r--   0        0        0     4417 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/serializers.py
+-rw-r--r--   0        0        0     4476 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/utils.py
+-rw-r--r--   0        0        0     1583 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/views.py
+-rw-r--r--   0        0        0        0 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/admin.py
+-rw-r--r--   0        0        0      168 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/custom_parser.py
+-rw-r--r--   0        0        0      834 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/forms.py
+-rw-r--r--   0        0        0    39683 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3529 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0002_auto_20200214_1129.py
+-rw-r--r--   0        0        0     3015 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0003_auto_20210310_0918.py
+-rw-r--r--   0        0        0     4440 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0004_auto_20210619_0826.py
+-rw-r--r--   0        0        0     1025 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0005_auto_20210713_2301.py
+-rw-r--r--   0        0        0        0 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/__init__.py
+-rw-r--r--   0        0        0    10311 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/models.py
+-rw-r--r--   0        0        0      323 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/serializers.py
+-rw-r--r--   0        0        0     1333 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/settings.py
+-rw-r--r--   0        0        0      124 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/templates/tests/food_tag_list.html
+-rw-r--r--   0        0        0     1394 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_admin.py
+-rw-r--r--   0        0        0     1857 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_forms.py
+-rw-r--r--   0        0        0     2359 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_models.py
+-rw-r--r--   0        0        0     3366 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_serializers.py
+-rw-r--r--   0        0        0      984 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0    54035 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/tests.py
+-rw-r--r--   0        0        0      294 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/urls.py
+-rw-r--r--   0        0        0      182 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/views.py
+-rw-r--r--   0        0        0     1174 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tox.ini
+-rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 django-tag-fields-4.0.2/PKG-INFO
```

### Comparing `django-tag-fields-4.0.1/.github/.git-commit-template.txt` & `django-tag-fields-4.0.2/.github/.git-commit-template.txt`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/bug-report.md` & `django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.github/ISSUE_TEMPLATE/feature-request.md` & `django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.github/semantic.yaml` & `django-tag-fields-4.0.2/.github/semantic.yaml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.github/workflows/release.yml` & `django-tag-fields-4.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.github/workflows/test.yml` & `django-tag-fields-4.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.gitignore` & `django-tag-fields-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/.pre-commit-config.yaml` & `django-tag-fields-4.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/AUTHORS` & `django-tag-fields-4.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/CHANGELOG.rst` & `django-tag-fields-4.0.2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   URL routing configurations).
 
   Generally speaking, this should not require action on your part as a library user, as
   existing tag slugs are persisted in the database, and only new tags will receive the
   enhanced unicode-compatible slug.
 
   If you wish to maintain the old stripping behavior, set the setting
-  ``TAGGIT_STRIP_UNICODE_WHEN_SLUGIFYING`` to ``True``.
+  ``TAGS_STRIP_UNICODE_WHEN_SLUGIFYING`` to ``True``.
 
   As a reminder, custom tag models can easily customize slugification behavior by overriding
   the ``slugify`` method to your business needs.
 
 `` Drop Django 2.2 support.
 
 2.1.0 (2022-01-24)
```

### Comparing `django-tag-fields-4.0.1/CODE_OF_CONDUCT.md` & `django-tag-fields-4.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/CONTRIBUTING.rst` & `django-tag-fields-4.0.2/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,121 +4,115 @@
 By contributing you agree to abide by the `Contributor Code of Conduct
 <https://github.com/imAsparky/django-tag-fields/blob/main/CODE_OF_CONDUCT.md>`_.
 
 Thank you for taking the time to contribute to django-tag-fields.
 
 Follow these guidelines to speed up the process.
 
-|
-
 Reach out before you start
 --------------------------
 
 Before opening a new issue, check if somebody else has already started working
 on the same issue in the ``GitHub`` `issues
 <https://github.com/imAsparky/django-tag-fields/issues>`_ and `pull requests
 <https://github.com/imAsparky/django-tag-fields/pulls>`_.
 
-|
-
 Fork the repository
 -------------------
 
 After forking this repository to your GitHub account, install your fork in your
 local development environment.
 
 .. code-block:: console
 
     # Clone your forked repository
     git clone git@github.com:<your_fork>/django-tag-fields.git
 
     # Change to the working directory
     cd django-tag-fields
 
-
-|
-
 Setup a virtual environment
 ---------------------------
 
 Use ``venv`` or your preferred virtual environment tool.
 
 Install the dependencies and setup ``pre-commit``.
 
 .. code-block:: console
+    :caption: **Create a virtual environment**
 
-
-    # Create a virtual environment
     python -m venv venv
 
-    # Activate your virtual environment, if venv it will be
+
+.. code-block:: console
+    :caption: **Activate your virtual environment, if venv it will be**
+
     . venv/bin/activate
 
-    # Install dependencies
+
+.. code-block:: console
+    :caption: **Install dependencies**
+
     pip install --upgrade pip
     pip install -r requirements/test.txt
     pip install -r requirements/docs.txt
 
-    # Setup pre-commit
+.. code-block:: console
+    :caption: **Setup pre-commit**
+
     pre-commit install
+.. code-block:: console
+    :caption: **Install django-tag-fields for local development**
 
-    # Install django-tag-fields for local development.
     python -m pip install -e .
 
 
 Running tests
 -------------
 
 django-tag-fields uses `tox <https://tox.readthedocs.io/>`_ to run tests:
 
 .. code-block:: console
 
     tox
 
-|
 
 Follow style conventions (black, flake8, isort)
 -----------------------------------------------
 
 Check that your changes are not breaking the style conventions with pre-commit.
 
 .. code-block:: console
 
     git add <your updated files>
 
     pre-commit
 
-|
-
 Update the documentation
 ------------------------
 
 When adding new features or modifying documented behaviour, it is important
 to remember to update the corresponding documentation.
 
 You can find the documentation in the "docs" directory of the repository.
 
 To make changes to the documentation, follow these steps.
 
 .. code-block:: console
 
     sphinx-build -n -W docs docs/_build
 
-|
-
 Add a changelog line
 --------------------
 
 Including a changelog line, even for minor changes, is helpful, as it helps
 explain the intention behind the change and alerts users who are upgrading.
 To do this, add a line to the ``(Unreleased)`` section of the ``CHANGELOG.rst``
 file and any additional details for more complex changes.
 
-|
-
 Commit/Release process
 ----------------------
 
 Releases are handled by `python-semantic-release <https://python-semantic-
 release.readthedocs.io/en/latest/>`_.
 
 .. caution::
@@ -149,16 +143,14 @@
 simply update your local git repo with the following command.
 
 
 .. code-block:: bash
 
     git config --local commit.template .github/.git-commit-template.txt
 
-|
-
 .. code-block:: vim
     :caption:  Available tags for commit message.
 
     # Tags with ** will be included in the CHANGELOG
 
     # **   chore    (a chore that needs to be done)
     #      dbg      (changes in debugging code/frameworks; no production code change)
@@ -183,7 +175,9 @@
 
 It is now time to push your changes to GitHub and open a `pull request
 <https://github.com/imAsparky/django-tag-fields/pulls>`_!
 
 |
 
 Thank you for your contribution.
+
+|
```

### Comparing `django-tag-fields-4.0.1/LICENSE` & `django-tag-fields-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/README.rst` & `django-tag-fields-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/codecov.yml` & `django-tag-fields-4.0.2/codecov.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/admin.rst` & `django-tag-fields-4.0.2/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/api.rst` & `django-tag-fields-4.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/custom_tagging.rst` & `django-tag-fields-4.0.2/docs/custom_tagging.rst`

 * *Files 6% similar despite different names*

```diff
@@ -172,28 +172,29 @@
 
 
     class Drink(models.Model):
         # ... fields here
 
         tags = TaggableManager(through=TaggedWhatever)
 
-|
 
 .. class:: TagBase
 
     .. method:: slugify(tag, i=None)
 
-        By default ``tag-fields`` uses :func:`django.utils.text.slugify` to
-        calculate a slug for a given tag.
+      The ``tag-fields`` feature uses the :func:`django.utils.text.slugify`
+      as the default method to generate a slug for a tag.
 
-        However, if you want to implement your logic, you can override this
-        method, which receives the ``tag`` (a string), and ``i``, which is
-        either ``None`` or an integer, which signifies how many times the slug
-        for this tag has been attempted to be calculated.  It is ``None`` on
-        the first attempt, and the counting begins at ``1`` thereafter.
+      But if you wish to use your logic, you can customize this process by
+      overriding the method.
+
+      The method takes in two arguments: the ``tag`` as a string and an
+      ``integer`` ``i``. If ``i`` is ``None``, it's the first attempt to
+      generate a slug for the tag, while a number greater than zero indicates
+      the number of attempts to create a unique slug.
 
 
 Using a custom tag string parser
 --------------------------------
 
 By default, ``django-tag-fields`` uses ``tag_fields.utils._parse_tags``, which
 accepts a string that may contain one or more tags and returns a list of tag
@@ -208,43 +209,39 @@
 * disallow certain characters
 * split only on commas rather than commas and whitespace
 * etc
 
 To provide your parser, write a function that takes a tag string and returns
 a list of tag names.
 
-|
 
 For example, see a simple function to split on comma's and convert to lowercase
 below.
 
-|
-
   .. code-block:: python
 
     def comma_splitter(tag_string):
         return [t.strip().lower() for t in tag_string.split(',') if t.strip()]
 
-|
 
 To use a specific function instead of the string parser, add a new setting
-called "TAGGIT_TAGS_FROM_STRING" and provide its dotted path to your desired
+called "TAGS_GET_TAGS_FROM_STRING" and provide its dotted path to your desired
 function.
 
 
 You can also offer a function that transforms a collection of tags into a
 string format. To change the default value
 (which is "tag_fields.utils._edit_string_for_tags"), use the
-"TAGGIT_STRING_FROM_TAGS" setting.
+"TAGS_GET_STRING_FROM_TAGS" setting.
 
   .. code-block:: python
 
     def comma_joiner(tags):
         return ', '.join(t.name for t in tags)
 
 To define the above functions in a module called "appname.utils", your
 project's settings.py file should include the following.
 
   .. code-block:: python
 
-    TAGGIT_TAGS_FROM_STRING = 'appname.utils.comma_splitter'
-    TAGGIT_STRING_FROM_TAGS = 'appname.utils.comma_joiner'
+    TAGS_GET_TAGS_FROM_STRING = 'appname.utils.comma_splitter'
+    TAGS_GET_STRING_FROM_TAGS = 'appname.utils.comma_joiner'
```

### Comparing `django-tag-fields-4.0.1/docs/external_apps.rst` & `django-tag-fields-4.0.2/docs/external_apps.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/faq.rst` & `django-tag-fields-4.0.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/forms.rst` & `django-tag-fields-4.0.2/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/docs/getting_started.rst` & `django-tag-fields-4.0.2/docs/getting_started.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,75 +4,69 @@
 To get started using ``django-tag-fields`` simply install it with
 ``pip``.
 
 .. code-block:: console
 
     $ pip install django-tag-fields
 
-|
 
 Add ``"tag_fields"`` to your project's ``INSTALLED_APPS`` setting and ``migrate``.
 
 .. code-block:: console
 
     ./manage.py migrate
 
-|
 
 And then, to any model you want tagged, do the following.
 
 .. code-block:: python
 
     from django.db import models
 
     from tag_fields.managers import TaggableManager
 
     class Food(models.Model):
         # ... fields here
 
         tags = TaggableManager()
 
-|
 
 .. tip::
 
-    To make ``django-tag-fields`` search for existing tags in a case-insensitive
-    way, you need to modify the ``TAGGIT_CASE_INSENSITIVE`` setting.
+    To make ``django-tag-fields`` search for existing tags in a
+    case-insensitive way, you need to modify the ``TAGS_CASE_INSENSITIVE``
+    setting.
 
     By default, it is set to ``False``, but you can change it to ``True`` in
     your Django settings file or wherever you store your settings.
 
     .. code-block:: python
 
-      TAGGIT_CASE_INSENSITIVE = True
+      TAGS_CASE_INSENSITIVE = True
 
 
 Settings
 --------
 
-|
-
-The following Django-level settings affect the behaviour of the library.
+You can alter ``django-tag-fields`` behaviour by changing the Django-level
+settings below.
 
 .. code-block:: python
 
 
-  TAGGIT_CASE_INSENSITIVE
+  TAGS_CASE_INSENSITIVE
 
   """"
   Defaults to ``False``.  When set to ``True``, tag lookups will be case
   insensitive.
   """
 
-
-|
-
 .. code-block:: python
 
-  TAGGIT_STRIP_UNICODE_WHEN_SLUGIFYING
+  TAGS_STRIP_UNICODE_WHEN_SLUGIFYING
 
   """"
   Defaults to False.  When set to True, tag slugs will be limited to ASCII
   characters.
 
   If ``True`` and you also have ``unidecode`` installed,
   then tag sluggification will transform a tag like (あい うえお) to (ai-ueo).
@@ -80,10 +74,10 @@
   If ``True`` and do not have ``unidecode`` installed, then you will usually
   be stripping Unicode, meaning that something like ``helloあい`` will be
   slugified as ``hello``.
   """
 
 .. caution::
 
-  The behaviour of ``TAGGIT_STRIP_UNICODE_WHEN_SLUGIFYING`` , when ``True``,
+  The behaviour of ``TAGS_STRIP_UNICODE_WHEN_SLUGIFYING`` , when ``True``,
   leads to situations where  slugs can be entirely stripped to an empty string;
   we **dont** recommend activating this.
```

### Comparing `django-tag-fields-4.0.1/docs/index.rst` & `django-tag-fields-4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/pyproject.toml` & `django-tag-fields-4.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 Repository = "https://github.com/imAsparky/django-tag-fields"
 Tracker = "https://github.com/imAsparky/django-tag-fields/issues"
 
 
 [tool.semantic_release]
 branch = "main"
 build_command = 'python -m pip install flit && flit build'
-changelog_file = "CHANGELOG.rst"
+changelog_file = "CHANGELOG.md"
 commit_subject = ":memo: build(version): Bump to version - {version}."
 version_variable = "docs/conf.py:__version__,tag_fields/__init__.py:__version__"
 
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 # tests = ["B201", "B301"]
```

### Comparing `django-tag-fields-4.0.1/tag_fields/forms.py` & `django-tag-fields-4.0.2/tag_fields/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ar/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/cs/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/da/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/de/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/el/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/en/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/eo/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/es/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fa/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fi/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/fr/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/he/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/it/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ja/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/nb/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/nl/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/pt_BR/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/ru/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/tr/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/uk/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po` & `django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/managers.py` & `django-tag-fields-4.0.2/tag_fields/managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,33 @@
 
     def __init__(self, alias, col, content_types):
         self.alias = alias
         self.col = col
         self.content_types = content_types
 
     def as_sql(self, compiler, connection):
+        """
+        Returns content_types and a string/list of  Join Restrictions.
+
+        Paramaters
+        ==========
+
+        :param compiler: A bandle to :class:`django.db.models.sql.compiler.SQLCompiler` # noqa: E501
+        :type compiler: class:`django.db.models.sql.compiler.SQLCompiler`
+
+        :param connection: todo
+        :type connection: todo
+
+        :return: String is in the format `'alias.col = %s'` for one
+            content_type or 'alias.col IN (%s%s%s)' for multiple content types.
+        :rtype: str
+
+        :return content_types: A string or list of content types
+        :rtype: str or [str,str, ...]
+        """
         qn = compiler.quote_name_unless_alias
         if len(self.content_types) == 1:
             extra_where = f"{qn(self.alias)}.{qn(self.col)} = %s"
         else:
             extra_where = "{}.{} IN ({})".format(
                 qn(self.alias),
                 qn(self.col),
@@ -57,16 +76,42 @@
         self.alias = change_map.get(self.alias, self.alias)
 
     def clone(self):
         return type(self)(self.alias, self.col, self.content_types[:])
 
 
 class _TaggableManager(models.Manager):
-    # TODO investigate whether we can use a RelatedManager instead of all this
-    # stuff to take advantage of all the Django goodness
+    """
+    Base class for Taggable Manager.
+
+    Paramaters
+    ==========
+
+    :param through: The name of the django through table
+    :type through: str
+
+    :param model: The namen of the model for the Taggable manager
+    :type model: str
+
+    :param instance: Instance for the Taggable manager
+    :type instance: class:`models.Model`
+
+    :param prefetch_cache_name: todo
+    :type prefetch_cache_name: todo
+
+    :param ordering: todo
+    :type ordering: todo
+
+    .. todo::
+        Very old todo here.
+
+        Investigate whether we can use a RelatedManager instead of all this
+        stuff to take advantage of all the Django goodness
+    """
+
     def __init__(
         self,
         through,
         model,
         instance,
         prefetch_cache_name,
         ordering=None,
@@ -92,14 +137,29 @@
         except (AttributeError, KeyError):
             kwargs = extra_filters if extra_filters else {}
             return self.through.tags_for(
                 self.model, self.instance, **kwargs
             ).order_by(*self.ordering)
 
     def get_prefetch_queryset(self, instances, queryset=None):
+        """
+        Overrides get_prefetch_queryset.
+
+        Paramaters
+        ==========
+
+        :param instance: Instance for Self
+        :type instance: class:`models.Model`
+
+        :param queryset: A django queryset, Should be None and will raise an
+            error if supplied.
+        :type queryset: todo
+
+        :raises ValueError: Custom queryset can't be used for this lookup.
+        """
         if queryset is not None:
             raise ValueError("Custom queryset can't be used for this lookup.")
 
         instance = instances[0]
         db = self._db or router.db_for_read(type(instance), instance=instance)
 
         fieldname = (
@@ -160,14 +220,38 @@
             self.instance, "_prefetched_objects_cache", None
         )
         if prefetch_cache:
             prefetch_cache.pop(self.prefetch_cache_name, None)
 
     @require_instance_manager
     def add(self, *tags, through_defaults=None, tag_kwargs=None, **kwargs):
+        """
+        Add tags to an object using either ``Tag`` instances or strings.
+
+        Paramaters
+        ==========
+
+        :param tags: A list of tags to get or create.
+        :type tags: List  [str,str,str ...]
+
+        :param through_defaults: You can specify values for your custom through
+            model by providing an argument if necessary.
+
+        :param tag_kwargs: TDefault: None his enables users to set specific
+            parameters for the tags.
+        :type tag_kwargs: dict, optional
+
+        .. todo::
+
+            Check if hardcode 'tag_id' in ``vals`` or should the column name be
+            got dynamically from somewhere?
+
+            Old todo, see vals below.
+        """
+
         self._remove_prefetched_objects()
         if tag_kwargs is None:
             tag_kwargs = {}
         db = router.db_for_write(self.through, instance=self.instance)
 
         tag_objs = self._to_tag_model_instances(tags, tag_kwargs)
         new_ids = {t.pk for t in tag_objs}
@@ -225,15 +309,15 @@
             else:
                 raise ValueError(
                     "Cannot add {} ({}). Expected {} or str.".format(
                         t, type(t), type(self.through.tag_model())
                     )
                 )
 
-        case_insensitive = getattr(settings, "TAGGIT_CASE_INSENSITIVE", False)
+        case_insensitive = getattr(settings, "TAGS_CASE_INSENSITIVE", False)
         manager = self.through.tag_model()._default_manager.using(db)
 
         if case_insensitive:
             # Some databases can do case-insensitive comparison with IN, which
             # would be faster, but we can't rely on it or easily detect it.
             existing = []
             tags_to_create = []
@@ -437,14 +521,48 @@
             obj = items[tuple(result[k] for k in lookup_keys)]
             obj.similar_tags = result["n"]
             results.append(obj)
         return results
 
 
 class TaggableManager(RelatedField):
+    """
+    Manager for handling the actions required on Tags.
+
+    Paramaters
+    ==========
+
+    :param blank: Default: False Determines if the field is required
+    :type blank: bool, optional
+
+    :param help_text: Default: _("A comma-separated list of tags.") The help
+        text that should be used in forms, including the admin.
+    :type help_text: str, optional
+
+    :param manager: Default: :class:`managers._TaggableManager` The Taggable
+        manager to use for this instance.
+    :type manager:
+
+    :param ordering: Default: None
+    :type ordering: todo, optional
+
+    :param related_name:
+    :type related_name: str, optional
+
+     :param through: Default: None The through table model, see
+        :doc:`custom_tagging` for more information.
+    :type through: str, optional
+
+    :param to: Default: None
+    :type to: todo, optional
+
+    :param verbose_name: Default: _("Tags") This field's verbose name.
+    :type verbose_name: str, optional
+    """
+
     # Field flags
     many_to_many = True
     many_to_one = False
     one_to_many = False
     one_to_one = False
 
     _related_name_counter = 0
@@ -476,14 +594,24 @@
         )
 
         self.ordering = ordering
         self.swappable = False
         self.manager = manager
 
     def __get__(self, instance, model):
+        """
+        Check the instance has a primary key.
+
+        :raises ValueError: "%s objects need to have a primary key value "
+                "before you can access their tags." % model.__name__
+
+        :return: An instance of the default manager.
+        :rtype: :class:`managers._TaggableManager`
+        """
+
         if instance is not None and instance.pk is None:
             raise ValueError(
                 "%s objects need to have a primary key value "
                 "before you can access their tags." % model.__name__
             )
         return self.manager(
             through=self.through,
@@ -728,15 +856,16 @@
 
     @cached_property
     def reverse_path_infos(self):
         return self.get_reverse_path_info()
 
     def get_joining_columns(self, reverse_join=False):
         # RemovedInDjango60Warning
-        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d
+        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d # noqa: E501
+        # Use "get_joining_fields() instead."
         if reverse_join:
             return ((self.model._meta.pk.column, "object_id"),)
         else:
             return (("object_id", self.model._meta.pk.column),)
 
     def get_joining_fields(self, reverse_join=False):
         if reverse_join:
@@ -772,15 +901,16 @@
     if django.VERSION < (4, 0):
         get_extra_restriction = _get_extra_restriction_legacy
     else:
         get_extra_restriction = _get_extra_restriction
 
     def get_reverse_joining_columns(self):
         # RemovedInDjango60Warning
-        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d
+        # https://github.com/django/django/commit/8b1ff0da4b162e87edebd94e61f2cd153e9e159d # noqa: E501
+        # Use "get_reverse_joining_fields() instead."
         return self.get_joining_columns(reverse_join=True)
 
     def get_reverse_joining_fields(self):
         return self.get_joining_fields(reverse_join=True)
 
     @property
     def related_fields(self):
```

### Comparing `django-tag-fields-4.0.1/tag_fields/migrations/0001_initial.py` & `django-tag-fields-4.0.2/tag_fields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py` & `django-tag-fields-4.0.2/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tag_fields/models.py` & `django-tag-fields-4.0.2/tag_fields/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     # (That is, till we found a nice solution...)
                     return super().save(*args, **kwargs)
                 i += 1
         else:
             return super().save(*args, **kwargs)
 
     def slugify(self, tag, i=None):
-        if getattr(settings, "TAGGIT_STRIP_UNICODE_WHEN_SLUGIFYING", False):
+        if getattr(settings, "TAGS_STRIP_UNICODE_WHEN_SLUGIFYING", False):
             slug = slugify(unidecode(tag))
         else:
             slug = slugify(tag, allow_unicode=True)
         if i is not None:
             slug += "_%d" % i
         return slug
```

### Comparing `django-tag-fields-4.0.1/tag_fields/serializers.py` & `django-tag-fields-4.0.2/tag_fields/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,29 @@
         try:
             return TagList(result)
         except TypeError:
             return result
 
     def __str__(self):
         if self.pretty_print:
-            return json.dumps(self, sort_keys=True, indent=4, separators=(",", ": "))
+            return json.dumps(
+                self, sort_keys=True, indent=4, separators=(",", ": ")
+            )
         else:
             return json.dumps(self)
 
 
 class TagListSerializerField(serializers.ListField):
     """
     A serializer field that can write out a tag list
 
-    This serializer field has some odd qualities compared to just using a ListField.
-    If this field poses problems, we should introduce a new field that is a simpler
-    ListField implementation with less features.
+    This serializer field has some odd qualities compared to just using a
+    ListField.
+    If this field poses problems, we should introduce a new field that is a
+    simpler ListField implementation with less features.
     """
 
     child = serializers.CharField()
     default_error_messages = {
         "not_a_list": gettext_lazy(
             'Expected a list of items but got type "{input_type}".'
         ),
@@ -105,15 +108,15 @@
                     tags = value.all()
                 value = [tag.name for tag in tags]
             value = TagList(value, pretty_print=self.pretty_print)
 
         return value
 
 
-class TaggitSerializer(serializers.Serializer):
+class TagSerializer(serializers.Serializer):
     def create(self, validated_data):
         to_be_tagged, validated_data = self._pop_tags(validated_data)
 
         tag_object = super().create(validated_data)
 
         return self._save_tags(tag_object, to_be_tagged)
```

### Comparing `django-tag-fields-4.0.1/tag_fields/utils.py` & `django-tag-fields-4.0.2/tag_fields/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,29 +113,38 @@
             names.append('"%s"' % name)
         else:
             names.append(name)
     return ", ".join(sorted(names))
 
 
 def require_instance_manager(func):
+    """
+    Checks the instance exists.
+
+    :raises TypeError: "Can't call %s with a non-instance manager" % func.__name__ # noqa: E501
+
+    """
+
     @wraps(func)
     def inner(self, *args, **kwargs):
         if self.instance is None:
-            raise TypeError("Can't call %s with a non-instance manager" % func.__name__)
+            raise TypeError(
+                "Can't call %s with a non-instance manager" % func.__name__
+            )
         return func(self, *args, **kwargs)
 
     return inner
 
 
 def get_func(key, default):
     func_path = getattr(settings, key, None)
     return default if func_path is None else import_string(func_path)
 
 
 def parse_tags(tagstring):
-    func = get_func("TAGGIT_TAGS_FROM_STRING", _parse_tags)
+    func = get_func("TAGS_GET_TAGS_FROM_STRING", _parse_tags)
     return func(tagstring)
 
 
 def edit_string_for_tags(tags):
-    func = get_func("TAGGIT_STRING_FROM_TAGS", _edit_string_for_tags)
+    func = get_func("TAGS_GET_STRING_FROM_TAGS", _edit_string_for_tags)
     return func(tags)
```

### Comparing `django-tag-fields-4.0.1/tag_fields/views.py` & `django-tag-fields-4.0.2/tag_fields/views.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/forms.py` & `django-tag-fields-4.0.2/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/migrations/0001_initial.py` & `django-tag-fields-4.0.2/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/migrations/0002_auto_20200214_1129.py` & `django-tag-fields-4.0.2/tests/migrations/0002_auto_20200214_1129.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/migrations/0003_auto_20210310_0918.py` & `django-tag-fields-4.0.2/tests/migrations/0003_auto_20210310_0918.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/migrations/0004_auto_20210619_0826.py` & `django-tag-fields-4.0.2/tests/migrations/0004_auto_20210619_0826.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/migrations/0005_auto_20210713_2301.py` & `django-tag-fields-4.0.2/tests/migrations/0005_auto_20210713_2301.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/models.py` & `django-tag-fields-4.0.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/settings.py` & `django-tag-fields-4.0.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/test_admin.py` & `django-tag-fields-4.0.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/test_forms.py` & `django-tag-fields-4.0.2/tests/test_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 def _test_parse_tags(tagstring):
     if "," in tagstring:
         return tagstring.split(",")
     else:
         raise ValueError()
 
 
-@override_settings(TAGGIT_TAGS_FROM_STRING="tests.test_forms._test_parse_tags")
+@override_settings(
+    TAGS_GET_TAGS_FROM_STRING="tests.test_forms._test_parse_tags"
+)
 class TagFieldTests(TestCase):
     def test_should_return_error_on_clean_if_not_comma_separated(self):
         class TestForm(forms.Form):
             tag = TagField()
 
         excpected_error = "Please provide a comma-separated list of tags."
```

### Comparing `django-tag-fields-4.0.1/tests/test_models.py` & `django-tag-fields-4.0.2/tests/test_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,24 @@
         """
         Confirm the preservation of unicode in slugification by default
         """
         sample_obj = TestModel.objects.create()
         # a unicode tag will be slugified for space reasons but
         # unicode-ness will be kept by default
         sample_obj.tags.add("あい うえお")
-        self.assertEqual([tag.slug for tag in sample_obj.tags.all()], ["あい-うえお"])
+        self.assertEqual(
+            [tag.slug for tag in sample_obj.tags.all()], ["あい-うえお"]
+        )
 
     def test_old_slugs(self):
         """
         Test that the setting that gives us the old slugification behavior
         is in place
         """
-        with override_settings(TAGGIT_STRIP_UNICODE_WHEN_SLUGIFYING=True):
+        with override_settings(TAGS_STRIP_UNICODE_WHEN_SLUGIFYING=True):
             sample_obj = TestModel.objects.create()
             # a unicode tag will be slugified for space reasons but
             # unicode-ness will be kept by default
             sample_obj.tags.add("あい うえお")
             self.assertEqual([tag.slug for tag in sample_obj.tags.all()], [""])
```

### Comparing `django-tag-fields-4.0.1/tests/test_serializers.py` & `django-tag-fields-4.0.2/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/test_utils.py` & `django-tag-fields-4.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/tests/tests.py` & `django-tag-fields-4.0.2/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -805,29 +805,29 @@
             )
             self.assertEqual(
                 connection.queries[-1]["sql"].count(join_clause),
                 1,
                 connection.queries[-2:],
             )
 
-    @override_settings(TAGGIT_CASE_INSENSITIVE=True)
+    @override_settings(TAGS_CASE_INSENSITIVE=True)
     def test_with_case_insensitive_option(self):
         spain = self.tag_model.objects.create(name="Spain", slug="spain")
         orange = self.food_model.objects.create(name="orange")
         orange.tags.add("spain")
         self.assertEqual(list(orange.tags.all()), [spain])
 
-    @override_settings(TAGGIT_CASE_INSENSITIVE=True)
+    @override_settings(TAGS_CASE_INSENSITIVE=True)
     def test_with_case_insensitive_option_and_creation(self):
         orange = self.food_model.objects.create(name="orange")
         orange.tags.add("spain", "Spain")
         tag_names = list(orange.tags.names())
         self.assertEqual(len(tag_names), 1, tag_names)
 
-    @override_settings(TAGGIT_CASE_INSENSITIVE=True)
+    @override_settings(TAGS_CASE_INSENSITIVE=True)
     def test_with_case_insensitive_option_new_and_old(self):
         orange = self.food_model.objects.create(name="orange")
         orange.tags.add("Spain")
         tag_names = list(orange.tags.names())
         self.assertEqual(len(tag_names), 1, tag_names)
         orange.tags.add("spain", "Valencia")
         tag_names = sorted(orange.tags.names())
@@ -1316,27 +1316,27 @@
             edit_string_for_tags([plain, comma]), '"com,ma", plain'
         )
         self.assertEqual(
             edit_string_for_tags([comma, spaces]), '"com,ma", "spa ces"'
         )
 
     @override_settings(
-        TAGGIT_TAGS_FROM_STRING="tests.custom_parser.comma_splitter"
+        TAGS_GET_TAGS_FROM_STRING="tests.custom_parser.comma_splitter"
     )
     def test_custom_comma_splitter(self):
         self.assertEqual(parse_tags("   Cued Speech "), ["Cued Speech"])
         self.assertEqual(parse_tags(" ,Cued Speech, "), ["Cued Speech"])
         self.assertEqual(parse_tags("Cued Speech"), ["Cued Speech"])
         self.assertEqual(
             parse_tags("Cued Speech, dictionary"),
             ["Cued Speech", "dictionary"],
         )
 
     @override_settings(
-        TAGGIT_STRING_FROM_TAGS="tests.custom_parser.comma_joiner"
+        TAGS_GET_STRING_FROM_TAGS="tests.custom_parser.comma_joiner"
     )
     def test_custom_comma_joiner(self):
         a = Tag(name="Cued Speech")
         b = Tag(name="transliterator")
         self.assertEqual(
             edit_string_for_tags([a, b]), "Cued Speech, transliterator"
         )
```

### Comparing `django-tag-fields-4.0.1/tox.ini` & `django-tag-fields-4.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.1/PKG-INFO` & `django-tag-fields-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tag-fields
-Version: 4.0.1
+Version: 4.0.2
 Summary: Add field tags to a Django project
 Keywords: Django,django,django tagging
 Author-email: Alex Gaynor <alex.gaynor@gmail.com>
 Maintainer-email: Mark Sevelj <mark.sevelj@dunwright.com.au>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 1 - Planning
```

