# Comparing `tmp/solution_harsha-0.6.tar.gz` & `tmp/solution_harsha-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solution_harsha-0.6.tar", last modified: Sat May  6 18:28:07 2023, max compression
+gzip compressed data, was "solution_harsha-0.7.tar", last modified: Sat May  6 18:31:17 2023, max compression
```

## Comparing `solution_harsha-0.6.tar` & `solution_harsha-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:28:07.662260 solution_harsha-0.6/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:28:07.661260 solution_harsha-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-05-06 18:25:16.000000 solution_harsha-0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:28:07.662260 solution_harsha-0.6/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-05-06 18:27:54.000000 solution_harsha-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:28:07.652264 solution_harsha-0.6/solution_harsha/
--rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.6/solution_harsha/__init__.py
--rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.6/solution_harsha/config.yaml
--rw-rw-rw-   0        0        0     4815 2023-05-06 18:21:28.000000 solution_harsha-0.6/solution_harsha/di_testcode.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:28:07.660284 solution_harsha-0.6/solution_harsha.egg-info/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 18:28:07.000000 solution_harsha-0.6/solution_harsha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.259631 solution_harsha-0.7/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:31:17.258632 solution_harsha-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-05-06 18:25:16.000000 solution_harsha-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:31:17.259631 solution_harsha-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-05-06 18:31:10.000000 solution_harsha-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.249638 solution_harsha-0.7/solution_harsha/
+-rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.7/solution_harsha/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.7/solution_harsha/config.yaml
+-rw-rw-rw-   0        0        0     4879 2023-05-06 18:30:39.000000 solution_harsha-0.7/solution_harsha/di_testcode.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.257632 solution_harsha-0.7/solution_harsha.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/top_level.txt
```

### Comparing `solution_harsha-0.6/README.md` & `solution_harsha-0.7/README.md`

 * *Files identical despite different names*

### Comparing `solution_harsha-0.6/setup.py` & `solution_harsha-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solution_harsha',
-    version='0.6',
+    version='0.7',
     description='A tool for performing string matching on text files',
     author='Sriharsha Aryasomayajula',
     author_email='harshaarya17@outlook.com',
     packages=find_packages(),
     package_data={"": ["config.yaml"]},
     include_package_data=True,
     install_requires=[
```

### Comparing `solution_harsha-0.6/solution_harsha/di_testcode.py` & `solution_harsha-0.7/solution_harsha/di_testcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def perform_string_operation(self, last_line: str,lines_file: list) -> list:
         """Performs string operation by matching last line with each line in the file and does some regex filtering to avoid numerical,special characters. 
         Returns
         print statement."""
         filter_list = []
         for line in lines_file[:-1]: #this for loop go through all the lines except the last line in the file
             if last_line in line: #sub string matching using python "in"
-                clean_line = re.sub(r'[^A-Za-zÀ-ÖØ-öø-ÿ\s]+', ' ', line) #more filters can be added here
+                clean_line = re.sub(r'[^A-Za-zÀ-ÖØ-öø-ÿäüßàáâãäåæçèéêëìíîïñòóôõöøœùúûüý\s]+', ' ', line) #more filters can be added here
                 filter_list.append(clean_line)
                 print(f'[{clean_line.strip()}]') #output is printed here 
         return filter_list
 
     def run(self) -> None:
         """Main block of the code."""
         error_message = self.check_file_health()
```

