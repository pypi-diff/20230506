# Comparing `tmp/replalive-3.0.0.tar.gz` & `tmp/replalive-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replalive-3.0.0.tar", last modified: Sat May  6 15:32:51 2023, max compression
+gzip compressed data, was "replalive-4.0.0.tar", last modified: Sat May  6 15:34:25 2023, max compression
```

## Comparing `replalive-3.0.0.tar` & `replalive-4.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:32:51.858859 replalive-3.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      742 2023-05-06 15:32:51.858859 replalive-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2023-05-06 15:32:48.000000 replalive-3.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 replalive-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:32:51.858859 replalive-3.0.0/replalive.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      742 2023-05-06 15:32:51.000000 replalive-3.0.0/replalive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-05-06 15:32:51.000000 replalive-3.0.0/replalive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:32:51.000000 replalive-3.0.0/replalive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-05-06 15:32:51.000000 replalive-3.0.0/replalive.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:32:51.000000 replalive-3.0.0/replalive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 15:32:51.858859 replalive-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      405 2023-05-06 15:31:59.000000 replalive-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:34:25.146693 replalive-4.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)      718 2023-05-06 15:34:25.146693 replalive-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2023-05-06 15:34:11.000000 replalive-4.0.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 replalive-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:34:25.146693 replalive-4.0.0/replalive.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      718 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 15:34:25.146693 replalive-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      405 2023-05-06 15:34:18.000000 replalive-4.0.0/setup.py
```

### Comparing `replalive-3.0.0/PKG-INFO` & `replalive-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: replalive
-Version: 3.0.0
+Version: 4.0.0
 Summary: Keep your replit project online 24/7!
 Author: Hologramsteve#1900 on discord
 
-ReplAlive \n
-Keep your replit project online 24/7 \n
+ReplAlive  
+Keep your replit project online 24/7  
 
-How to use \n
-1. Enter ```pip install replalive``` into your shell and press enter \n
-2. Enter ```from replalive import keep_alive``` at the top of your code \n
-3. Enter the code ```keep_alive()``` in your code. Before (for example) client.run() is called, not after that! \n
-4. Go to https://uptimerobot.com/, register and make a monitor. \n
-5. The monitor settings will be: \n
-Monitor Type: Ping \n
-Friendly Name: my-monitor \n
-IP (or Host): https://PROJECTNAME.MYUSERNAME.repl.co \n
-Monitoring Interval: Every 5 minutes (1 minute costs money) \n
+How to use  
+1. Enter `pip install replalive` into your shell and press enter  
+2. Enter `from replalive import keep_alive` at the top of your code  
+3. Enter the code `keep_alive()` in your code. Before (for example) client.run() is called, not after that!  
+4. Go to https://uptimerobot.com/, register and make a monitor.  
+5. The monitor settings will be:  
+Monitor Type: Ping  
+Friendly Name: my-monitor  
+IP (or Host): https://PROJECTNAME.MYUSERNAME.repl.co  
+Monitoring Interval: Every 5 minutes (1 minute costs money)
```

### Comparing `replalive-3.0.0/replalive.egg-info/PKG-INFO` & `replalive-4.0.0/replalive.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: replalive
-Version: 3.0.0
+Version: 4.0.0
 Summary: Keep your replit project online 24/7!
 Author: Hologramsteve#1900 on discord
 
-ReplAlive \n
-Keep your replit project online 24/7 \n
+ReplAlive  
+Keep your replit project online 24/7  
 
-How to use \n
-1. Enter ```pip install replalive``` into your shell and press enter \n
-2. Enter ```from replalive import keep_alive``` at the top of your code \n
-3. Enter the code ```keep_alive()``` in your code. Before (for example) client.run() is called, not after that! \n
-4. Go to https://uptimerobot.com/, register and make a monitor. \n
-5. The monitor settings will be: \n
-Monitor Type: Ping \n
-Friendly Name: my-monitor \n
-IP (or Host): https://PROJECTNAME.MYUSERNAME.repl.co \n
-Monitoring Interval: Every 5 minutes (1 minute costs money) \n
+How to use  
+1. Enter `pip install replalive` into your shell and press enter  
+2. Enter `from replalive import keep_alive` at the top of your code  
+3. Enter the code `keep_alive()` in your code. Before (for example) client.run() is called, not after that!  
+4. Go to https://uptimerobot.com/, register and make a monitor.  
+5. The monitor settings will be:  
+Monitor Type: Ping  
+Friendly Name: my-monitor  
+IP (or Host): https://PROJECTNAME.MYUSERNAME.repl.co  
+Monitoring Interval: Every 5 minutes (1 minute costs money)
```

