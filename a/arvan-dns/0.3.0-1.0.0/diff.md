# Comparing `tmp/arvan_dns-0.3.0.tar.gz` & `tmp/arvan_dns-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvan_dns-0.3.0.tar", last modified: Sat May  6 19:52:40 2023, max compression
+gzip compressed data, was "arvan_dns-1.0.0.tar", last modified: Sat May  6 19:58:12 2023, max compression
```

## Comparing `arvan_dns-0.3.0.tar` & `arvan_dns-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:52:40.562722 arvan_dns-0.3.0/
--rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:52:40.562450 arvan_dns-0.3.0/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      195 2023-05-06 19:40:32.000000 arvan_dns-0.3.0/README.md
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:52:40.562197 arvan_dns-0.3.0/arvan_dns.egg-info/
--rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      231 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/SOURCES.txt
--rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/dependency_links.txt
--rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/entry_points.txt
--rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/requires.txt
--rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-06 19:52:40.000000 arvan_dns-0.3.0/arvan_dns.egg-info/top_level.txt
--rw-r--r--   0 seyed      (501) staff       (20)     3566 2023-05-06 19:51:48.000000 arvan_dns-0.3.0/arvan_dns.py
--rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-06 19:52:40.562779 arvan_dns-0.3.0/setup.cfg
--rw-r--r--   0 seyed      (501) staff       (20)      430 2023-05-06 19:51:54.000000 arvan_dns-0.3.0/setup.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:58:12.870903 arvan_dns-1.0.0/
+-rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:58:12.870639 arvan_dns-1.0.0/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      473 2023-05-06 19:57:54.000000 arvan_dns-1.0.0/README.md
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-06 19:58:12.870427 arvan_dns-1.0.0/arvan_dns.egg-info/
+-rw-r--r--   0 seyed      (501) staff       (20)      220 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      231 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/entry_points.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/requires.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-06 19:58:12.000000 arvan_dns-1.0.0/arvan_dns.egg-info/top_level.txt
+-rw-r--r--   0 seyed      (501) staff       (20)     3566 2023-05-06 19:51:48.000000 arvan_dns-1.0.0/arvan_dns.py
+-rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-06 19:58:12.870954 arvan_dns-1.0.0/setup.cfg
+-rw-r--r--   0 seyed      (501) staff       (20)      430 2023-05-06 19:58:07.000000 arvan_dns-1.0.0/setup.py
```

### Comparing `arvan_dns-0.3.0/arvan_dns.py` & `arvan_dns-1.0.0/arvan_dns.py`

 * *Files identical despite different names*

