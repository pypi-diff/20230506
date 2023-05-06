# Comparing `tmp/pyaxetool-1.0.0.tar.gz` & `tmp/pyaxetool-1.1.0.tar.gz`

## Comparing `pyaxetool-1.0.0.tar` & `pyaxetool-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/.gitignore
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/LICENSE
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/README.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/TODO.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/MD5.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/PyInstaller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/__main__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/oldbak/MANIFEST.in
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/oldbak/setup.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/.gitignore
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/LICENSE
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/TODO.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/CMake.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/MD5.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/PyInstaller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/oldbak/MANIFEST.in
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/oldbak/setup.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PKG-INFO
```

### Comparing `pyaxetool-1.0.0/.gitignore` & `pyaxetool-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.0.0/LICENSE` & `pyaxetool-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.0.0/PyAxeTool/MD5.py` & `pyaxetool-1.1.0/PyAxeTool/MD5.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.0.0/PyAxeTool/PyInstaller.py` & `pyaxetool-1.1.0/PyAxeTool/PyInstaller.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.0.0/oldbak/setup.py` & `pyaxetool-1.1.0/oldbak/setup.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.0.0/PKG-INFO` & `pyaxetool-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyaxetool
-Version: 1.0.0
+Version: 1.1.0
 Summary: An utility tool collection for make life easily
 Project-URL: Bug Tracker, https://github.com/sunjinopensource/PyAxeTool/issues
 Project-URL: Homepage, https://github.com/sunjinopensource/PyAxeTool
 Author-email: Sun Jin <412640665@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Requires-Dist: pyaxe>=1.0.32
 Description-Content-Type: text/markdown
 
 PyAxeTool
 =========
 
 An utility tool collection for make life easily.
 
@@ -26,8 +27,11 @@
 python3 -m PyAxeTool.MD5 file "*.txt"
 
 # 显示目录内所有文件汇总的单个MD5
 python3 -m PyAxeTool.MD5 dir testdir
 
 # 显示字符串的MD5
 python3 -m PyAxeTool.MD5 str abc
+
+# 通过lib模板创建CMake工程
+python3 -m PyAxeTool.CMake archetype:generate lib --libname=foo
 ```
```

