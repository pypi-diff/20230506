# Comparing `tmp/arvan_dns-0.2.0.tar.gz` & `tmp/arvan_dns-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvan_dns-0.2.0.tar", last modified: Sat May  6 19:50:49 2023, max compression
+gzip compressed data, was "arvan_dns-0.3.0.tar", last modified: Sat May  6 19:52:40 2023, max compression
```

## Comparing `arvan_dns-0.2.0.tar` & `arvan_dns-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:50:49.525041 arvan_dns-0.2.0/
--rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:50:49.524744 arvan_dns-0.2.0/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      195 2023-05-06 19:40:32.000000 arvan_dns-0.2.0/README.md
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:50:49.524508 arvan_dns-0.2.0/arvan_dns.egg-info/
--rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      231 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/SOURCES.txt
--rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/dependency_links.txt
--rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/entry_points.txt
--rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/requires.txt
--rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-06 19:50:49.000000 arvan_dns-0.2.0/arvan_dns.egg-info/top_level.txt
--rw-r--r--   0 seyed      (501) staff       (20)     3586 2023-05-06 19:50:01.000000 arvan_dns-0.2.0/arvan_dns.py
--rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-06 19:50:49.525101 arvan_dns-0.2.0/setup.cfg
--rw-r--r--   0 seyed      (501) staff       (20)      430 2023-05-06 19:50:41.000000 arvan_dns-0.2.0/setup.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:52:40.562722 arvan_dns-0.3.0/
+-rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:52:40.562450 arvan_dns-0.3.0/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      195 2023-05-06 19:40:32.000000 arvan_dns-0.3.0/README.md
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:52:40.562197 arvan_dns-0.3.0/arvan_dns.egg-info/
+-rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      231 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/entry_points.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/requires.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/top_level.txt
+-rw-r--r--   0 seyed      (501) staff       (20)     3566 2023-05-06 19:51:48.000000 arvan_dns-0.3.0/arvan_dns.py
+-rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-06 19:52:40.562779 arvan_dns-0.3.0/setup.cfg
+-rw-r--r--   0 seyed      (501) staff       (20)      430 2023-05-06 19:51:54.000000 arvan_dns-0.3.0/setup.py
```

### Comparing `arvan_dns-0.2.0/arvan_dns.py` & `arvan_dns-0.3.0/arvan_dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
 BEARER_TOKEN = args.bearer_token
 OLD_IP = args.old_ip
 NEW_IP = args.new_ip
 SLEEP_TIME = int(args.sleep_time)
 DOMAINS_FILE = args.domains_file
 
-def get_domains():
-
 headers = {
         'authority': 'napi.arvancloud.ir',
         'accept': 'application/json, text/plain, */*',
         'accept-language': 'fa',
         'authorization': f'Bearer {BEARER_TOKEN}',
         'content-type': 'application/json',
         'origin': 'https://panel.arvancloud.ir',
```

