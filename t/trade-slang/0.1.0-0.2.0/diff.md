# Comparing `tmp/trade_slang-0.1.0.tar.gz` & `tmp/trade_slang-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade_slang-0.1.0.tar", max compression
+gzip compressed data, was "trade_slang-0.2.0.tar", max compression
```

## Comparing `trade_slang-0.1.0.tar` & `trade_slang-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34523 2023-05-05 23:46:04.000000 trade_slang-0.1.0/LICENSE
--rw-r--r--   0        0        0       22 2023-05-06 06:58:52.937649 trade_slang-0.1.0/README.md
--rw-r--r--   0        0        0      388 2023-05-06 06:58:10.510458 trade_slang-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 06:52:07.902358 trade_slang-0.1.0/slang/__init__.py
--rw-r--r--   0        0        0       64 2023-05-06 06:58:10.506490 trade_slang-0.1.0/slang/__main__.py
--rw-r--r--   0        0        0     1030 2023-05-06 06:58:10.500166 trade_slang-0.1.0/slang/cli.py
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 trade_slang-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-05 23:46:04.000000 trade_slang-0.2.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-06 06:58:52.937649 trade_slang-0.2.0/README.md
+-rw-r--r--   0        0        0      388 2023-05-06 07:02:49.842132 trade_slang-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 06:52:07.902358 trade_slang-0.2.0/slang/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-06 06:58:10.506490 trade_slang-0.2.0/slang/__main__.py
+-rw-r--r--   0        0        0     1232 2023-05-06 07:02:49.838562 trade_slang-0.2.0/slang/cli.py
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 trade_slang-0.2.0/PKG-INFO
```

### Comparing `trade_slang-0.1.0/LICENSE` & `trade_slang-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trade_slang-0.1.0/slang/cli.py` & `trade_slang-0.2.0/slang/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 
 
 @cli.command()
 @click.argument('word')
 def term(word):
     """Get term definition"""
     response = requests.get(url + "/term/" + word)
-    click.echo(response.json())
+    console = rich.get_console()
+    if response.status_code == 404:
+        console.print("[bold]Not found[/bold]")
+        return
+    r = response.json()
+    console.print(Panel(r["result"]["definition"], title=r["result"]["key"]))
 
 
 @cli.command()
 @click.argument('text')
 def detect_slang(text):
     """Detect slang in text"""
     payload = {"text": text}
```

