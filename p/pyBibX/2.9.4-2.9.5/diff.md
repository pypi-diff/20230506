# Comparing `tmp/pyBibX-2.9.4.tar.gz` & `tmp/pyBibX-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.4.tar", last modified: Fri May  5 20:48:44 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.5.tar", last modified: Fri May  5 22:38:26 2023, max compression
```

## Comparing `pyBibX-2.9.4.tar` & `pyBibX-2.9.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.4/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9127 2023-05-05 20:48:44.000000 pyBibX-2.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     8690 2023-05-02 21:59:33.000000 pyBibX-2.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.4/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.4/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   263868 2023-05-05 20:47:14.000000 pyBibX-2.9.4/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.4/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9127 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-05 20:48:44.000000 pyBibX-2.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-05-05 20:48:21.000000 pyBibX-2.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:38:26.000000 pyBibX-2.9.5/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.5/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9127 2023-05-05 22:38:26.000000 pyBibX-2.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8690 2023-05-02 21:59:33.000000 pyBibX-2.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 22:38:26.000000 pyBibX-2.9.5/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.5/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:38:26.000000 pyBibX-2.9.5/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.5/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   264093 2023-05-05 22:34:06.000000 pyBibX-2.9.5/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:38:26.000000 pyBibX-2.9.5/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.5/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:38:26.000000 pyBibX-2.9.5/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9127 2023-05-05 22:38:25.000000 pyBibX-2.9.5/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-05-05 22:38:26.000000 pyBibX-2.9.5/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 22:38:25.000000 pyBibX-2.9.5/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-05 22:38:25.000000 pyBibX-2.9.5/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 22:38:25.000000 pyBibX-2.9.5/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 22:38:25.000000 pyBibX-2.9.5/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-05 22:38:26.000000 pyBibX-2.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-05-05 22:38:18.000000 pyBibX-2.9.5/setup.py
```

### Comparing `pyBibX-2.9.4/LICENSE` & `pyBibX-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/PKG-INFO` & `pyBibX-2.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.4
+Version: 2.9.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.4/README.md` & `pyBibX-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/pbx.py` & `pyBibX-2.9.5/pyBibX/base/pbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -921,14 +921,18 @@
                 rhs.append('WoS')
             doc = doc + 1
           if (f_list[i].find('=') != -1 and f_list[i].find(' ') != 0):
             lhs.append(f_list[i].split('=')[0].lower().strip())
             rhs.append(f_list[i].split('=')[1].replace('{', '').replace('},', '').replace('}', '').replace('}},', '').strip())
           elif (f_list[i].find(' ') == 0 and i!= 0 and rhs[-1] != 'doc_start'):
             rhs[-1] = rhs[-1]+' '+f_list[i].replace('{', '').replace('},', '').replace('}', '').replace('}},', '').strip()
+        if (db == 'scopus' and 'abbrev_source_title' not in lhs and 'journal' in lhs):
+            for i in range(0, len(lhs)):
+                if (lhs[i] == 'journal'):
+                    lhs[i] = 'abbrev_source_title'
         if (db == 'wos'):
             for i in range(0, len(lhs)):
                 if (lhs[i] == 'affiliation'):
                     lhs[i] = 'affiliation_'
                 if (lhs[i] == 'affiliations'):
                     lhs[i] = 'affiliation'
                 if (lhs[i] == 'article-number'):
```

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.5/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.5/pyBibX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.4
+Version: 2.9.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.4/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.5/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.4/setup.py` & `pyBibX-2.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.4',
+    version='2.9.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

