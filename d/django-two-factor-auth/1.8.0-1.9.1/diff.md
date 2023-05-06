# Comparing `tmp/django-two-factor-auth-1.8.0.tar.gz` & `tmp/django-two-factor-auth-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-two-factor-auth-1.8.0.tar", last modified: Fri Aug  3 13:55:51 2018, max compression
+gzip compressed data, was "dist/django-two-factor-auth-1.9.1.tar", last modified: Sun Jul  7 07:01:37 2019, max compression
```

## Comparing `django-two-factor-auth-1.8.0.tar` & `django-two-factor-auth-1.9.1.tar`

### file list

```diff
@@ -1,170 +1,175 @@
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/
--rw-r--r--   0 bouke      (501) admin       (80)     6607 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/PKG-INFO
--rw-r--r--   0 bouke      (501) staff       (20)     1057 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/LICENSE
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/templatetags/
--rw-r--r--   0 bouke      (501) staff       (20)     1560 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templatetags/two_factor.py
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templatetags/__init__.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/middleware/
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/middleware/__init__.py
--rw-r--r--   0 bouke      (501) staff       (20)      396 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/middleware/threadlocals.py
--rw-r--r--   0 bouke      (501) staff       (20)      105 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/signals.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/migrations/
--rw-r--r--   0 bouke      (501) staff       (20)     1656 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/0003_auto_20150817_1733.py
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/__init__.py
--rw-r--r--   0 bouke      (501) staff       (20)      518 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/0004_auto_20160205_1827.py
--rw-r--r--   0 bouke      (501) staff       (20)     1560 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/0001_initial.py
--rw-r--r--   0 bouke      (501) staff       (20)     1609 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/0005_auto_20160224_0450.py
--rw-r--r--   0 bouke      (501) staff       (20)      564 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/migrations/0002_auto_20150110_0810.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/pl/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/pl/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    10439 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16681 2018-08-03 13:23:37.000000 django-two-factor-auth-1.8.0/two_factor/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/sv/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/sv/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    10287 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16400 2018-08-03 13:23:38.000000 django-two-factor-auth-1.8.0/two_factor/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9891 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15974 2018-08-03 13:23:37.000000 django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/it/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/it/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    10381 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16563 2018-08-03 13:23:34.000000 django-two-factor-auth-1.8.0/two_factor/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ru/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ru/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9250 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16876 2018-08-03 13:23:36.000000 django-two-factor-auth-1.8.0/two_factor/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/he_IL/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9537 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/he_IL/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16600 2018-08-03 13:23:35.000000 django-two-factor-auth-1.8.0/two_factor/locale/he_IL/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/hi_IN/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/hi_IN/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)      505 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/hi_IN/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    12033 2018-08-03 13:23:39.000000 django-two-factor-auth-1.8.0/two_factor/locale/hi_IN/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ro/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ro/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) admin       (80)    10801 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) admin       (80)    16932 2018-08-03 13:23:40.000000 django-two-factor-auth-1.8.0/two_factor/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9370 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15445 2018-08-03 13:23:36.000000 django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9949 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16055 2018-08-03 13:23:38.000000 django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/en_GB/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9829 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/en_GB/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15986 2018-08-03 13:23:35.000000 django-two-factor-auth-1.8.0/two_factor/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ar/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    12669 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    18825 2018-08-03 13:23:39.000000 django-two-factor-auth-1.8.0/two_factor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/nl/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/nl/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    11126 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16446 2018-08-03 13:41:29.000000 django-two-factor-auth-1.8.0/two_factor/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/nb/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/nb/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9571 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15663 2018-08-03 13:23:38.000000 django-two-factor-auth-1.8.0/two_factor/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/de/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/de/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9942 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16122 2018-08-03 13:23:36.000000 django-two-factor-auth-1.8.0/two_factor/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/as/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/as/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)      494 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/as/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    12022 2018-08-03 13:23:38.000000 django-two-factor-auth-1.8.0/two_factor/locale/as/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ca_ES/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/ca_ES/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)      507 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/ca_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    12035 2018-08-03 13:23:39.000000 django-two-factor-auth-1.8.0/two_factor/locale/ca_ES/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fi/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fi/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9738 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15844 2018-08-03 13:23:35.000000 django-two-factor-auth-1.8.0/two_factor/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)      512 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    12040 2018-08-03 13:23:37.000000 django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fr/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    10608 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16902 2018-08-03 13:23:35.000000 django-two-factor-auth-1.8.0/two_factor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/es/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/es/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)    10403 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    16588 2018-08-03 13:23:36.000000 django-two-factor-auth-1.8.0/two_factor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/en/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/en/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     5288 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15410 2018-08-03 13:23:23.000000 django-two-factor-auth-1.8.0/two_factor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fa/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/fa/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)      492 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    12020 2018-08-03 13:23:34.000000 django-two-factor-auth-1.8.0/two_factor/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/da_DK/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/locale/da_DK/LC_MESSAGES/
--rw-r--r--   0 bouke      (501) staff       (20)     9702 2018-08-03 13:41:30.000000 django-two-factor-auth-1.8.0/two_factor/locale/da_DK/LC_MESSAGES/django.mo
--rw-r--r--   0 bouke      (501) staff       (20)    15773 2018-08-03 13:23:39.000000 django-two-factor-auth-1.8.0/two_factor/locale/da_DK/LC_MESSAGES/django.po
--rw-r--r--   0 bouke      (501) staff       (20)     3338 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/models.py
--rw-r--r--   0 bouke      (501) staff       (20)      570 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/validators.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/management/
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/management/__init__.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/management/commands/
--rw-r--r--   0 bouke      (501) staff       (20)     1008 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/management/commands/two_factor_disable.py
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/management/commands/__init__.py
--rw-r--r--   0 bouke      (501) staff       (20)     1156 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/management/commands/two_factor_status.py
--rw-r--r--   0 bouke      (501) staff       (20)       55 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/__init__.py
--rw-r--r--   0 bouke      (501) staff       (20)      330 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/apps.py
--rw-r--r--   0 bouke      (501) staff       (20)     6366 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/forms.py
--rw-r--r--   0 bouke      (501) admin       (80)     2400 2018-08-03 13:07:09.000000 django-two-factor-auth-1.8.0/two_factor/admin.py
--rw-r--r--   0 bouke      (501) staff       (20)     1830 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/utils.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/gateways/
--rw-r--r--   0 bouke      (501) staff       (20)     1066 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/fake.py
--rw-r--r--   0 bouke      (501) staff       (20)      484 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/__init__.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/gateways/twilio/
--rw-r--r--   0 bouke      (501) staff       (20)     2713 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/twilio/gateway.py
--rw-r--r--   0 bouke      (501) staff       (20)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/twilio/__init__.py
--rw-r--r--   0 bouke      (501) staff       (20)      250 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/twilio/urls.py
--rw-r--r--   0 bouke      (501) staff       (20)     3317 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/gateways/twilio/views.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/templates/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/
--rw-r--r--   0 bouke      (501) staff       (20)      909 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/phone_register.html
--rw-r--r--   0 bouke      (501) staff       (20)     2075 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/login.html
--rw-r--r--   0 bouke      (501) staff       (20)      923 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/setup_complete.html
--rw-r--r--   0 bouke      (501) staff       (20)     1131 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0 bouke      (501) staff       (20)     2730 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/setup.html
--rw-r--r--   0 bouke      (501) staff       (20)      816 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/otp_required.html
--rw-r--r--   0 bouke      (501) staff       (20)       68 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_wizard_forms.html
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/profile/
--rw-r--r--   0 bouke      (501) staff       (20)     2754 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/profile/profile.html
--rw-r--r--   0 bouke      (501) admin       (80)      512 2018-08-03 13:07:09.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/profile/disable.html
--rw-r--r--   0 bouke      (501) staff       (20)     1013 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_base.html
--rw-r--r--   0 bouke      (501) staff       (20)      250 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_base_focus.html
--rw-r--r--   0 bouke      (501) staff       (20)      520 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_wizard_actions.html
--rw-r--r--   0 bouke      (501) staff       (20)     1462 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/urls.py
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/two_factor/views/
--rw-r--r--   0 bouke      (501) staff       (20)     2965 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/views/mixins.py
--rw-r--r--   0 bouke      (501) staff       (20)     2223 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/views/profile.py
--rw-r--r--   0 bouke      (501) staff       (20)      222 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/two_factor/views/__init__.py
--rw-r--r--   0 bouke      (501) admin       (80)    21008 2018-08-03 13:07:09.000000 django-two-factor-auth-1.8.0/two_factor/views/core.py
--rw-r--r--   0 bouke      (501) admin       (80)     8102 2018-08-03 13:07:09.000000 django-two-factor-auth-1.8.0/two_factor/views/utils.py
--rw-r--r--   0 bouke      (501) staff       (20)      125 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/MANIFEST.in
--rw-r--r--   0 bouke      (501) admin       (80)     1671 2018-08-03 13:55:35.000000 django-two-factor-auth-1.8.0/setup.py
--rw-r--r--   0 bouke      (501) staff       (20)      415 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/CONTRIBUTORS.rst
-drwxr-xr-x   0 bouke      (501) admin       (80)        0 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/
--rw-r--r--   0 bouke      (501) staff       (20)     6607 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/PKG-INFO
--rw-r--r--   0 bouke      (501) staff       (20)     4164 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/SOURCES.txt
--rw-r--r--   0 bouke      (501) staff       (20)      181 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/requires.txt
--rw-r--r--   0 bouke      (501) staff       (20)       11 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/top_level.txt
--rw-r--r--   0 bouke      (501) staff       (20)        1 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/dependency_links.txt
--rw-r--r--   0 bouke      (501) admin       (80)      510 2018-08-03 13:55:51.000000 django-two-factor-auth-1.8.0/setup.cfg
--rw-r--r--   0 bouke      (501) staff       (20)     4468 2017-12-19 05:54:37.000000 django-two-factor-auth-1.8.0/README.rst
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/
+-rw-r--r--   0 bouke      (501) admin       (80)      415 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/CONTRIBUTORS.rst
+-rw-r--r--   0 bouke      (501) admin       (80)     1057 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/LICENSE
+-rw-r--r--   0 bouke      (501) admin       (80)      125 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/MANIFEST.in
+-rw-r--r--   0 bouke      (501) admin       (80)     7098 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/PKG-INFO
+-rw-r--r--   0 bouke      (501) admin       (80)     4733 2019-07-07 06:53:23.000000 django-two-factor-auth-1.9.1/README.rst
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/
+-rw-r--r--   0 bouke      (501) admin       (80)     7098 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/PKG-INFO
+-rw-r--r--   0 bouke      (501) admin       (80)     4280 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 bouke      (501) admin       (80)        1 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 bouke      (501) admin       (80)      181 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/requires.txt
+-rw-r--r--   0 bouke      (501) admin       (80)       17 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/top_level.txt
+-rw-r--r--   0 bouke      (501) admin       (80)      515 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/setup.cfg
+-rw-r--r--   0 bouke      (501) admin       (80)     1758 2019-07-07 07:01:11.000000 django-two-factor-auth-1.9.1/setup.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/tests/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/tests/migrations/
+-rw-r--r--   0 bouke      (501) admin       (80)     1885 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/tests/migrations/0001_initial.py
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/tests/migrations/__init__.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/
+-rw-r--r--   0 bouke      (501) admin       (80)       55 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     2400 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/admin.py
+-rw-r--r--   0 bouke      (501) admin       (80)      334 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/two_factor/apps.py
+-rw-r--r--   0 bouke      (501) admin       (80)     6366 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/forms.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/gateways/
+-rw-r--r--   0 bouke      (501) admin       (80)      484 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1066 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/fake.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/gateways/twilio/
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/twilio/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     2713 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/twilio/gateway.py
+-rw-r--r--   0 bouke      (501) admin       (80)      250 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/twilio/urls.py
+-rw-r--r--   0 bouke      (501) admin       (80)     3317 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/gateways/twilio/views.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ar/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    14039 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    19618 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/as/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/as/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)      494 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/as/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    12022 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/as/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ca_ES/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ca_ES/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)      507 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/ca_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    12035 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/ca_ES/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/da_DK/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/da_DK/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9702 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/da_DK/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15773 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/da_DK/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/de/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/de/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9942 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16122 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/en/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     5288 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15414 2019-07-07 06:46:32.000000 django-two-factor-auth-1.9.1/two_factor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/en_GB/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9829 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/en_GB/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15986 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/es/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    10403 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16588 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fa/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)      492 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    12020 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fi/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    10030 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16035 2019-07-07 06:46:42.000000 django-two-factor-auth-1.9.1/two_factor/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fr/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    12364 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    17794 2019-07-07 06:46:42.000000 django-two-factor-auth-1.9.1/two_factor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/he_IL/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9537 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/he_IL/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16600 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/he_IL/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/hi_IN/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)      505 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/hi_IN/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    12033 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/hi_IN/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9949 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16055 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/it/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/it/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    10381 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16563 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)      512 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    12040 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/nb/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9571 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15663 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/nl/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    11270 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16509 2019-07-07 06:46:43.000000 django-two-factor-auth-1.9.1/two_factor/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/pl/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    10439 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16681 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9891 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15974 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ro/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    12565 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    17817 2019-07-07 06:46:43.000000 django-two-factor-auth-1.9.1/two_factor/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ru/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    15276 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    20646 2019-07-07 06:46:44.000000 django-two-factor-auth-1.9.1/two_factor/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/sv/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)    10287 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    16400 2018-08-05 06:54:58.000000 django-two-factor-auth-1.9.1/two_factor/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 bouke      (501) admin       (80)     9754 2019-07-07 06:46:45.000000 django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 bouke      (501) admin       (80)    15641 2019-07-07 06:46:43.000000 django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/management/
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/management/__init__.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/management/commands/
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/management/commands/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1008 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/management/commands/two_factor_disable.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1156 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/management/commands/two_factor_status.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/middleware/
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/middleware/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)      396 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/middleware/threadlocals.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/migrations/
+-rw-r--r--   0 bouke      (501) admin       (80)     1560 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0001_initial.py
+-rw-r--r--   0 bouke      (501) admin       (80)      564 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0002_auto_20150110_0810.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1656 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0003_auto_20150817_1733.py
+-rw-r--r--   0 bouke      (501) admin       (80)      518 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0004_auto_20160205_1827.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1609 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0005_auto_20160224_0450.py
+-rw-r--r--   0 bouke      (501) admin       (80)      492 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/two_factor/migrations/0006_phonedevice_key_default.py
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/migrations/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     3175 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/two_factor/models.py
+-rw-r--r--   0 bouke      (501) admin       (80)      105 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/signals.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/
+-rw-r--r--   0 bouke      (501) admin       (80)     1013 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_base.html
+-rw-r--r--   0 bouke      (501) admin       (80)      250 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_base_focus.html
+-rw-r--r--   0 bouke      (501) admin       (80)      520 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0 bouke      (501) admin       (80)       68 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_wizard_forms.html
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/
+-rw-r--r--   0 bouke      (501) admin       (80)     1131 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0 bouke      (501) admin       (80)     2075 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/login.html
+-rw-r--r--   0 bouke      (501) admin       (80)      816 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/otp_required.html
+-rw-r--r--   0 bouke      (501) admin       (80)      909 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/phone_register.html
+-rw-r--r--   0 bouke      (501) admin       (80)     2730 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/setup.html
+-rw-r--r--   0 bouke      (501) admin       (80)      927 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/setup_complete.html
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/profile/
+-rw-r--r--   0 bouke      (501) admin       (80)      512 2018-08-03 13:07:09.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/profile/disable.html
+-rw-r--r--   0 bouke      (501) admin       (80)     2754 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templates/two_factor/profile/profile.html
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/templatetags/
+-rw-r--r--   0 bouke      (501) admin       (80)        0 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templatetags/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1560 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/templatetags/two_factor.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1462 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/urls.py
+-rw-r--r--   0 bouke      (501) admin       (80)     1830 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/utils.py
+-rw-r--r--   0 bouke      (501) admin       (80)      570 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/validators.py
+drwxr-xr-x   0 bouke      (501) admin       (80)        0 2019-07-07 07:01:37.000000 django-two-factor-auth-1.9.1/two_factor/views/
+-rw-r--r--   0 bouke      (501) admin       (80)      222 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/views/__init__.py
+-rw-r--r--   0 bouke      (501) admin       (80)    21068 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/two_factor/views/core.py
+-rw-r--r--   0 bouke      (501) admin       (80)     2965 2017-12-19 05:54:37.000000 django-two-factor-auth-1.9.1/two_factor/views/mixins.py
+-rw-r--r--   0 bouke      (501) admin       (80)     2223 2019-07-07 06:39:44.000000 django-two-factor-auth-1.9.1/two_factor/views/profile.py
+-rw-r--r--   0 bouke      (501) admin       (80)     8106 2019-07-07 06:39:49.000000 django-two-factor-auth-1.9.1/two_factor/views/utils.py
```

### Comparing `django-two-factor-auth-1.8.0/PKG-INFO` & `django-two-factor-auth-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-two-factor-auth
-Version: 1.8.0
+Version: 1.9.1
 Summary: Complete Two-Factor Authentication for Django
 Home-page: https://github.com/Bouke/django-two-factor-auth
 Author: Bouke Haarsma
 Author-email: bouke@haarsma.eu
 License: MIT
 Download-URL: https://pypi.python.org/pypi/django-two-factor-auth
 Description: ================================
@@ -40,23 +40,32 @@
         Test drive this app through the online `example app`_, hosted by Heroku_. It
         demos most features except the Twilio integration. The example also includes
         django-user-sessions_ for providing Django sessions with a foreign key to the
         user. Although the package is optional, it improves account security control
         over ``django.contrib.sessions``.
         
         Compatible with modern Django versions. At the moment of writing that's
-        including 1.11 and 2.0 on Python 2.7, 3.4, 3.5 and 3.6. Documentation
+        including 1.11, 2.1, and 2.2 on Python 2.7, 3.4, 3.5, 3.6 and 3.7. Documentation
         is available at `readthedocs.org`_.
         
         
         Installation
         ============
         Refer to the `installation instructions`_ in the documentation.
         
         
+        Getting help
+        ============
+        
+        For general questions regarding this package, please hop over to Stack 
+        Overflow. If you think there is an issue with this package; check if the
+        issue is already listed (either open or closed), and file an issue if
+        it's not.
+        
+        
         Contribute
         ==========
         * Submit issues to the `issue tracker`_ on Github.
         * Fork the `source code`_ at Github.
         * Write some code and make sure it is covered with unit tests.
         * Send a pull request with your changes.
         * Provide a translation using Transifex_.
@@ -133,20 +142,25 @@
            https://hynek.me/articles/sharing-your-labor-of-love-pypi-quick-and-dirty/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
+Provides-Extra: Call
+Provides-Extra: SMS
+Provides-Extra: YubiKey
```

### Comparing `django-two-factor-auth-1.8.0/LICENSE` & `django-two-factor-auth-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templatetags/two_factor.py` & `django-two-factor-auth-1.9.1/two_factor/templatetags/two_factor.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/migrations/0003_auto_20150817_1733.py` & `django-two-factor-auth-1.9.1/two_factor/migrations/0003_auto_20150817_1733.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/migrations/0004_auto_20160205_1827.py` & `django-two-factor-auth-1.9.1/two_factor/migrations/0004_auto_20160205_1827.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/migrations/0001_initial.py` & `django-two-factor-auth-1.9.1/two_factor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/migrations/0005_auto_20160224_0450.py` & `django-two-factor-auth-1.9.1/two_factor/migrations/0005_auto_20160224_0450.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/migrations/0002_auto_20150110_0810.py` & `django-two-factor-auth-1.9.1/two_factor/migrations/0002_auto_20150110_0810.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/pl/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/pl/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/sv/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/sv/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/pt_BR/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/it/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/it/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ru/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/nb/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,290 +1,288 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
-# Jan Pol <pavel@yarkovoy.com>, 2018
-# Mikhail M <malexey1984@gmail.com>, 2017
-# partizan <serg.partizan@gmail.com>, 2017
+# Stein Strindhaug <stein.strindhaug@gmail.com>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-08-03 15:23+0200\n"
 "PO-Revision-Date: 2018-08-03 13:23+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
-"Language-Team: Russian (http://www.transifex.com/Bouke/django-two-factor-auth/language/ru/)\n"
+"Language-Team: Norwegian Bokmål (http://www.transifex.com/Bouke/django-two-factor-auth/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: nb\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
-msgstr "Метод"
+msgstr "Metode"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
 msgstr ""
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
-msgstr "Токен"
+msgstr "Engangskode"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
 msgid "Entered token is not valid."
-msgstr "Введен некорректный токен"
+msgstr "Engangskoden er ugyldig"
 
 #: forms.py:76 forms.py:170 models.py:42
 msgid "YubiKey"
 msgstr "YubiKey"
 
 #: forms.py:79
 msgid "The YubiKey could not be verified."
-msgstr "Неправильный YubiKey"
+msgstr "Kunne ikke verifisere YubiKey'en."
 
 #: forms.py:138
 msgid "Yes, I am sure"
-msgstr "Да, я уверен"
+msgstr "Ja, jeg er sikker"
 
 #: gateways/twilio/gateway.py:61
 #, python-format
 msgid "Your authentication token is %s"
-msgstr "Ваш код авторизации: %s"
+msgstr "Auteniseringskoden din er %s"
 
 #. Translators: twilio_locale should be a locale supported by
 #. Twilio, see http://bit.ly/187I5cr
 #: gateways/twilio/gateway.py:70 gateways/twilio/views.py:74
 msgctxt "twilio_locale"
 msgid "en"
-msgstr "en"
+msgstr "nb-NO"
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:39
 #, python-format
 #| msgid ""
 #| "is is %(site_name)s calling. Please enter the following code on r "
 #| "screen:token)s. Repeat: %(token)s."
 msgid "Hi, this is %(site_name)s calling. Press any key to continue."
-msgstr "Привет, это %(site_name)sвызывает. Нажмите любую кнопку для продолжения."
+msgstr "Hei, dette er %(site_name)s som ringer. Trykk en tast for å fortsette."
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:44
 #, python-format
 msgid "Your token is %(token)s. Repeat: %(token)s. Good bye."
-msgstr "Ваш код %(token)s. Повторяю: %(token)s. До свидания."
+msgstr "Din kode er %(token)s. Jeg gjentar: %(token)s. Ha det."
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:48
 #| msgid "You don't have any backup codes yet."
 msgid "You didn't press any keys. Good bye."
-msgstr "Вы не нажали любую кнопку. Прощайте."
+msgstr "Du trykket ikke noen tast. Ha det."
 
 #: models.py:25
 msgid "Phone Call"
-msgstr "Телефонный звонок"
+msgstr "Telefonsamtale"
 
 #: models.py:26
 msgid "Text Message"
-msgstr "SMS сообщение"
+msgstr "SMS"
 
 #: models.py:33
 #| msgid "Phone Call"
 msgid "Phone call"
-msgstr "Телефонный звонок"
+msgstr "Telefonsamtale"
 
 #: models.py:35
 #| msgid "Text Message"
 msgid "Text message"
-msgstr "SMS сообщение"
+msgstr "SMS"
 
 #: models.py:47
 msgid "Token generator"
-msgstr "Генератор токенов"
+msgstr "Kodegenerator"
 
 #: models.py:71
 msgid "method"
-msgstr "метод"
+msgstr "metode"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
-msgstr "Отмена"
+msgstr "Avbryt"
 
 #: templates/two_factor/_wizard_actions.html:10
 #: templates/two_factor/_wizard_actions.html:13
 msgid "Back"
-msgstr "Назад"
+msgstr "Tilbake"
 
 #: templates/two_factor/_wizard_actions.html:15
 msgid "Next"
-msgstr "Далее"
+msgstr "Neste"
 
 #: templates/two_factor/core/backup_tokens.html:5
 #: templates/two_factor/profile/profile.html:37
 msgid "Backup Tokens"
-msgstr "Резервные токены"
+msgstr "Reserve-koder"
 
 #: templates/two_factor/core/backup_tokens.html:6
 msgid ""
 "Backup tokens can be used when your primary and backup\n"
 "      phone numbers aren't available. The backup tokens below can be used\n"
 "      for login verification. If you've used up all your backup tokens, you\n"
 "      can generate a new set of backup tokens. Only the backup tokens shown\n"
 "      below will be valid."
-msgstr "Резервные токены могут использоваться когда ваше основное устройство недоступно.\nТокены из спииска ниже могут использоваться для подтверждения логина.\nЕсли вы использовали все токены, можно сгенерировать новые.\nСейчас активны только токены из списка ниже."
+msgstr "Reservekoder kan brukes når hoved og reserve telefonnummeret ditt ikke er tilgjengelig. Reservekodene nedenfor kan benyttes for innloggingsverifikasjon. Hivs du har brukt opp alle reservekodene kan du generere et nytt sett med koder. Bare reservekodene vist nedenfor vil være gyldige."
 
 #: templates/two_factor/core/backup_tokens.html:18
 msgid "Print these tokens and keep them somewhere safe."
-msgstr "Распечатайте эти токены и храните их в безопасном месте."
+msgstr "Skriv ut disse kodene og oppbevar dem et trygt sted."
 
 #: templates/two_factor/core/backup_tokens.html:20
 msgid "You don't have any backup codes yet."
-msgstr "У Вас нет резервных кодов."
+msgstr "Du har ikke noen reservekoder ennå."
 
 #: templates/two_factor/core/backup_tokens.html:25
 msgid "Back to Account Security"
-msgstr "Назад к Безопасности"
+msgstr "Tilbake til kontosikkerhet"
 
 #: templates/two_factor/core/backup_tokens.html:26
 msgid "Generate Tokens"
-msgstr "Сгенерировать токены"
+msgstr "Lag engangskoder"
 
 #: templates/two_factor/core/login.html:5
 msgid "Login"
-msgstr "Логин"
+msgstr "Innlogging"
 
 #: templates/two_factor/core/login.html:8
 msgid "Enter your credentials."
-msgstr "Введите логин и пароль"
+msgstr "Skriv inn innloggingsdetaljer"
 
 #: templates/two_factor/core/login.html:11
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "        digits you hear."
-msgstr "Мы совершаем звонок на ваш телефон, пожалуйста, введите цифры которые услышите."
+msgstr "Vi ringer telefonen din nå, skriv inn tallene du hører."
 
 #: templates/two_factor/core/login.html:14
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "        sent."
-msgstr "Мы отправили вам SMS, введите полученный токен."
+msgstr "Vi har sendt deg en SMS, skriv inn engangskoden vi sendte deg."
 
 #: templates/two_factor/core/login.html:17
 msgid ""
 "Please enter the tokens generated by your token\n"
 "        generator."
-msgstr "Введите токен предоставленный вашим генератором."
+msgstr "Skriv inn engangskoden fra kodegeneratoren din."
 
 #: templates/two_factor/core/login.html:21
 msgid ""
 "Use this form for entering backup tokens for logging in.\n"
 "      These tokens have been generated for you to print and keep safe. Please\n"
 "      enter one of these backup tokens to login to your account."
-msgstr "В процессе настройки вам было предложено сгенерировать резервные токены, распечатать и сохранить в надежном месте.\nСейчас введите один из этих токенов для входа в аккаунт."
+msgstr "Bruk dette skjemaet for å logge inn med reservekoder.\nDisse engangskodene har blitt generert for å skrives ut og oppbevares trygt. Skriv inn en av disse reservekodene for å logge inn."
 
 #: templates/two_factor/core/login.html:33
 msgid "Or, alternatively, use one of your backup phones:"
-msgstr "Или используйте один из резервных телефонов:"
+msgstr "Eller alternativt, bruk en av reservetelefonene dine:"
 
 #: templates/two_factor/core/login.html:43
 msgid "As a last resort, you can use a backup token:"
-msgstr "В крайнем случае, используйте резервный токен:"
+msgstr "I et nødstilfelle, kan du bruke en reservekode:"
 
 #: templates/two_factor/core/login.html:46
 #| msgid "Backup Tokens"
 msgid "Use Backup Token"
-msgstr "Использовать резервный токен"
+msgstr "Bruk reservekode"
 
 #: templates/two_factor/core/otp_required.html:5
 msgid "Permission Denied"
-msgstr "Доступ Запрещен"
+msgstr "Ingen adgang"
 
 #: templates/two_factor/core/otp_required.html:7
 msgid ""
 "The page you requested, enforces users to verify using\n"
 "    two-factor authentication for security reasons. You need to enable these\n"
 "    security features in order to access this page."
-msgstr "Запрошенная страница требует двухфакторной авторизации.\nДля продолжения, настройте ее использование в вашем профиле."
+msgstr "Siden vil besøke, krever av sikkerhetsgrunner at brukerene verifiseres med to-faktor-autentisering. Du må aktivere disse sikkerhetsfunksjonene for å få tilgang til denne siden."
 
 #: templates/two_factor/core/otp_required.html:11
 msgid ""
 "Two-factor authentication is not enabled for your\n"
 "    account. Enable two-factor authentication for enhanced account\n"
 "    security."
-msgstr "Двухфакторная авторизация не используется для вашего аккаунта.\nВключите двухфакторную авторизацию для повышения безопасности."
+msgstr "To-faktor-autentisering er ikke aktivert på din konto. Aktiver to-faktor-autentisering for bedre kontosikkerhet."
 
 #: templates/two_factor/core/otp_required.html:16
 msgid "Go back"
-msgstr "Назад"
+msgstr "Gå tilbake"
 
 #: templates/two_factor/core/otp_required.html:18
 #: templates/two_factor/core/setup.html:5
 #: templates/two_factor/core/setup_complete.html:5
 #: templates/two_factor/profile/profile.html:60
 msgid "Enable Two-Factor Authentication"
-msgstr "Включить Двухфакторную Аутентификацию"
+msgstr "Aktiver to-faktor-autentisering"
 
 #: templates/two_factor/core/phone_register.html:5
 msgid "Add Backup Phone"
-msgstr "Добавить резервный телефон"
+msgstr "Legg til reservetelefon"
 
 #: templates/two_factor/core/phone_register.html:8
 msgid ""
 "You'll be adding a backup phone number to your\n"
 "        account. This number will be used if your primary method of\n"
 "        registration is not available."
-msgstr "Вы добавляете резервный номер телефона к вашему аккаунту.\nЭтот номер будет использован если ваш первичный метод авторизации недоступен."
+msgstr "Du legger nå inn reserve-telefonnummer i kontoen din. Dette nummeret vil bli brukt hvis din primære registreringsmetode ikke er tilgjengelig."
 
 #: templates/two_factor/core/phone_register.html:12
 msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
-msgstr "Мы отправили токен авторизации на ваш телефон.\nВведите полученный токен."
+msgstr "Vi har sendt deg en engangskode til ditt telefonummer. Skriv inn koden du har mottatt."
 
 #: templates/two_factor/core/setup.html:7
 msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
-msgstr "Вы собираетесь повысить безопасность вашего аккаунта.\nСледуйте указаниям мастера для активации двухфакторной авторизации."
+msgstr "Du er i ferd med å ta kontosikkerheten til neste nivå. Følg trinnene i denne veiviseren for å aktivere to-faktor-autentisering."
 
 #: templates/two_factor/core/setup.html:11
 msgid ""
 "Please select which authentication method you would\n"
 "        like to use."
-msgstr "Выберите какой метод авторизации вы хотите использовать."
+msgstr "Velg hvilken autentiseringsmetode du vil bruke."
 
 #: templates/two_factor/core/setup.html:14
 msgid ""
 "To start using a token generator, please use your\n"
 "        smartphone to scan the QR code below. For example, use Google\n"
 "        Authenticator. Then, enter the token generated by the app.\n"
 "        "
-msgstr "Для начала использования генератора токенов, просканируйте QR-код ниже с помощью выбранного приложения (например, Google Authenticator).\nЗатем, введите полученный токен здесь."
+msgstr "For å begynne å bruke en kodegenerator, bruk smarttelefonen din til å scanne QR-koden nedenfor. Bruk f.eks. bruker Google Autentisering. Så kan du skrive inn koden som appen lager."
 
 #: templates/two_factor/core/setup.html:20
 msgid ""
 "Please enter the phone number you wish to receive the\n"
 "      text messages on. This number will be validated in the next step.\n"
 "      "
-msgstr ""
+msgstr "Skriv inn telefonnummeret du ønsker å motta SMS på. Dette nummeret vil valideres i neste trinn."
 
 #: templates/two_factor/core/setup.html:24
 msgid ""
 "Please enter the phone number you wish to be called on.\n"
 "      This number will be validated in the next step. "
-msgstr ""
+msgstr "Skriv inn telefonnummeret du vil at vi skal ringe. Nummeret vil bli validert i neste trinn."
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
 msgstr ""
 
@@ -304,153 +302,151 @@
 msgstr ""
 
 #: templates/two_factor/core/setup.html:43
 msgid ""
 "To identify and verify your YubiKey, please insert a\n"
 "      token in the field below. Your YubiKey will be linked to your\n"
 "      account."
-msgstr ""
+msgstr "For å verifisere din YubiKey, skriv inn en engangskode i feltet nedenfor. YubiKey'en vil så bli knyttet til din konto."
 
 #: templates/two_factor/core/setup_complete.html:7
 #| msgid ""
 #| "tulations, you've successfully enabled\n"
 #| "o-factor authentication."
 msgid ""
 "Congratulations, you've successfully enabled two-factor\n"
 "      authentication."
-msgstr "Поздравляем, Вы успешно активировали двухафакторную аутентификацию"
+msgstr "Gratulerer, du har nå aktivert to-faktor-autentisering."
 
 #: templates/two_factor/core/setup_complete.html:12
 #: templates/two_factor/core/setup_complete.html:19
 #| msgid "Back to profile"
 msgid "Back to Profile"
-msgstr "Вернуться в Профиль"
+msgstr "Tilbake til profil"
 
 #: templates/two_factor/core/setup_complete.html:14
 msgid ""
 "However, it might happen that you don't have access to\n"
 "      your primary token device. To enable account recovery, add a phone \n"
 "      number."
-msgstr ""
+msgstr "Det kan hende du ikke har tilgang til din primære kode-enhet. For å gjøre konto-gjennoppretting mulig, legg til et telefonnummer."
 
 #: templates/two_factor/core/setup_complete.html:21
 #: templates/two_factor/profile/profile.html:34
 msgid "Add Phone Number"
-msgstr "Добавьте номер телефон"
+msgstr "Legg til telefonummer"
 
 #: templates/two_factor/profile/disable.html:5
 msgid "Disable Two-factor Authentication"
-msgstr "Отключить Двухфакторную Аутентификацию"
+msgstr "Deaktiver to-faktor-autentisering"
 
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
 msgstr ""
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
-msgstr "Отключить"
+msgstr "Deaktiver"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
-msgstr "Безопасность"
+msgstr "Kontosikkerhet"
 
 #: templates/two_factor/profile/profile.html:9
 msgid "Tokens will be generated by your token generator."
-msgstr ""
+msgstr "Engangskoder vil bli laget av din kodegenerator."
 
 #: templates/two_factor/profile/profile.html:11
 #, python-format
 msgid "Primary method: %(primary)s"
-msgstr ""
+msgstr "Primærmetode:  %(primary)s"
 
 #: templates/two_factor/profile/profile.html:13
 #| msgid "Tokens will be generated by your token generator."
 msgid "Tokens will be generated by your YubiKey."
-msgstr ""
+msgstr "Engangskoder vil bli laget av din YubiKey."
 
 #: templates/two_factor/profile/profile.html:17
 msgid "Backup Phone Numbers"
-msgstr ""
+msgstr "Reserve-telefonnummere"
 
 #: templates/two_factor/profile/profile.html:18
 #| msgid ""
 #| "r primary method is not available, we are able to\n"
 #| "send backup tokens to the phone numbers listed below."
 msgid ""
 "If your primary method is not available, we are able to\n"
 "        send backup tokens to the phone numbers listed below."
 msgstr ""
 
 #: templates/two_factor/profile/profile.html:28
 msgid "Unregister"
-msgstr "Удалить регистрацию "
+msgstr "Avregistrer"
 
 #: templates/two_factor/profile/profile.html:39
 msgid ""
 "If you don't have any device with you, you can access\n"
 "        your account using backup tokens."
-msgstr ""
+msgstr "Hvis du ikke har noen enheter med deg, kan du komme inn i kontoen med reservekoder."
 
 #: templates/two_factor/profile/profile.html:41
 #, python-format
 msgid ""
 "\n"
 "        You have only one backup token remaining.\n"
 "      "
 msgid_plural ""
 "\n"
 "        You have %(counter)s backup tokens remaining.\n"
 "      "
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
+msgstr[0] "\n        Du har bare en reservekode igjen.\n\n      "
+msgstr[1] "\n        Du har %(counter)s reservekoder igjen.\n      "
 
 #: templates/two_factor/profile/profile.html:48
 msgid "Show Codes"
-msgstr ""
+msgstr "Vis koder"
 
 #: templates/two_factor/profile/profile.html:50
 #: templates/two_factor/profile/profile.html:54
 msgid "Disable Two-Factor Authentication"
-msgstr "Отключить Двухэтапную Аутентификацию"
+msgstr "Deaktiver to-faktor-autentisering"
 
 #: templates/two_factor/profile/profile.html:51
 msgid ""
 "However we strongly discourage you to do so, you can\n"
 "      also disable two-factor authentication for your account."
-msgstr ""
+msgstr "Vi fraråder på det sterkeste å gjøre dette, men du kan også deaktivere to-faktor-autentisering på kontoen din."
 
 #: templates/two_factor/profile/profile.html:56
 msgid ""
 "Two-factor authentication is not enabled for your\n"
 "      account. Enable two-factor authentication for enhanced account\n"
 "      security."
-msgstr ""
+msgstr "To-faktor-autentisering er ikke aktivert på kontoen din. Aktiver to-faktor-autentisering for bedre kontosikkerhet."
 
 #: templatetags/two_factor.py:56
 #, python-format
 msgid "Send text message to %s"
-msgstr "Отправка сообщения на номер: %s"
+msgstr "Send SMS til %s"
 
 #: templatetags/two_factor.py:58
 #, python-format
 msgid "Call number %s"
-msgstr "Звонок на номер: %s"
+msgstr "Ring nummer %s"
 
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
-msgstr "Пожалуйста введите верный телефонный номер, включая код страны, начинающиеся с + или 00"
+msgstr "Skriv inn et gyldig telefonnummer, inkludert landskoden som starter med + eller 00."
 
 #: views/utils.py:111
 msgid "ManagementForm data is missing or has been tampered."
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/he_IL/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/he_IL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/he_IL/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/he_IL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/hi_IN/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/hi_IN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ro/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/ro/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2018-08-06 14:39+0000\n"
+"Last-Translator: Bogdan Mateescu\n"
 "Language-Team: Romanian (http://www.transifex.com/Bouke/django-two-factor-"
 "auth/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
@@ -136,17 +136,27 @@
 msgid ""
 "If you don't have any device with you, you can access\n"
 "        your account using backup tokens."
 msgstr ""
 "Dacă nu aveți niciun dispozitiv la îndemână, vă puteți accesa\n"
 "        contul utilizând codurile de rezervă."
 
+msgid ""
+"If your primary method is not available, we are able to\n"
+"        send backup tokens to the phone numbers listed below."
+msgstr ""
+"Dacă metoda dvs. principală nu este disponibilă, vă vom putea\n"
+"      trimite codurile de rezervă la numerele de telefon listate mai jos."
+
 msgid "Login"
 msgstr "Conectare"
 
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "Datele din formularul de gestionare lipsesc sau au fost falsificate"
+
 msgid "Method"
 msgstr "Metoda"
 
 msgid "Next"
 msgstr "Înainte"
 
 msgid "Or, alternatively, use one of your backup phones:"
@@ -154,14 +164,17 @@
 
 msgid "Permission Denied"
 msgstr "Acces refuzat"
 
 msgid "Phone Call"
 msgstr "Apel telefonic"
 
+msgid "Phone Number"
+msgstr "Număr de telefon"
+
 msgid "Phone call"
 msgstr "Apel telefonic"
 
 msgid ""
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 msgstr ""
@@ -299,38 +312,77 @@
 "      Păstrați aceste coduri de rezervă într-un loc sigur, însă unde dvs. le "
 "puteți accesa ușor.\n"
 "      Te rugăm să introduci unul din aceste coduri de rezervă pentru a te "
 "conecta la contul tău."
 
 msgid ""
 "We are calling your phone right now, please enter the\n"
+"          digits you hear."
+msgstr ""
+"Vă sunăm pe telefon chiar acum, vă rugăm să introduceți\n"
+"        cifrele pe care le auziți."
+
+msgid ""
+"We are calling your phone right now, please enter the\n"
 "        digits you hear."
 msgstr ""
 "Vă sunăm pe telefon chiar acum, vă rugăm să introduceți\n"
 "        cifrele pe care le auziți."
 
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
+"          sent."
+msgstr ""
+"Un mesaj text cu un cod de verificare tocmai a fost\n"
+"        trimis."
+
+msgid ""
+"We sent you a text message, please enter the tokens we\n"
 "        sent."
 msgstr ""
 "Un mesaj text cu un cod de verificare tocmai a fost\n"
 "        trimis."
 
 msgid ""
+"We've\n"
+"        encountered an issue with the selected authentication method. "
+"Please\n"
+"        go back and verify that you entered your information correctly, try\n"
+"        again, or use a different authentication method instead. If the "
+"issue\n"
+"        persists, contact the site administrator."
+msgstr ""
+"Am\n"
+"        întâmpinat o problemă cu metoda de autentificare selectată. "
+"Reveniți\n"
+"        și verificați dacă ați introdus corect informațiile dvs., încercați\n"
+"        din nou, sau utilizați o metodă de autentificare diferită. Dacă "
+"problema\n"
+"        persistă, contactați administratorul site-ului."
+
+msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
 msgstr ""
 "Un mesaj text cu un cod de verificare a fost trimis către numărul dvs. de "
 "telefon.\n"
 "        Introduceți codul pe care l-ați primit."
 
 msgid "Yes, I am sure"
 msgstr "Da, sunt sigur"
 
 msgid ""
+"You are about to disable two-factor authentication. This\n"
+"    weakens your account security, are you sure?"
+msgstr ""
+"Sunteți pe cale să dezactivați verificarea în doi pași.\n"
+" Contul dvs. nu va mai beneficia de securitatea suplimentară\n"
+" și veți folosi numai parola pentru a vă conecta. Sunteți sigur?"
+
+msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
 msgstr ""
 "Sunteți pe cale să vă îmbunătățiți securitatea contului\n"
 "        Urmați pașii următori pentru a activa verificarea în doi\n"
 "        pași."
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ro/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/ro/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 # Translators:
 # Bogdan Mateescu, 2018
 # Bogdan Mateescu, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2018-08-06 14:39+0000\n"
+"Last-Translator: Bogdan Mateescu\n"
 "Language-Team: Romanian (http://www.transifex.com/Bouke/django-two-factor-auth/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
 msgstr "Metoda"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
-msgstr ""
+msgstr "Număr de telefon"
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
 msgstr "Cod de autentificare"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
@@ -104,15 +104,15 @@
 msgid "Text message"
 msgstr "Mesaj text"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Generator de coduri"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "metodă"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "Anulare"
 
@@ -281,30 +281,30 @@
 "      This number will be validated in the next step. "
 msgstr "Introduceți numărul de telefon pe care doriți să fiți apelat.\n      Acest număr va fi verificat în pasul următor."
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
-msgstr ""
+msgstr "Vă sunăm pe telefon chiar acum, vă rugăm să introduceți\n        cifrele pe care le auziți."
 
 #: templates/two_factor/core/setup.html:32
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "          sent."
-msgstr ""
+msgstr "Un mesaj text cu un cod de verificare tocmai a fost\n        trimis."
 
 #: templates/two_factor/core/setup.html:36
 msgid ""
 "We've\n"
 "        encountered an issue with the selected authentication method. Please\n"
 "        go back and verify that you entered your information correctly, try\n"
 "        again, or use a different authentication method instead. If the issue\n"
 "        persists, contact the site administrator."
-msgstr ""
+msgstr "Am\n        întâmpinat o problemă cu metoda de autentificare selectată. Reveniți\n        și verificați dacă ați introdus corect informațiile dvs., încercați\n        din nou, sau utilizați o metodă de autentificare diferită. Dacă problema\n        persistă, contactați administratorul site-ului."
 
 #: templates/two_factor/core/setup.html:43
 msgid ""
 "To identify and verify your YubiKey, please insert a\n"
 "      token in the field below. Your YubiKey will be linked to your\n"
 "      account."
 msgstr "Pentru a identifica și verifica dispozitivul dvs. YubiKey, introduceți un\n      cod în câmpul de mai jos. Dispozitivul dvs. YubiKey va fi legat de\n      contul dvs."
@@ -343,15 +343,15 @@
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
-msgstr ""
+msgstr "Sunteți pe cale să dezactivați verificarea în doi pași.\n Contul dvs. nu va mai beneficia de securitatea suplimentară\n și veți folosi numai parola pentru a vă conecta. Sunteți sigur?"
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
 msgstr "Dezactivați"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
@@ -378,15 +378,15 @@
 #: templates/two_factor/profile/profile.html:18
 #| msgid ""
 #| "r primary method is not available, we are able to\n"
 #| "send backup tokens to the phone numbers listed below."
 msgid ""
 "If your primary method is not available, we are able to\n"
 "        send backup tokens to the phone numbers listed below."
-msgstr ""
+msgstr "Dacă metoda dvs. principală nu este disponibilă, vă vom putea\n      trimite codurile de rezervă la numerele de telefon listate mai jos."
 
 #: templates/two_factor/profile/profile.html:28
 msgid "Unregister"
 msgstr "Anulați înregistrarea"
 
 #: templates/two_factor/profile/profile.html:39
 msgid ""
@@ -443,15 +443,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "Te rugăm să introduci un număr de telefon valid, inclusiv codul țarii dvs. începând cu + sau 00."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
-msgstr ""
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "Datele din formularul de gestionare lipsesc sau au fost falsificate"
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-05-17 20:13+0000\n"
+"Last-Translator: phui chen <phui.chen@gmail.com>\n"
 "Language-Team: Chinese (China) (http://www.transifex.com/Bouke/django-two-"
 "factor-auth/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -134,14 +134,17 @@
 
 msgid "Permission Denied"
 msgstr "拒绝访问"
 
 msgid "Phone Call"
 msgstr "电话呼叫"
 
+msgid "Phone Number"
+msgstr "电话号码"
+
 msgid "Phone call"
 msgstr "电话呼叫"
 
 msgid ""
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 msgstr "请输入一个有效的电话号码，包含以 + 或 00 开头的国家区号。"
@@ -252,19 +255,29 @@
 msgstr ""
 "使用这个用备用验证码登录的表单。\n"
 "这些验证码曾经为您生成过，并且您已经将它们保存在安全的地方了。\n"
 "请从这些验证码中随便输入一个用来登录您的账户。"
 
 msgid ""
 "We are calling your phone right now, please enter the\n"
+"          digits you hear."
+msgstr "我们现在就将给您致电，请输入您所听到的数字。"
+
+msgid ""
+"We are calling your phone right now, please enter the\n"
 "        digits you hear."
 msgstr "我们现在就呼叫您的电话，请输入您所听到的数字。"
 
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
+"          sent."
+msgstr "我们已经给您发了一条短信，请输入我们发送的验证码。"
+
+msgid ""
+"We sent you a text message, please enter the tokens we\n"
 "        sent."
 msgstr "我们已经给您发了一条短信，请输入我们发送的验证码。"
 
 msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
 msgstr "我们已经将验证码发送到您的电话号码了。请输入您所收到的验证码。"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/zh_CN/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
 # mozillazg <opensource.mozillazg@gmail.com>, 2014
+# phui chen <phui.chen@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-05-17 20:13+0000\n"
+"Last-Translator: phui chen <phui.chen@gmail.com>\n"
 "Language-Team: Chinese (China) (http://www.transifex.com/Bouke/django-two-factor-auth/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
 msgstr "方法"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
-msgstr ""
+msgstr "电话号码"
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
 msgstr "验证码"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
@@ -103,15 +104,15 @@
 msgid "Text message"
 msgstr "短信"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "验证码生成器"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "方法"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "取消"
 
@@ -280,21 +281,21 @@
 "      This number will be validated in the next step. "
 msgstr "请输入您想被呼叫的电话号码。这个号码将在下一步被验证。"
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
-msgstr ""
+msgstr "我们现在就将给您致电，请输入您所听到的数字。"
 
 #: templates/two_factor/core/setup.html:32
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "          sent."
-msgstr ""
+msgstr "我们已经给您发了一条短信，请输入我们发送的验证码。"
 
 #: templates/two_factor/core/setup.html:36
 msgid ""
 "We've\n"
 "        encountered an issue with the selected authentication method. Please\n"
 "        go back and verify that you entered your information correctly, try\n"
 "        again, or use a different authentication method instead. If the issue\n"
@@ -440,15 +441,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "请输入一个有效的电话号码，包含以 + 或 00 开头的国家区号。"
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
+msgid "ManagementForm data is missing or has been tampered with"
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/hu_HU/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/hu_HU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/en_GB/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/en_GB/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/en_GB/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ar/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/ar/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-01-15 02:03+0000\n"
+"Last-Translator: Anwar Allawi <yuri.wolf.vlas@gmail.com>\n"
 "Language-Team: Arabic (http://www.transifex.com/Bouke/django-two-factor-auth/"
 "language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
@@ -303,37 +303,69 @@
 msgstr ""
 "استخدم هذه نموذج لإدخال رمز التفويض الاحتياطي لتسجيل الدخول.\n"
 "      رموز التفويض هذه تم إنشاؤها ليتم طباعتها و الاحتفاظ بها بمكان آمن. "
 "الرجاء إدخال أحد رموز التفويض الإحتياطية للدخول لحسابك."
 
 msgid ""
 "We are calling your phone right now, please enter the\n"
+"          digits you hear."
+msgstr ""
+"يتم الان الاتصال على رقم الهاتف الخاص بك, الرجاء ادخال الارقام التي يتم "
+"سماعها."
+
+msgid ""
+"We are calling your phone right now, please enter the\n"
 "        digits you hear."
 msgstr ""
 "جاري الإتصال بكم الآن, الرجاء إدخال\n"
 "الأرقام التي تسمعها عبر الإتصال."
 
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
+"          sent."
+msgstr "قمنا بأرسال رسالة نصية الى هاتفك, الرجاء ادخال الرمز المرسل."
+
+msgid ""
+"We sent you a text message, please enter the tokens we\n"
 "        sent."
 msgstr ""
 "تم إرسال الرسالة النصية لكم, الرجاء إدخال رمز التفويض المرسل\n"
 "لكم."
 
 msgid ""
+"We've\n"
+"        encountered an issue with the selected authentication method. "
+"Please\n"
+"        go back and verify that you entered your information correctly, try\n"
+"        again, or use a different authentication method instead. If the "
+"issue\n"
+"        persists, contact the site administrator."
+msgstr ""
+"واجهنا مشكلة مع طريقة المصادقة المحددة. الرجاء الرجوع و التحقق من صحة "
+"البيانات المدخلة, حاول مرة اخرى, او استخدم طريقة مصادقة اخرى عوضا. اذا "
+"استمرت المشكلة, قم بمراسلة مسؤول الموقع."
+
+msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
 msgstr ""
 "تم إرسال رمز تفويض لرقم هاتفكم. الرجاء\n"
 "إدخال رمز التفويض الذي وصل لكم."
 
 msgid "Yes, I am sure"
 msgstr "نعم, أنا متأكد"
 
 msgid ""
+"You are about to disable two-factor authentication. This\n"
+"    weakens your account security, are you sure?"
+msgstr ""
+"انت على وشك ايقاف التوثيق ذو العاملين. هذا الاختيار سيضعف من امان حسابك, هل "
+"انت متأكد؟"
+
+msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
 msgstr ""
 "أنت بصدد ترقية أمان حسابك\n"
 "للمستوى التالي. الرجاء إتباع الخطوات التالية لتفعيل خاصية التحقق من\n"
 "خطوتين."
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ar/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/ar/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
+# Anwar Allawi <yuri.wolf.vlas@gmail.com>, 2019
 # Bashar Al-Abdulhadi, 2013-2014
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-01-15 02:03+0000\n"
+"Last-Translator: Anwar Allawi <yuri.wolf.vlas@gmail.com>\n"
 "Language-Team: Arabic (http://www.transifex.com/Bouke/django-two-factor-auth/language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
@@ -103,15 +104,15 @@
 msgid "Text message"
 msgstr "رسالة نصية"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "منشئ رمز التفويض"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "الطريقة"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "إلغاء"
 
@@ -280,30 +281,30 @@
 "      This number will be validated in the next step. "
 msgstr "الرجاء إدخال رقم الهاتف الذي ترغب بإستلام\nالمكالمة عليه. سيتم التحقق من الرقم بالخطوة التالية."
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
-msgstr ""
+msgstr "يتم الان الاتصال على رقم الهاتف الخاص بك, الرجاء ادخال الارقام التي يتم سماعها."
 
 #: templates/two_factor/core/setup.html:32
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "          sent."
-msgstr ""
+msgstr "قمنا بأرسال رسالة نصية الى هاتفك, الرجاء ادخال الرمز المرسل."
 
 #: templates/two_factor/core/setup.html:36
 msgid ""
 "We've\n"
 "        encountered an issue with the selected authentication method. Please\n"
 "        go back and verify that you entered your information correctly, try\n"
 "        again, or use a different authentication method instead. If the issue\n"
 "        persists, contact the site administrator."
-msgstr ""
+msgstr "واجهنا مشكلة مع طريقة المصادقة المحددة. الرجاء الرجوع و التحقق من صحة البيانات المدخلة, حاول مرة اخرى, او استخدم طريقة مصادقة اخرى عوضا. اذا استمرت المشكلة, قم بمراسلة مسؤول الموقع."
 
 #: templates/two_factor/core/setup.html:43
 msgid ""
 "To identify and verify your YubiKey, please insert a\n"
 "      token in the field below. Your YubiKey will be linked to your\n"
 "      account."
 msgstr "ليتم التعرف و التحقق من مفتاح YubiKey الخاص بك, الرجاء أدخل\n      رمز تفويض في الحقل أدناه. مفتاح YubiKey الخاص بك سيتم ربطة\n      بحسابك."
@@ -342,15 +343,15 @@
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
-msgstr ""
+msgstr "انت على وشك ايقاف التوثيق ذو العاملين. هذا الاختيار سيضعف من امان حسابك, هل انت متأكد؟"
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
 msgstr "تعطيل"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
@@ -445,15 +446,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "يرجى إدخال رقم هاتف صحيح، بما في ذلك رمز البلد الخاص بدءا بـ + أو 00."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
+msgid "ManagementForm data is missing or has been tampered with"
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/nl/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/nl/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:39+0000\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-07-07 06:31+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
 "Language-Team: Dutch (http://www.transifex.com/Bouke/django-two-factor-auth/"
 "language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl\n"
@@ -133,14 +133,17 @@
 msgstr ""
 "Wanneer je primaire methode niet beschikbaar is, kunnen we tokens naar de "
 "onderstaande telefoonnummers sturen."
 
 msgid "Login"
 msgstr "Inloggen"
 
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "ManagementForm gegevens missen of zijn mee geknoeid"
+
 msgid "Method"
 msgstr "Methode"
 
 msgid "Next"
 msgstr "Volgende"
 
 msgid "Or, alternatively, use one of your backup phones:"
@@ -317,16 +320,16 @@
 "authenticatiemethode. Als het probleem blijft aanhouden, neem dan contact op "
 "met de sitebeheerder."
 
 msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
 msgstr ""
-"We heb een token verzonden naar jouw telefoonnummer. Voer het token dat je "
-"hebt ontvangen."
+"We heb een token verzonden naar jouw telefoonnummer. Voer het token in dat "
+"je hebt ontvangen."
 
 msgid "Yes, I am sure"
 msgstr "Ja, ik weet het zeker"
 
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/nl/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
-# Bouke Haarsma <bouke@haarsma.eu>, 2018
+# Bouke Haarsma <bouke@haarsma.eu>, 2018-2019
 # Bouke Haarsma <bouke@haarsma.eu>, 2013-2014
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:39+0000\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-07-07 06:31+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
 "Language-Team: Dutch (http://www.transifex.com/Bouke/django-two-factor-auth/language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -104,15 +104,15 @@
 msgid "Text message"
 msgstr "SMS-bericht"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Tokengenerator"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "methode"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "Annuleren"
 
@@ -241,15 +241,15 @@
 "        registration is not available."
 msgstr "Je gaat een alternatief telefoonnummer aan je account toevoegen. Dit nummer wordt gebruikt als uw primaire token niet beschikbaar is."
 
 #: templates/two_factor/core/phone_register.html:12
 msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
-msgstr "We heb een token verzonden naar jouw telefoonnummer. Voer het token dat je hebt ontvangen."
+msgstr "We heb een token verzonden naar jouw telefoonnummer. Voer het token in dat je hebt ontvangen."
 
 #: templates/two_factor/core/setup.html:7
 msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
 msgstr "Je staat op het punt om je accountbeveiliging naar het volgende niveau te tillen. Volg de stappen in deze wizard om tweestapsauthenticatie in te schakelen."
@@ -442,15 +442,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "Voer een geldig telefoonnummer in, inclusief landcode en begin met + of 00."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
-msgstr ""
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "ManagementForm gegevens missen of zijn mee geknoeid"
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/nb/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/nb/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/da_DK/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,288 +1,288 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
-# Stein Strindhaug <stein.strindhaug@gmail.com>, 2017
+# valberg <valberg@orn.li>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-08-03 15:23+0200\n"
 "PO-Revision-Date: 2018-08-03 13:23+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
-"Language-Team: Norwegian Bokmål (http://www.transifex.com/Bouke/django-two-factor-auth/language/nb/)\n"
+"Language-Team: Danish (Denmark) (http://www.transifex.com/Bouke/django-two-factor-auth/language/da_DK/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nb\n"
+"Language: da_DK\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
 msgstr "Metode"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
 msgstr ""
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
-msgstr "Engangskode"
+msgstr "Kode"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
 msgid "Entered token is not valid."
-msgstr "Engangskoden er ugyldig"
+msgstr "Den indtastet kode er ikke gyldig."
 
 #: forms.py:76 forms.py:170 models.py:42
 msgid "YubiKey"
 msgstr "YubiKey"
 
 #: forms.py:79
 msgid "The YubiKey could not be verified."
-msgstr "Kunne ikke verifisere YubiKey'en."
+msgstr "YubiKey kunne ikke verificeres."
 
 #: forms.py:138
 msgid "Yes, I am sure"
 msgstr "Ja, jeg er sikker"
 
 #: gateways/twilio/gateway.py:61
 #, python-format
 msgid "Your authentication token is %s"
-msgstr "Auteniseringskoden din er %s"
+msgstr "Din autentifikationskode er %s"
 
 #. Translators: twilio_locale should be a locale supported by
 #. Twilio, see http://bit.ly/187I5cr
 #: gateways/twilio/gateway.py:70 gateways/twilio/views.py:74
 msgctxt "twilio_locale"
 msgid "en"
-msgstr "nb-NO"
+msgstr "en"
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:39
 #, python-format
 #| msgid ""
 #| "is is %(site_name)s calling. Please enter the following code on r "
 #| "screen:token)s. Repeat: %(token)s."
 msgid "Hi, this is %(site_name)s calling. Press any key to continue."
-msgstr "Hei, dette er %(site_name)s som ringer. Trykk en tast for å fortsette."
+msgstr "Hej, dette er %(site_name)s. Tryk på en vilkårlig knap for at fortsætte."
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:44
 #, python-format
 msgid "Your token is %(token)s. Repeat: %(token)s. Good bye."
-msgstr "Din kode er %(token)s. Jeg gjentar: %(token)s. Ha det."
+msgstr "Din token er %(token)s. Repeat: %(token)s. Farvel."
 
 #. Translators: should be a language supported by Twilio,
 #. see http://bit.ly/187I5cr
 #: gateways/twilio/views.py:48
 #| msgid "You don't have any backup codes yet."
 msgid "You didn't press any keys. Good bye."
-msgstr "Du trykket ikke noen tast. Ha det."
+msgstr "Du trykkede ikke på nogen taster. Farvel."
 
 #: models.py:25
 msgid "Phone Call"
-msgstr "Telefonsamtale"
+msgstr "Telefonopkald"
 
 #: models.py:26
 msgid "Text Message"
-msgstr "SMS"
+msgstr "Tekstbesked"
 
 #: models.py:33
 #| msgid "Phone Call"
 msgid "Phone call"
-msgstr "Telefonsamtale"
+msgstr "Telefonopkald"
 
 #: models.py:35
 #| msgid "Text Message"
 msgid "Text message"
-msgstr "SMS"
+msgstr "Tekstbesked"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Kodegenerator"
 
 #: models.py:71
 msgid "method"
 msgstr "metode"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Annuller"
 
 #: templates/two_factor/_wizard_actions.html:10
 #: templates/two_factor/_wizard_actions.html:13
 msgid "Back"
-msgstr "Tilbake"
+msgstr "Tilbage"
 
 #: templates/two_factor/_wizard_actions.html:15
 msgid "Next"
-msgstr "Neste"
+msgstr "Næste"
 
 #: templates/two_factor/core/backup_tokens.html:5
 #: templates/two_factor/profile/profile.html:37
 msgid "Backup Tokens"
-msgstr "Reserve-koder"
+msgstr "Backupkoder"
 
 #: templates/two_factor/core/backup_tokens.html:6
 msgid ""
 "Backup tokens can be used when your primary and backup\n"
 "      phone numbers aren't available. The backup tokens below can be used\n"
 "      for login verification. If you've used up all your backup tokens, you\n"
 "      can generate a new set of backup tokens. Only the backup tokens shown\n"
 "      below will be valid."
-msgstr "Reservekoder kan brukes når hoved og reserve telefonnummeret ditt ikke er tilgjengelig. Reservekodene nedenfor kan benyttes for innloggingsverifikasjon. Hivs du har brukt opp alle reservekodene kan du generere et nytt sett med koder. Bare reservekodene vist nedenfor vil være gyldige."
+msgstr "Backupkoder kan bruges når din primære og backup telefonnumre ikke er tilgængelige. De backupkoder listet herunder kan bruges til login verifikation. Hvis du har brugt alle dine backupkoder, kan du generere et nyt sæt koder. Kun de backupkoder der er listet herunder er gyldige."
 
 #: templates/two_factor/core/backup_tokens.html:18
 msgid "Print these tokens and keep them somewhere safe."
-msgstr "Skriv ut disse kodene og oppbevar dem et trygt sted."
+msgstr "Print disse tokens ud og gem dem et sikkert sted."
 
 #: templates/two_factor/core/backup_tokens.html:20
 msgid "You don't have any backup codes yet."
-msgstr "Du har ikke noen reservekoder ennå."
+msgstr "Du har ikke nogen backup koder endnu."
 
 #: templates/two_factor/core/backup_tokens.html:25
 msgid "Back to Account Security"
-msgstr "Tilbake til kontosikkerhet"
+msgstr "Tilbage til Konto Sikkerhed"
 
 #: templates/two_factor/core/backup_tokens.html:26
 msgid "Generate Tokens"
-msgstr "Lag engangskoder"
+msgstr "Generér Koder"
 
 #: templates/two_factor/core/login.html:5
 msgid "Login"
-msgstr "Innlogging"
+msgstr "Login"
 
 #: templates/two_factor/core/login.html:8
 msgid "Enter your credentials."
-msgstr "Skriv inn innloggingsdetaljer"
+msgstr "Indtast dine logininformationer"
 
 #: templates/two_factor/core/login.html:11
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "        digits you hear."
-msgstr "Vi ringer telefonen din nå, skriv inn tallene du hører."
+msgstr "Vi er i gang med at ringe til din telefon nu. Indtast venligst de tal du hører."
 
 #: templates/two_factor/core/login.html:14
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "        sent."
-msgstr "Vi har sendt deg en SMS, skriv inn engangskoden vi sendte deg."
+msgstr "Vi har sendt dig en tekstbesked. Indtast venligst de koder vi har sendt."
 
 #: templates/two_factor/core/login.html:17
 msgid ""
 "Please enter the tokens generated by your token\n"
 "        generator."
-msgstr "Skriv inn engangskoden fra kodegeneratoren din."
+msgstr "Indtast venligst koder genereret af din kodegenerator."
 
 #: templates/two_factor/core/login.html:21
 msgid ""
 "Use this form for entering backup tokens for logging in.\n"
 "      These tokens have been generated for you to print and keep safe. Please\n"
 "      enter one of these backup tokens to login to your account."
-msgstr "Bruk dette skjemaet for å logge inn med reservekoder.\nDisse engangskodene har blitt generert for å skrives ut og oppbevares trygt. Skriv inn en av disse reservekodene for å logge inn."
+msgstr "Brug denne formular for at indtaste backupkoder for at logge ind.\nIndtast venligst en af disse backupkoder for at logge ind på din konto."
 
 #: templates/two_factor/core/login.html:33
 msgid "Or, alternatively, use one of your backup phones:"
-msgstr "Eller alternativt, bruk en av reservetelefonene dine:"
+msgstr "Eller, alternativt, brug en af dine backuptelefoner:"
 
 #: templates/two_factor/core/login.html:43
 msgid "As a last resort, you can use a backup token:"
-msgstr "I et nødstilfelle, kan du bruke en reservekode:"
+msgstr "Som sidste udvej, kan du bruge en backupkode:"
 
 #: templates/two_factor/core/login.html:46
 #| msgid "Backup Tokens"
 msgid "Use Backup Token"
-msgstr "Bruk reservekode"
+msgstr "Brug Backupkode"
 
 #: templates/two_factor/core/otp_required.html:5
 msgid "Permission Denied"
-msgstr "Ingen adgang"
+msgstr "Adgang nægtet"
 
 #: templates/two_factor/core/otp_required.html:7
 msgid ""
 "The page you requested, enforces users to verify using\n"
 "    two-factor authentication for security reasons. You need to enable these\n"
 "    security features in order to access this page."
-msgstr "Siden vil besøke, krever av sikkerhetsgrunner at brukerene verifiseres med to-faktor-autentisering. Du må aktivere disse sikkerhetsfunksjonene for å få tilgang til denne siden."
+msgstr "Den side du forsøger at tilgå kræver at du, grundet sikkerhedshensyn, er verificeret ved hjælp af to-faktor autentifikation . Du skal aktivere disse sikkerhedselementer for at få adgang til denne side."
 
 #: templates/two_factor/core/otp_required.html:11
 msgid ""
 "Two-factor authentication is not enabled for your\n"
 "    account. Enable two-factor authentication for enhanced account\n"
 "    security."
-msgstr "To-faktor-autentisering er ikke aktivert på din konto. Aktiver to-faktor-autentisering for bedre kontosikkerhet."
+msgstr "To-faktor autentifikation er ikke aktiveret for din konto. Aktivér to-faktor autentifikation for forøget kontosikkerhed."
 
 #: templates/two_factor/core/otp_required.html:16
 msgid "Go back"
-msgstr "Gå tilbake"
+msgstr "Gå tilbage"
 
 #: templates/two_factor/core/otp_required.html:18
 #: templates/two_factor/core/setup.html:5
 #: templates/two_factor/core/setup_complete.html:5
 #: templates/two_factor/profile/profile.html:60
 msgid "Enable Two-Factor Authentication"
-msgstr "Aktiver to-faktor-autentisering"
+msgstr "Aktivér To-Faktor Autentifaktion"
 
 #: templates/two_factor/core/phone_register.html:5
 msgid "Add Backup Phone"
-msgstr "Legg til reservetelefon"
+msgstr "Tilføj Backup Telefon"
 
 #: templates/two_factor/core/phone_register.html:8
 msgid ""
 "You'll be adding a backup phone number to your\n"
 "        account. This number will be used if your primary method of\n"
 "        registration is not available."
-msgstr "Du legger nå inn reserve-telefonnummer i kontoen din. Dette nummeret vil bli brukt hvis din primære registreringsmetode ikke er tilgjengelig."
+msgstr "Du er i gang med at tilføje et telefonnummer til din konto. Dette nummer vil blive brugt hvis din primære metode til registrering ikke er tilgængelig."
 
 #: templates/two_factor/core/phone_register.html:12
 msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
-msgstr "Vi har sendt deg en engangskode til ditt telefonummer. Skriv inn koden du har mottatt."
+msgstr "Vi har sendt en kode til dit telefonnummer. Indtast venligst den kode du har modtaget."
 
 #: templates/two_factor/core/setup.html:7
 msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
-msgstr "Du er i ferd med å ta kontosikkerheten til neste nivå. Følg trinnene i denne veiviseren for å aktivere to-faktor-autentisering."
+msgstr "Du er nu i gang med at ophøje sikkerheden på din konto. Følg skridtene i denne guide for at aktivere to-faktor autentifikation."
 
 #: templates/two_factor/core/setup.html:11
 msgid ""
 "Please select which authentication method you would\n"
 "        like to use."
-msgstr "Velg hvilken autentiseringsmetode du vil bruke."
+msgstr "Vælg venligst hvilken autentifikationsmetode du vil anvende."
 
 #: templates/two_factor/core/setup.html:14
 msgid ""
 "To start using a token generator, please use your\n"
 "        smartphone to scan the QR code below. For example, use Google\n"
 "        Authenticator. Then, enter the token generated by the app.\n"
 "        "
-msgstr "For å begynne å bruke en kodegenerator, bruk smarttelefonen din til å scanne QR-koden nedenfor. Bruk f.eks. bruker Google Autentisering. Så kan du skrive inn koden som appen lager."
+msgstr "For at benytte en kodegenerator, brug venligst din smartphone til at skanne QR koden herunder. Brug for eksempel Google Authenticator. Indtast derefter den kode som appen genererer."
 
 #: templates/two_factor/core/setup.html:20
 msgid ""
 "Please enter the phone number you wish to receive the\n"
 "      text messages on. This number will be validated in the next step.\n"
 "      "
-msgstr "Skriv inn telefonnummeret du ønsker å motta SMS på. Dette nummeret vil valideres i neste trinn."
+msgstr "Indtast venligst det telefonnummer du ønsker at modtage tekstbeskederne på. Dette nummer vil blive verificeret i næste skridt."
 
 #: templates/two_factor/core/setup.html:24
 msgid ""
 "Please enter the phone number you wish to be called on.\n"
 "      This number will be validated in the next step. "
-msgstr "Skriv inn telefonnummeret du vil at vi skal ringe. Nummeret vil bli validert i neste trinn."
+msgstr "Indtast venligst det telefonnummer du ønsker at blive ringer op på. Dette nummer vil blive verificeret i næste skridt."
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
 msgstr ""
 
@@ -302,46 +302,46 @@
 msgstr ""
 
 #: templates/two_factor/core/setup.html:43
 msgid ""
 "To identify and verify your YubiKey, please insert a\n"
 "      token in the field below. Your YubiKey will be linked to your\n"
 "      account."
-msgstr "For å verifisere din YubiKey, skriv inn en engangskode i feltet nedenfor. YubiKey'en vil så bli knyttet til din konto."
+msgstr "For at identificere og verificere din YubiKey, indsæt venligst en kode i feltet nedenunder. Din YubiKey vil blive forbundet med din konto."
 
 #: templates/two_factor/core/setup_complete.html:7
 #| msgid ""
 #| "tulations, you've successfully enabled\n"
 #| "o-factor authentication."
 msgid ""
 "Congratulations, you've successfully enabled two-factor\n"
 "      authentication."
-msgstr "Gratulerer, du har nå aktivert to-faktor-autentisering."
+msgstr "Tillykke, du har nu aktiveret to-faktor autentifikation."
 
 #: templates/two_factor/core/setup_complete.html:12
 #: templates/two_factor/core/setup_complete.html:19
 #| msgid "Back to profile"
 msgid "Back to Profile"
-msgstr "Tilbake til profil"
+msgstr "Tilbage til Profil"
 
 #: templates/two_factor/core/setup_complete.html:14
 msgid ""
 "However, it might happen that you don't have access to\n"
 "      your primary token device. To enable account recovery, add a phone \n"
 "      number."
-msgstr "Det kan hende du ikke har tilgang til din primære kode-enhet. For å gjøre konto-gjennoppretting mulig, legg til et telefonnummer."
+msgstr "Det kan dog forekomme at du ikke har adgang til dit primære kodeenhed. For at aktivere kontogendannelse, tilføj et telefonnummer."
 
 #: templates/two_factor/core/setup_complete.html:21
 #: templates/two_factor/profile/profile.html:34
 msgid "Add Phone Number"
-msgstr "Legg til telefonummer"
+msgstr "Tilføj Telefonnummer"
 
 #: templates/two_factor/profile/disable.html:5
 msgid "Disable Two-factor Authentication"
-msgstr "Deaktiver to-faktor-autentisering"
+msgstr "Deaktivér To-Faktor Autentifaktion"
 
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
@@ -350,103 +350,103 @@
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
 msgstr "Deaktiver"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
-msgstr "Kontosikkerhet"
+msgstr "Kontosikkerhed"
 
 #: templates/two_factor/profile/profile.html:9
 msgid "Tokens will be generated by your token generator."
-msgstr "Engangskoder vil bli laget av din kodegenerator."
+msgstr "Koder vil blive genereret af din kodegenerator."
 
 #: templates/two_factor/profile/profile.html:11
 #, python-format
 msgid "Primary method: %(primary)s"
-msgstr "Primærmetode:  %(primary)s"
+msgstr "Primære metode: %(primary)s"
 
 #: templates/two_factor/profile/profile.html:13
 #| msgid "Tokens will be generated by your token generator."
 msgid "Tokens will be generated by your YubiKey."
-msgstr "Engangskoder vil bli laget av din YubiKey."
+msgstr "Koder vil blive genereret af din YubiKey."
 
 #: templates/two_factor/profile/profile.html:17
 msgid "Backup Phone Numbers"
-msgstr "Reserve-telefonnummere"
+msgstr "Backup telefonnumre"
 
 #: templates/two_factor/profile/profile.html:18
 #| msgid ""
 #| "r primary method is not available, we are able to\n"
 #| "send backup tokens to the phone numbers listed below."
 msgid ""
 "If your primary method is not available, we are able to\n"
 "        send backup tokens to the phone numbers listed below."
 msgstr ""
 
 #: templates/two_factor/profile/profile.html:28
 msgid "Unregister"
-msgstr "Avregistrer"
+msgstr "Afmeld"
 
 #: templates/two_factor/profile/profile.html:39
 msgid ""
 "If you don't have any device with you, you can access\n"
 "        your account using backup tokens."
-msgstr "Hvis du ikke har noen enheter med deg, kan du komme inn i kontoen med reservekoder."
+msgstr "Hvis du ikke har nogen enhed med dig, kan du tilgå din konto ved brug af backupkoder."
 
 #: templates/two_factor/profile/profile.html:41
 #, python-format
 msgid ""
 "\n"
 "        You have only one backup token remaining.\n"
 "      "
 msgid_plural ""
 "\n"
 "        You have %(counter)s backup tokens remaining.\n"
 "      "
-msgstr[0] "\n        Du har bare en reservekode igjen.\n\n      "
-msgstr[1] "\n        Du har %(counter)s reservekoder igjen.\n      "
+msgstr[0] "\n        Du har kun én backupkode tilbage.\n\n      "
+msgstr[1] "\n        Du har %(counter)s backupkoder tilbage.\n      "
 
 #: templates/two_factor/profile/profile.html:48
 msgid "Show Codes"
-msgstr "Vis koder"
+msgstr "Vis Koder"
 
 #: templates/two_factor/profile/profile.html:50
 #: templates/two_factor/profile/profile.html:54
 msgid "Disable Two-Factor Authentication"
-msgstr "Deaktiver to-faktor-autentisering"
+msgstr "Deaktivér To-Faktor Autentifaktion"
 
 #: templates/two_factor/profile/profile.html:51
 msgid ""
 "However we strongly discourage you to do so, you can\n"
 "      also disable two-factor authentication for your account."
-msgstr "Vi fraråder på det sterkeste å gjøre dette, men du kan også deaktivere to-faktor-autentisering på kontoen din."
+msgstr "Selvom vi stærkt fraråder det, kan du også deaktivere to-faktor autentifikation for din konto."
 
 #: templates/two_factor/profile/profile.html:56
 msgid ""
 "Two-factor authentication is not enabled for your\n"
 "      account. Enable two-factor authentication for enhanced account\n"
 "      security."
-msgstr "To-faktor-autentisering er ikke aktivert på kontoen din. Aktiver to-faktor-autentisering for bedre kontosikkerhet."
+msgstr "To-faktor autentifikation er ikke aktiveret for din konto. Aktivér to-faktor autentifikation for forøget kontosikkerhed."
 
 #: templatetags/two_factor.py:56
 #, python-format
 msgid "Send text message to %s"
-msgstr "Send SMS til %s"
+msgstr "Send tekstbesked til %s"
 
 #: templatetags/two_factor.py:58
 #, python-format
 msgid "Call number %s"
-msgstr "Ring nummer %s"
+msgstr "Ring %s"
 
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
-msgstr "Skriv inn et gyldig telefonnummer, inkludert landskoden som starter med + eller 00."
+msgstr "Venligst indtast et gyldigt telefonnummer inkl. landekode startende med + eller 00"
 
 #: views/utils.py:111
 msgid "ManagementForm data is missing or has been tampered."
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/de/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/de/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/as/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/as/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/ca_ES/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/ca_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/fi/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/fi/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2018-10-16 18:09+0000\n"
+"Last-Translator: Mika Mäkelä <mika.m.makela@gmail.com>\n"
 "Language-Team: Finnish (http://www.transifex.com/Bouke/django-two-factor-"
 "auth/language/fi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -143,14 +143,17 @@
 
 msgid "Permission Denied"
 msgstr "Lupa evätty"
 
 msgid "Phone Call"
 msgstr "Puhelinsoitto"
 
+msgid "Phone Number"
+msgstr "Puhelinnumero"
+
 msgid "Phone call"
 msgstr "Puhelinsoitto"
 
 msgid ""
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 msgstr ""
@@ -228,15 +231,15 @@
 msgstr ""
 "Aloittaaksesi tunnusgeneraattorin käytön,\n"
 "aloita skannaamalla alla oleva QR-koodi.\n"
 "Käytä esimerkiksi Google Authenticatoria.\n"
 "Syötä tämän jälkeen saamasi koodi."
 
 msgid "Token"
-msgstr "Tunnu"
+msgstr "Tunnus"
 
 msgid "Token generator"
 msgstr "Tunnusgeneraattori"
 
 msgid "Tokens will be generated by your YubiKey."
 msgstr "Tunnukset luodaan YubiKeyllasi"
 
@@ -298,14 +301,21 @@
 "Olemme lähettäneet sinulle tunnuksen \n"
 "puhelinnumeroosi. Syötä saamasi tunnus."
 
 msgid "Yes, I am sure"
 msgstr "Kyllä, olen varma."
 
 msgid ""
+"You are about to disable two-factor authentication. This\n"
+"    weakens your account security, are you sure?"
+msgstr ""
+"Olet poistamassa kaksivaiheisen tunnistautumisen. Tämä heikentää tilisi "
+"turvallisuutta. Haluatko varmasti poistaa?"
+
+msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
 msgstr ""
 "Olet parantamassa tilisi tietoturvaa. Seuraa tämän ohjeen\n"
 "askelia ottaaksesi kaksivaiheisen tunnistautumisen käyttöön."
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/fi/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
 # Aleksi Häkli <aleksi.hakli@iki.fi>, 2016
+# Mika Mäkelä <mika.m.makela@gmail.com>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2018-10-16 18:09+0000\n"
+"Last-Translator: Mika Mäkelä <mika.m.makela@gmail.com>\n"
 "Language-Team: Finnish (http://www.transifex.com/Bouke/django-two-factor-auth/language/fi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
 msgstr "Tapa"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
-msgstr ""
+msgstr "Puhelinnumero"
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
-msgstr "Tunnu"
+msgstr "Tunnus"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
 msgid "Entered token is not valid."
 msgstr "Syötetty tunnus ei ole voimassa."
 
 #: forms.py:76 forms.py:170 models.py:42
@@ -103,15 +104,15 @@
 msgid "Text message"
 msgstr "Tekstiviesti"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Tunnusgeneraattori"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "tapa"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "Peruuta"
 
@@ -342,15 +343,15 @@
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
-msgstr ""
+msgstr "Olet poistamassa kaksivaiheisen tunnistautumisen. Tämä heikentää tilisi turvallisuutta. Haluatko varmasti poistaa?"
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
 msgstr "Poista käytöstä"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
@@ -441,15 +442,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "Näppäile puhelinnnumero maakoodin kanssa, joka alkaa + tai 00 -merkeillä."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
+msgid "ManagementForm data is missing or has been tampered with"
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/mn_MN/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/mn_MN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/fr/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/fr/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-02-06 17:43+0000\n"
+"Last-Translator: Doryan R\n"
 "Language-Team: French (http://www.transifex.com/Bouke/django-two-factor-auth/"
 "language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -133,17 +133,28 @@
 msgid ""
 "If you don't have any device with you, you can access\n"
 "        your account using backup tokens."
 msgstr ""
 "Si vous n'avez aucun appareil sur vous, vous pouvez accéder à votre\n"
 "compte en utilisant des jetons de secours."
 
+msgid ""
+"If your primary method is not available, we are able to\n"
+"        send backup tokens to the phone numbers listed below."
+msgstr ""
+"Si votre méthode principale n’est pas disponible, nous pouvons\n"
+"envoyez des jetons de sauvegarde aux numéros de téléphone indiqués ci-"
+"dessous."
+
 msgid "Login"
 msgstr "Se connecter"
 
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "Les données ManagementForm sont manquantes ou ont été falsifiées"
+
 msgid "Method"
 msgstr "Méthode"
 
 msgid "Next"
 msgstr "Suivante"
 
 msgid "Or, alternatively, use one of your backup phones:"
@@ -151,14 +162,17 @@
 
 msgid "Permission Denied"
 msgstr "Permission refusée"
 
 msgid "Phone Call"
 msgstr "Appel téléphonique"
 
+msgid "Phone Number"
+msgstr "Numéro de téléphone"
+
 msgid "Phone call"
 msgstr "Appel téléphonique"
 
 msgid ""
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 msgstr ""
@@ -295,37 +309,76 @@
 "      Ces jetons ont été générés pour que vous les imprimiez et les gardiez "
 "en sécurité. Merci\n"
 "      d'entrer un de ces jetons de secours pour vous connecter à votre "
 "compte."
 
 msgid ""
 "We are calling your phone right now, please enter the\n"
+"          digits you hear."
+msgstr ""
+"Nous appelons votre téléphone dès maintenant, veuillez entrer le\n"
+"chiffres que vous entendez."
+
+msgid ""
+"We are calling your phone right now, please enter the\n"
 "        digits you hear."
 msgstr ""
 "Nous essayons de vous contacter au numéro fourni à l'instant.\n"
 "Veuillez entrer les numéros que vous entendez."
 
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
+"          sent."
+msgstr ""
+"Nous vous avons envoyé un message texte, veuillez entrer les jetons que nous "
+"avons envoyer."
+
+msgid ""
+"We sent you a text message, please enter the tokens we\n"
 "        sent."
 msgstr ""
 "Vous avez reçu un SMS, veuillez entrer les jetons\n"
 "que nous avons envoyés."
 
 msgid ""
+"We've\n"
+"        encountered an issue with the selected authentication method. "
+"Please\n"
+"        go back and verify that you entered your information correctly, try\n"
+"        again, or use a different authentication method instead. If the "
+"issue\n"
+"        persists, contact the site administrator."
+msgstr ""
+"Nous avons\n"
+"rencontré un problème avec la méthode d'authentification sélectionnée. S'il "
+"vous plaît\n"
+"revenir en arrière et vérifier que vous avez entré vos informations "
+"correctement, essayez\n"
+"à nouveau, ou utilisez une autre méthode d’authentification. Si le problème\n"
+"persiste, contactez l'administrateur du site."
+
+msgid ""
 "We've sent a token to your phone number. Please\n"
 "        enter the token you've received."
 msgstr ""
 "Nous vous avons envoyé un jeton par téléphone.\n"
 "Veuillez entrer le jeton que vous avez reçu."
 
 msgid "Yes, I am sure"
 msgstr "Oui, je suis sûr"
 
 msgid ""
+"You are about to disable two-factor authentication. This\n"
+"    weakens your account security, are you sure?"
+msgstr ""
+"Vous êtes sur le point de désactiver l'authentification à deux facteurs. "
+"Cela\n"
+"affaiblira la sécurité du compte compte, êtes-vous sûr?"
+
+msgid ""
 "You are about to take your account security to the\n"
 "        next level. Follow the steps in this wizard to enable two-factor\n"
 "        authentication."
 msgstr ""
 "Vous êtes sur le point d'augmenter la sécurité de \n"
 "votre compte. Suivez les étapes de cet assistant pour activer\n"
 "l'authentification à deux facteurs "
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/fr/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/fr/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Translators:
+# Doryan R, 2019
 # bato <francoisconil@gmail.com>, 2014,2018
 # Michael Mior <michael.mior@gmail.com>, 2014
 # Nils Van Zuijlen <nilsdu29@gmail.com>, 2018
 # qmarlats <qmarlats.ghost@outlook.com>, 2015
 # xxinfinityxx <xxinfinityxx@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
-"PO-Revision-Date: 2018-08-03 13:23+0000\n"
-"Last-Translator: Bouke Haarsma <bouke@haarsma.eu>\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
+"PO-Revision-Date: 2019-02-06 17:43+0000\n"
+"Last-Translator: Doryan R\n"
 "Language-Team: French (http://www.transifex.com/Bouke/django-two-factor-auth/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: forms.py:24 forms.py:36
 msgid "Method"
 msgstr "Méthode"
 
 #: forms.py:34 forms.py:49
 #| msgid "Add Phone Number"
 msgid "Phone Number"
-msgstr ""
+msgstr "Numéro de téléphone"
 
 #: forms.py:58 forms.py:88 forms.py:142 forms.py:178
 msgid "Token"
 msgstr "Jeton"
 
 #: forms.py:61 forms.py:91
 #| msgid "Entered token is not valid"
@@ -107,15 +108,15 @@
 msgid "Text message"
 msgstr "Message texte"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Générateur des jetons"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "méthode"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "Annuler"
 
@@ -284,30 +285,30 @@
 "      This number will be validated in the next step. "
 msgstr "Veuillez entrer le numéro qui sera utilisé pour vous\ncontacter. Ce numéro sera validé à la prochaine étape."
 
 #: templates/two_factor/core/setup.html:29
 msgid ""
 "We are calling your phone right now, please enter the\n"
 "          digits you hear."
-msgstr ""
+msgstr "Nous appelons votre téléphone dès maintenant, veuillez entrer le\nchiffres que vous entendez."
 
 #: templates/two_factor/core/setup.html:32
 msgid ""
 "We sent you a text message, please enter the tokens we\n"
 "          sent."
-msgstr ""
+msgstr "Nous vous avons envoyé un message texte, veuillez entrer les jetons que nous avons envoyer."
 
 #: templates/two_factor/core/setup.html:36
 msgid ""
 "We've\n"
 "        encountered an issue with the selected authentication method. Please\n"
 "        go back and verify that you entered your information correctly, try\n"
 "        again, or use a different authentication method instead. If the issue\n"
 "        persists, contact the site administrator."
-msgstr ""
+msgstr "Nous avons\nrencontré un problème avec la méthode d'authentification sélectionnée. S'il vous plaît\nrevenir en arrière et vérifier que vous avez entré vos informations correctement, essayez\nà nouveau, ou utilisez une autre méthode d’authentification. Si le problème\npersiste, contactez l'administrateur du site."
 
 #: templates/two_factor/core/setup.html:43
 msgid ""
 "To identify and verify your YubiKey, please insert a\n"
 "      token in the field below. Your YubiKey will be linked to your\n"
 "      account."
 msgstr "Pour identifier et vérifier votre YubiKey, merci d'insérer un\n      jeton dans le champ ci-dessous. Votre YubiKey sera liée à votre\n      compte."
@@ -346,15 +347,15 @@
 #: templates/two_factor/profile/disable.html:6
 #| msgid ""
 #| "e about to disable two-factor authentication. This\n"
 #| "mpromises your account security, are you sure?"
 msgid ""
 "You are about to disable two-factor authentication. This\n"
 "    weakens your account security, are you sure?"
-msgstr ""
+msgstr "Vous êtes sur le point de désactiver l'authentification à deux facteurs. Cela\naffaiblira la sécurité du compte compte, êtes-vous sûr?"
 
 #: templates/two_factor/profile/disable.html:12
 msgid "Disable"
 msgstr "Désactiver"
 
 #: templates/two_factor/profile/profile.html:5
 msgid "Account Security"
@@ -381,15 +382,15 @@
 #: templates/two_factor/profile/profile.html:18
 #| msgid ""
 #| "r primary method is not available, we are able to\n"
 #| "send backup tokens to the phone numbers listed below."
 msgid ""
 "If your primary method is not available, we are able to\n"
 "        send backup tokens to the phone numbers listed below."
-msgstr ""
+msgstr "Si votre méthode principale n’est pas disponible, nous pouvons\nenvoyez des jetons de sauvegarde aux numéros de téléphone indiqués ci-dessous."
 
 #: templates/two_factor/profile/profile.html:28
 msgid "Unregister"
 msgstr "Désinscrire"
 
 #: templates/two_factor/profile/profile.html:39
 msgid ""
@@ -445,15 +446,15 @@
 #: validators.py:14
 msgid ""
 "Please enter a valid phone number, including your country code starting with"
 " + or 00."
 msgstr "Veuillez entrer un numéro valide, contenant l'indicateur du pays commençant par + ou 00."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
-msgstr ""
+msgid "ManagementForm data is missing or has been tampered with"
+msgstr "Les données ManagementForm sont manquantes ou ont été falsifiées"
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/es/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/es/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/en/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/en/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
 "PO-Revision-Date: 2013-11-27 20:08+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@webatoom.nl>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/en/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/en/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-two-factor-auth\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-08-03 15:23+0200\n"
+"POT-Creation-Date: 2019-07-07 08:46+0200\n"
 "PO-Revision-Date: 2013-11-27 20:08+0000\n"
 "Last-Translator: Bouke Haarsma <bouke@webatoom.nl>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -108,15 +108,15 @@
 msgid "Text message"
 msgstr "Text Message"
 
 #: models.py:47
 msgid "Token generator"
 msgstr "Token generator"
 
-#: models.py:71
+#: models.py:75
 msgid "method"
 msgstr "method"
 
 #: templates/two_factor/_wizard_actions.html:5
 msgid "Cancel"
 msgstr "Cancel"
 
@@ -507,15 +507,15 @@
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 msgstr ""
 "Please enter a valid phone number, including your country code starting with "
 "+ or 00."
 
 #: views/utils.py:111
-msgid "ManagementForm data is missing or has been tampered."
+msgid "ManagementForm data is missing or has been tampered with"
 msgstr ""
 
 #~ msgid "Please enter a valid token."
 #~ msgstr "Please enter a valid token."
 
 #~ msgid "number"
 #~ msgstr "number"
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/fa/LC_MESSAGES/django.po` & `django-two-factor-auth-1.9.1/two_factor/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/locale/da_DK/LC_MESSAGES/django.mo` & `django-two-factor-auth-1.9.1/two_factor/locale/da_DK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/models.py` & `django-two-factor-auth-1.9.1/two_factor/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,42 +51,39 @@
 
 
 def key_validator(*args, **kwargs):
     """Wraps hex_validator generator, to keep makemigrations happy."""
     return hex_validator()(*args, **kwargs)
 
 
+def random_hex_str():
+    return random_hex().decode('utf-8')
+
+
 class PhoneDevice(Device):
     """
     Model with phone number and token seed linked to a user.
     """
     class Meta:
         app_label = 'two_factor'
 
     number = PhoneNumberField()
     key = models.CharField(max_length=40,
                            validators=[key_validator],
-                           default=random_hex,
+                           default=random_hex_str,
                            help_text="Hex-encoded secret key")
     method = models.CharField(max_length=4, choices=PHONE_METHODS,
                               verbose_name=_('method'))
 
     def __repr__(self):
         return '<PhoneDevice(number={!r}, method={!r}>'.format(
             self.number,
             self.method,
         )
 
-    def __eq__(self, other):
-        if not isinstance(other, PhoneDevice):
-            return False
-        return self.number == other.number \
-            and self.method == other.method \
-            and self.key == other.key
-
     @property
     def bin_key(self):
         return unhexlify(self.key.encode())
 
     def verify_token(self, token):
         # local import to avoid circular import
         from two_factor.utils import totp_digits
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/validators.py` & `django-two-factor-auth-1.9.1/two_factor/validators.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/management/commands/two_factor_disable.py` & `django-two-factor-auth-1.9.1/two_factor/management/commands/two_factor_disable.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/management/commands/two_factor_status.py` & `django-two-factor-auth-1.9.1/two_factor/management/commands/two_factor_status.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/forms.py` & `django-two-factor-auth-1.9.1/two_factor/forms.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/admin.py` & `django-two-factor-auth-1.9.1/two_factor/admin.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/utils.py` & `django-two-factor-auth-1.9.1/two_factor/utils.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/gateways/fake.py` & `django-two-factor-auth-1.9.1/two_factor/gateways/fake.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/gateways/twilio/gateway.py` & `django-two-factor-auth-1.9.1/two_factor/gateways/twilio/gateway.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/gateways/twilio/views.py` & `django-two-factor-auth-1.9.1/two_factor/gateways/twilio/views.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/phone_register.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/login.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/setup_complete.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/setup_complete.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "two_factor/_base_focus.html" %}
 {% load i18n %}
 
 {% block content %}
   <h1>{% block title %}{% trans "Enable Two-Factor Authentication" %}{% endblock %}</h1>
 
   <p>{% blocktrans %}Congratulations, you've successfully enabled two-factor
-      authentication.{% endblocktrans %}
+      authentication.{% endblocktrans %}</p>
 
   {% if not phone_methods %}
     <p><a href="{% url 'two_factor:profile' %}"
         class="btn btn-block btn-default">{% trans "Back to Profile" %}</a></p>
   {% else %}
     <p>{% blocktrans %}However, it might happen that you don't have access to
       your primary token device. To enable account recovery, add a phone
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% extends "two_factor/_base_focus.html" %} {% load i18n %} {% block content %}
 ****** {% block title %}{% trans "Enable Two-Factor Authentication" %}{%
 endblock %} ******
 {% blocktrans %}Congratulations, you've successfully enabled two-factor
-authentication.{% endblocktrans %} {% if not phone_methods %}
+authentication.{% endblocktrans %}
+{% if not phone_methods %}
 {%_trans_"Back_to_Profile"_%}
 {% else %}
 {% blocktrans %}However, it might happen that you don't have access to your
 primary token device. To enable account recovery, add a phone number.{%
 endblocktrans %}
 {%_trans_"Back_to_Profile"_%}
 {%_trans_"Add_Phone_Number"_%}
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/backup_tokens.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/setup.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/core/otp_required.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/profile/profile.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/profile/profile.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/profile/disable.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_base.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_base.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/templates/two_factor/_wizard_actions.html` & `django-two-factor-auth-1.9.1/two_factor/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/urls.py` & `django-two-factor-auth-1.9.1/two_factor/urls.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/views/mixins.py` & `django-two-factor-auth-1.9.1/two_factor/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/views/profile.py` & `django-two-factor-auth-1.9.1/two_factor/views/profile.py`

 * *Files identical despite different names*

### Comparing `django-two-factor-auth-1.8.0/two_factor/views/core.py` & `django-two-factor-auth-1.9.1/two_factor/views/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,14 +534,17 @@
 
     # The qrcode library only supports PNG and SVG for now
     image_content_types = {
         'PNG': 'image/png',
         'SVG': 'image/svg+xml; charset=utf-8',
     }
 
+    def get_issuer(self):
+        return get_current_site(self.request).name
+
     def get(self, request, *args, **kwargs):
         # Get the data from the session
         try:
             key = self.request.session[self.session_key_name]
         except KeyError:
             raise Http404()
 
@@ -551,15 +554,15 @@
         content_type = self.image_content_types[image_factory.kind]
         try:
             username = self.request.user.get_username()
         except AttributeError:
             username = self.request.user.username
 
         otpauth_url = get_otpauth_url(accountname=username,
-                                      issuer=get_current_site(self.request).name,
+                                      issuer=self.get_issuer(),
                                       secret=key,
                                       digits=totp_digits())
 
         # Make and return QR code
         img = qrcode.make(otpauth_url, image_factory=image_factory)
         resp = HttpResponse(content_type=content_type)
         img.save(resp)
```

### Comparing `django-two-factor-auth-1.8.0/two_factor/views/utils.py` & `django-two-factor-auth-1.9.1/two_factor/views/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,19 +104,19 @@
         wizard_goto_step = self.request.POST.get('wizard_goto_step', None)
         if wizard_goto_step and wizard_goto_step in self.get_form_list():
             return self.render_goto_step(wizard_goto_step)
 
         # Check if form was refreshed
         management_form = ManagementForm(self.request.POST, prefix=self.prefix)
         if not management_form.is_valid():
-            raise SuspiciousOperation(_('ManagementForm data is missing or has been tampered.'))
+            raise SuspiciousOperation(_('ManagementForm data is missing or has been tampered with'))
 
         form_current_step = management_form.cleaned_data['current_step']
-        if (form_current_step != self.steps.current and
-                self.storage.current_step is not None):
+        if (form_current_step != self.steps.current
+                and self.storage.current_step is not None):
             # form refreshed, change current step
             self.storage.current_step = form_current_step
         # -- End duplicated code from upstream
 
         # This is different from the first check, as this checks
         # if the new step is available. See issue #65.
         if self.steps.current not in self.steps.all:
```

### Comparing `django-two-factor-auth-1.8.0/setup.py` & `django-two-factor-auth-1.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django-two-factor-auth',
-    version='1.8.0',
+    version='1.9.1',
     description='Complete Two-Factor Authentication for Django',
     long_description=open('README.rst').read(),
     author='Bouke Haarsma',
     author_email='bouke@haarsma.eu',
     url='https://github.com/Bouke/django-two-factor-auth',
     download_url='https://pypi.python.org/pypi/django-two-factor-auth',
     license='MIT',
     packages=find_packages(exclude=('example', 'tests')),
     install_requires=[
         'Django>=1.11',
-        'django_otp>=0.3.4,<0.99',
+        'django_otp>=0.6.0,<0.99',
         'qrcode>=4.0.0,<6.99',
         'django-phonenumber-field>=1.1.0,<1.99',
         'django-formtools',
     ],
     extras_require={
         'Call': ['twilio>=6.0'],
         'SMS': ['twilio>=6.0'],
@@ -25,22 +25,24 @@
     },
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.0',
+        'Framework :: Django :: 2.1',
+        'Framework :: Django :: 2.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Topic :: Security',
         'Topic :: System :: Systems Administration :: Authentication/Directory',
     ],
 )
```

### Comparing `django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/PKG-INFO` & `django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-two-factor-auth
-Version: 1.8.0
+Version: 1.9.1
 Summary: Complete Two-Factor Authentication for Django
 Home-page: https://github.com/Bouke/django-two-factor-auth
 Author: Bouke Haarsma
 Author-email: bouke@haarsma.eu
 License: MIT
 Download-URL: https://pypi.python.org/pypi/django-two-factor-auth
 Description: ================================
@@ -40,23 +40,32 @@
         Test drive this app through the online `example app`_, hosted by Heroku_. It
         demos most features except the Twilio integration. The example also includes
         django-user-sessions_ for providing Django sessions with a foreign key to the
         user. Although the package is optional, it improves account security control
         over ``django.contrib.sessions``.
         
         Compatible with modern Django versions. At the moment of writing that's
-        including 1.11 and 2.0 on Python 2.7, 3.4, 3.5 and 3.6. Documentation
+        including 1.11, 2.1, and 2.2 on Python 2.7, 3.4, 3.5, 3.6 and 3.7. Documentation
         is available at `readthedocs.org`_.
         
         
         Installation
         ============
         Refer to the `installation instructions`_ in the documentation.
         
         
+        Getting help
+        ============
+        
+        For general questions regarding this package, please hop over to Stack 
+        Overflow. If you think there is an issue with this package; check if the
+        issue is already listed (either open or closed), and file an issue if
+        it's not.
+        
+        
         Contribute
         ==========
         * Submit issues to the `issue tracker`_ on Github.
         * Fork the `source code`_ at Github.
         * Write some code and make sure it is covered with unit tests.
         * Send a pull request with your changes.
         * Provide a translation using Transifex_.
@@ -133,20 +142,25 @@
            https://hynek.me/articles/sharing-your-labor-of-love-pypi-quick-and-dirty/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
+Provides-Extra: Call
+Provides-Extra: SMS
+Provides-Extra: YubiKey
```

### Comparing `django-two-factor-auth-1.8.0/django_two_factor_auth.egg-info/SOURCES.txt` & `django-two-factor-auth-1.9.1/django_two_factor_auth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup.cfg
 setup.py
 django_two_factor_auth.egg-info/PKG-INFO
 django_two_factor_auth.egg-info/SOURCES.txt
 django_two_factor_auth.egg-info/dependency_links.txt
 django_two_factor_auth.egg-info/requires.txt
 django_two_factor_auth.egg-info/top_level.txt
+tests/migrations/0001_initial.py
+tests/migrations/__init__.py
 two_factor/__init__.py
 two_factor/admin.py
 two_factor/apps.py
 two_factor/forms.py
 two_factor/models.py
 two_factor/signals.py
 two_factor/urls.py
@@ -79,14 +81,15 @@
 two_factor/middleware/__init__.py
 two_factor/middleware/threadlocals.py
 two_factor/migrations/0001_initial.py
 two_factor/migrations/0002_auto_20150110_0810.py
 two_factor/migrations/0003_auto_20150817_1733.py
 two_factor/migrations/0004_auto_20160205_1827.py
 two_factor/migrations/0005_auto_20160224_0450.py
+two_factor/migrations/0006_phonedevice_key_default.py
 two_factor/migrations/__init__.py
 two_factor/templates/two_factor/_base.html
 two_factor/templates/two_factor/_base_focus.html
 two_factor/templates/two_factor/_wizard_actions.html
 two_factor/templates/two_factor/_wizard_forms.html
 two_factor/templates/two_factor/core/backup_tokens.html
 two_factor/templates/two_factor/core/login.html
```

### Comparing `django-two-factor-auth-1.8.0/README.rst` & `django-two-factor-auth-1.9.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,23 +31,32 @@
 Test drive this app through the online `example app`_, hosted by Heroku_. It
 demos most features except the Twilio integration. The example also includes
 django-user-sessions_ for providing Django sessions with a foreign key to the
 user. Although the package is optional, it improves account security control
 over ``django.contrib.sessions``.
 
 Compatible with modern Django versions. At the moment of writing that's
-including 1.11 and 2.0 on Python 2.7, 3.4, 3.5 and 3.6. Documentation
+including 1.11, 2.1, and 2.2 on Python 2.7, 3.4, 3.5, 3.6 and 3.7. Documentation
 is available at `readthedocs.org`_.
 
 
 Installation
 ============
 Refer to the `installation instructions`_ in the documentation.
 
 
+Getting help
+============
+
+For general questions regarding this package, please hop over to Stack 
+Overflow. If you think there is an issue with this package; check if the
+issue is already listed (either open or closed), and file an issue if
+it's not.
+
+
 Contribute
 ==========
 * Submit issues to the `issue tracker`_ on Github.
 * Fork the `source code`_ at Github.
 * Write some code and make sure it is covered with unit tests.
 * Send a pull request with your changes.
 * Provide a translation using Transifex_.
```

