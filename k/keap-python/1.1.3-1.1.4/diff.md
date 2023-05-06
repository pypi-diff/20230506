# Comparing `tmp/keap-python-1.1.3.tar.gz` & `tmp/keap-python-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keap-python-1.1.3.tar", last modified: Thu Mar 16 15:07:45 2023, max compression
+gzip compressed data, was "keap-python-1.1.4.tar", last modified: Sat May  6 15:13:59 2023, max compression
```

## Comparing `keap-python-1.1.3.tar` & `keap-python-1.1.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.752225 keap-python-1.1.3/
--rw-rw-rw-   0        0        0      291 2023-03-16 15:07:45.752225 keap-python-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    19817 2023-01-17 21:08:49.000000 keap-python-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.670226 keap-python-1.1.3/keap/
--rw-rw-rw-   0        0        0     4059 2023-03-16 15:07:06.000000 keap-python-1.1.3/keap/Keap.py
--rw-rw-rw-   0        0        0      485 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/KeapToken.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.677225 keap-python-1.1.3/keap/REST/
--rw-rw-rw-   0        0        0     3793 2023-02-10 17:54:39.000000 keap-python-1.1.3/keap/REST/BaseService.py
--rw-rw-rw-   0        0        0     1639 2023-02-09 20:48:03.000000 keap-python-1.1.3/keap/REST/REST_V1.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.712226 keap-python-1.1.3/keap/REST/V1/
--rw-rw-rw-   0        0        0      213 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/AccountService.py
--rw-rw-rw-   0        0        0      982 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/AffiliateService.py
--rw-rw-rw-   0        0        0      450 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/AppointmentService.py
--rw-rw-rw-   0        0        0     1283 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/CampaignService.py
--rw-rw-rw-   0        0        0      283 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/CompanyService.py
--rw-rw-rw-   0        0        0     5753 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/ContactService.py
--rw-rw-rw-   0        0        0     1360 2023-03-09 19:21:44.000000 keap-python-1.1.3/keap/REST/V1/EmailService.py
--rw-rw-rw-   0        0        0      281 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/FileService.py
--rw-rw-rw-   0        0        0     1010 2023-02-15 17:35:17.000000 keap-python-1.1.3/keap/REST/V1/HookService.py
--rw-rw-rw-   0        0        0      513 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/LocaleService.py
--rw-rw-rw-   0        0        0      174 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/MerchantService.py
--rw-rw-rw-   0        0        0      603 2023-02-10 19:28:12.000000 keap-python-1.1.3/keap/REST/V1/NoteService.py
--rw-rw-rw-   0        0        0      426 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/OpportunityService.py
--rw-rw-rw-   0        0        0     1126 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/OrderService.py
--rw-rw-rw-   0        0        0     1175 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/ProductService.py
--rw-rw-rw-   0        0        0      410 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/SettingService.py
--rw-rw-rw-   0        0        0      232 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/SubscriptionService.py
--rw-rw-rw-   0        0        0     2420 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/TagService.py
--rw-rw-rw-   0        0        0      455 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/TaskService.py
--rw-rw-rw-   0        0        0      210 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/TransactionService.py
--rw-rw-rw-   0        0        0      434 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/UserService.py
--rw-rw-rw-   0        0        0      918 2023-02-09 20:47:46.000000 keap-python-1.1.3/keap/REST/V1/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/V1/mixins.py
--rw-rw-rw-   0        0        0       38 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/__init__.py
--rw-rw-rw-   0        0        0     3188 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/REST/models.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.738224 keap-python-1.1.3/keap/XML/
--rw-rw-rw-   0        0        0      148 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/AffiliateProgramService.py
--rw-rw-rw-   0        0        0      289 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/AffiliateService.py
--rw-rw-rw-   0        0        0     1744 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/BaseService.py
--rw-rw-rw-   0        0        0     1836 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/ContactService.py
--rw-rw-rw-   0        0        0     1338 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/DataService.py
--rw-rw-rw-   0        0        0      140 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/DiscountService.py
--rw-rw-rw-   0        0        0      454 2023-03-10 19:45:25.000000 keap-python-1.1.3/keap/XML/EmailService.py
--rw-rw-rw-   0        0        0      136 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/FileService.py
--rw-rw-rw-   0        0        0      138 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/FunnelService.py
--rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/InvoiceService.py
--rw-rw-rw-   0        0        0      137 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/OrderService.py
--rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/ProductService.py
--rw-rw-rw-   0        0        0      300 2023-03-08 17:04:18.000000 keap-python-1.1.3/keap/XML/SearchService.py
--rw-rw-rw-   0        0        0      140 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/ShippingService.py
--rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/WebFormService.py
--rw-rw-rw-   0        0        0     1172 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/XML.py
--rw-rw-rw-   0        0        0      656 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/XML/__init__.py
--rw-rw-rw-   0        0        0       58 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/__init__.py
--rw-rw-rw-   0        0        0      229 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/exceptions.py
--rw-rw-rw-   0        0        0     3939 2023-01-17 21:10:51.000000 keap-python-1.1.3/keap/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.741225 keap-python-1.1.3/keap/scripts/
--rw-rw-rw-   0        0        0        0 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/scripts/__init__.py
--rw-rw-rw-   0        0        0     3755 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/scripts/cli.py
--rw-rw-rw-   0        0        0     5145 2023-01-17 21:13:02.000000 keap-python-1.1.3/keap/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.747224 keap-python-1.1.3/keap/storages/
--rw-rw-rw-   0        0        0      348 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      700 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1562 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      122 2023-01-17 21:08:49.000000 keap-python-1.1.3/keap/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:07:45.751225 keap-python-1.1.3/keap_python.egg-info/
--rw-rw-rw-   0        0        0      291 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-16 15:07:45.000000 keap-python-1.1.3/keap_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 15:07:45.753225 keap-python-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-03-16 15:07:30.000000 keap-python-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.051998 keap-python-1.1.4/
+-rw-rw-rw-   0        0        0      291 2023-05-06 15:13:59.051998 keap-python-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    19817 2023-01-17 21:08:49.000000 keap-python-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:58.965999 keap-python-1.1.4/keap/
+-rw-rw-rw-   0        0        0     4059 2023-03-16 15:07:06.000000 keap-python-1.1.4/keap/Keap.py
+-rw-rw-rw-   0        0        0      485 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/KeapToken.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:58.972998 keap-python-1.1.4/keap/REST/
+-rw-rw-rw-   0        0        0     3793 2023-02-10 17:54:39.000000 keap-python-1.1.4/keap/REST/BaseService.py
+-rw-rw-rw-   0        0        0     1639 2023-02-09 20:48:03.000000 keap-python-1.1.4/keap/REST/REST_V1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.009998 keap-python-1.1.4/keap/REST/V1/
+-rw-rw-rw-   0        0        0      213 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/AccountService.py
+-rw-rw-rw-   0        0        0      982 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/AffiliateService.py
+-rw-rw-rw-   0        0        0      450 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/AppointmentService.py
+-rw-rw-rw-   0        0        0     1283 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/CampaignService.py
+-rw-rw-rw-   0        0        0      283 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/CompanyService.py
+-rw-rw-rw-   0        0        0     5753 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/ContactService.py
+-rw-rw-rw-   0        0        0     1360 2023-03-09 19:21:44.000000 keap-python-1.1.4/keap/REST/V1/EmailService.py
+-rw-rw-rw-   0        0        0      281 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/FileService.py
+-rw-rw-rw-   0        0        0     1010 2023-02-15 17:35:17.000000 keap-python-1.1.4/keap/REST/V1/HookService.py
+-rw-rw-rw-   0        0        0      513 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/LocaleService.py
+-rw-rw-rw-   0        0        0      174 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/MerchantService.py
+-rw-rw-rw-   0        0        0      603 2023-02-10 19:28:12.000000 keap-python-1.1.4/keap/REST/V1/NoteService.py
+-rw-rw-rw-   0        0        0      426 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/OpportunityService.py
+-rw-rw-rw-   0        0        0     1126 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/OrderService.py
+-rw-rw-rw-   0        0        0     1175 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/ProductService.py
+-rw-rw-rw-   0        0        0      410 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/SettingService.py
+-rw-rw-rw-   0        0        0      232 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/SubscriptionService.py
+-rw-rw-rw-   0        0        0     2420 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/TagService.py
+-rw-rw-rw-   0        0        0      455 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/TaskService.py
+-rw-rw-rw-   0        0        0      210 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/TransactionService.py
+-rw-rw-rw-   0        0        0      434 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/UserService.py
+-rw-rw-rw-   0        0        0      918 2023-02-09 20:47:46.000000 keap-python-1.1.4/keap/REST/V1/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/V1/mixins.py
+-rw-rw-rw-   0        0        0       38 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/__init__.py
+-rw-rw-rw-   0        0        0     3188 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/REST/models.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.036998 keap-python-1.1.4/keap/XML/
+-rw-rw-rw-   0        0        0      148 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/AffiliateProgramService.py
+-rw-rw-rw-   0        0        0      289 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/AffiliateService.py
+-rw-rw-rw-   0        0        0     1744 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/BaseService.py
+-rw-rw-rw-   0        0        0     1836 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/ContactService.py
+-rw-rw-rw-   0        0        0     1338 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/DataService.py
+-rw-rw-rw-   0        0        0      140 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/DiscountService.py
+-rw-rw-rw-   0        0        0      454 2023-03-10 19:45:25.000000 keap-python-1.1.4/keap/XML/EmailService.py
+-rw-rw-rw-   0        0        0      136 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/FileService.py
+-rw-rw-rw-   0        0        0      138 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/FunnelService.py
+-rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/InvoiceService.py
+-rw-rw-rw-   0        0        0      137 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/OrderService.py
+-rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/ProductService.py
+-rw-rw-rw-   0        0        0      300 2023-03-08 17:04:18.000000 keap-python-1.1.4/keap/XML/SearchService.py
+-rw-rw-rw-   0        0        0      140 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/ShippingService.py
+-rw-rw-rw-   0        0        0      139 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/WebFormService.py
+-rw-rw-rw-   0        0        0     1172 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/XML.py
+-rw-rw-rw-   0        0        0      656 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/XML/__init__.py
+-rw-rw-rw-   0        0        0       58 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/__init__.py
+-rw-rw-rw-   0        0        0      229 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/exceptions.py
+-rw-rw-rw-   0        0        0     3939 2023-01-17 21:10:51.000000 keap-python-1.1.4/keap/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.039997 keap-python-1.1.4/keap/scripts/
+-rw-rw-rw-   0        0        0        0 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3755 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/scripts/cli.py
+-rw-rw-rw-   0        0        0     5469 2023-05-06 15:12:47.000000 keap-python-1.1.4/keap/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.045998 keap-python-1.1.4/keap/storages/
+-rw-rw-rw-   0        0        0      348 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      700 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1562 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      122 2023-01-17 21:08:49.000000 keap-python-1.1.4/keap/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:13:59.050998 keap-python-1.1.4/keap_python.egg-info/
+-rw-rw-rw-   0        0        0      291 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-06 15:13:58.000000 keap-python-1.1.4/keap_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 15:13:59.051998 keap-python-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-06 15:12:58.000000 keap-python-1.1.4/setup.py
```

### Comparing `keap-python-1.1.3/README.md` & `keap-python-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/Keap.py` & `keap-python-1.1.4/keap/Keap.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/BaseService.py` & `keap-python-1.1.4/keap/REST/BaseService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/REST_V1.py` & `keap-python-1.1.4/keap/REST/REST_V1.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/AffiliateService.py` & `keap-python-1.1.4/keap/REST/V1/AffiliateService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/CampaignService.py` & `keap-python-1.1.4/keap/REST/V1/CampaignService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/ContactService.py` & `keap-python-1.1.4/keap/REST/V1/ContactService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/EmailService.py` & `keap-python-1.1.4/keap/REST/V1/EmailService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/HookService.py` & `keap-python-1.1.4/keap/REST/V1/HookService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/LocaleService.py` & `keap-python-1.1.4/keap/REST/V1/LocaleService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/NoteService.py` & `keap-python-1.1.4/keap/REST/V1/NoteService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/OrderService.py` & `keap-python-1.1.4/keap/REST/V1/OrderService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/ProductService.py` & `keap-python-1.1.4/keap/REST/V1/ProductService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/TagService.py` & `keap-python-1.1.4/keap/REST/V1/TagService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/__init__.py` & `keap-python-1.1.4/keap/REST/V1/__init__.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/V1/mixins.py` & `keap-python-1.1.4/keap/REST/V1/mixins.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/REST/models.py` & `keap-python-1.1.4/keap/REST/models.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/XML/BaseService.py` & `keap-python-1.1.4/keap/XML/BaseService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/XML/ContactService.py` & `keap-python-1.1.4/keap/XML/ContactService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/XML/DataService.py` & `keap-python-1.1.4/keap/XML/DataService.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/XML/XML.py` & `keap-python-1.1.4/keap/XML/XML.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/XML/__init__.py` & `keap-python-1.1.4/keap/XML/__init__.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/module_loading.py` & `keap-python-1.1.4/keap/module_loading.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/scripts/cli.py` & `keap-python-1.1.4/keap/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/settings.py` & `keap-python-1.1.4/keap/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 }
 
 This module provides the `api_setting` object, that is used to access
 KEAP settings, checking for user settings first, then falling
 back to the defaults.
 """
 from .module_loading import import_string
+from pathlib import Path
+import glob
+BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
+
+creds_search = glob.glob(str(BASE_DIR) + '/**/keap-credentials.json', recursive=True)
+if len(creds_search) > 0:
+    KEAP_CREDENTIALS = creds_search[0]
+else:
+    KEAP_CREDENTIALS = './keap-credentials.json'
+
 django_imported = False
 try:
     from django.conf import settings
     from django.test.signals import setting_changed
     # from django.utils.module_loading import import_string
     from django.core.exceptions import ImproperlyConfigured
 
@@ -42,15 +52,15 @@
     'CLIENT_SECRET': None,
     'REDIRECT_URL': 'https://theapiguys.com',
 
     'ALLOW_NONE': False,
     'USE_DATETIME': True,
 
     'STORAGE_CLASS': 'keap.storages.JSONStorage',
-    'CREDENTIALS_PATH': './keap-credentials.json',
+    'CREDENTIALS_PATH': KEAP_CREDENTIALS,
     'JSON_STORAGE_PATH': './keap-tokens.json',
 
     'APP_NAME': 'default',
 }
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
```

### Comparing `keap-python-1.1.3/keap/storages/InMemoryStorage.py` & `keap-python-1.1.4/keap/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap/storages/JSONStorage.py` & `keap-python-1.1.4/keap/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/keap_python.egg-info/SOURCES.txt` & `keap-python-1.1.4/keap_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keap-python-1.1.3/setup.py` & `keap-python-1.1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='keap-python',
-    version='1.1.3',
+    version='1.1.4',
     description='Python SDK for Keap API with Django Integration',
     url='https://bitbucket.org/theapiguys/keap-python',
     author='Brandon @ TheAPIGuys',
     author_email='brandon@theapiguys.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

