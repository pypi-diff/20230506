# Comparing `tmp/OWR-2.7.1.tar.gz` & `tmp/OWR-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.7.1.tar", last modified: Sat May  6 07:22:37 2023, max compression
+gzip compressed data, was "OWR-2.7.2.tar", last modified: Sat May  6 14:10:47 2023, max compression
```

## Comparing `OWR-2.7.1.tar` & `OWR-2.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.7.1/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    15092 2023-05-06 07:20:26.000000 OWR-2.7.1/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     5788 2023-05-06 07:20:17.000000 OWR-2.7.1/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-06 07:22:37.335755 OWR-2.7.1/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-06 07:20:17.000000 OWR-2.7.1/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-06 07:22:37.335755 OWR-2.7.1/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-06 07:22:26.000000 OWR-2.7.1/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 14:10:47.174733 OWR-2.7.2/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.7.2/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 14:10:47.174733 OWR-2.7.2/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    15076 2023-05-06 14:08:22.000000 OWR-2.7.2/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 14:10:47.174733 OWR-2.7.2/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     5788 2023-05-06 14:08:00.000000 OWR-2.7.2/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 14:10:47.174733 OWR-2.7.2/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      348 2023-05-06 14:10:47.000000 OWR-2.7.2/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-06 14:10:47.000000 OWR-2.7.2/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-06 14:10:47.000000 OWR-2.7.2/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-06 14:10:47.000000 OWR-2.7.2/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-06 14:10:47.000000 OWR-2.7.2/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      348 2023-05-06 14:10:47.174733 OWR-2.7.2/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-06 14:08:00.000000 OWR-2.7.2/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-06 14:10:47.174733 OWR-2.7.2/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      789 2023-05-06 14:10:33.000000 OWR-2.7.2/setup.py
```

### Comparing `OWR-2.7.1/LICENSE` & `OWR-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.7.1/OWR/__init__.py` & `OWR-2.7.2/OWR/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         Сохранение фонограм для всех слов из базы нецензурных слов.
 
         Parameters:
         ----------
             path_to_words: str
                 Json-файл со словарем нецензурных слов
-                
+
         Returns:
         ----------
             dict[str, str]]:
                 Словарь типа слово - код для всех нецензурных слов
         """
 
         result_word_to_code = {}
```

### Comparing `OWR-2.7.1/OWR/data/obscenity_words.json` & `OWR-2.7.2/OWR/data/obscenity_words.json`

 * *Files identical despite different names*

### Comparing `OWR-2.7.1/setup.py` & `OWR-2.7.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.7.1',
+    version='2.7.2',
     description='Obscene word recognition package',
     url='https://github.com/RuslanGaliullin/FFixTelegramBot/tree/OWR',
-    author='Vlad Vasilev',
-    author_email='vpvasilev.work@gmail.com',
+    author='Vlad Vasilev, Ruslan Galiullin',
+    author_email='vpvasilev.work@gmail.com, rmgaliullin@edu.hse.ru',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
     include_package_data=True,
     install_requires=['scikit-learn',
                       'huggingsound',
                       'librosa',
```

