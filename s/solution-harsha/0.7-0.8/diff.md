# Comparing `tmp/solution_harsha-0.7.tar.gz` & `tmp/solution_harsha-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solution_harsha-0.7.tar", last modified: Sat May  6 18:31:17 2023, max compression
+gzip compressed data, was "solution_harsha-0.8.tar", last modified: Sat May  6 18:42:28 2023, max compression
```

## Comparing `solution_harsha-0.7.tar` & `solution_harsha-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.259631 solution_harsha-0.7/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:31:17.258632 solution_harsha-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-05-06 18:25:16.000000 solution_harsha-0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:31:17.259631 solution_harsha-0.7/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-05-06 18:31:10.000000 solution_harsha-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.249638 solution_harsha-0.7/solution_harsha/
--rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.7/solution_harsha/__init__.py
--rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.7/solution_harsha/config.yaml
--rw-rw-rw-   0        0        0     4879 2023-05-06 18:30:39.000000 solution_harsha-0.7/solution_harsha/di_testcode.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:31:17.257632 solution_harsha-0.7/solution_harsha.egg-info/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 18:31:17.000000 solution_harsha-0.7/solution_harsha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.973876 solution_harsha-0.8/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:42:28.973876 solution_harsha-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-05-06 18:25:16.000000 solution_harsha-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:42:28.974893 solution_harsha-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-05-06 18:36:27.000000 solution_harsha-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.963876 solution_harsha-0.8/solution_harsha/
+-rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.8/solution_harsha/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.8/solution_harsha/config.yaml
+-rw-rw-rw-   0        0        0     5021 2023-05-06 18:36:01.000000 solution_harsha-0.8/solution_harsha/di_testcode.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.971877 solution_harsha-0.8/solution_harsha.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/top_level.txt
```

### Comparing `solution_harsha-0.7/README.md` & `solution_harsha-0.8/README.md`

 * *Files identical despite different names*

### Comparing `solution_harsha-0.7/setup.py` & `solution_harsha-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solution_harsha',
-    version='0.7',
+    version='0.8',
     description='A tool for performing string matching on text files',
     author='Sriharsha Aryasomayajula',
     author_email='harshaarya17@outlook.com',
     packages=find_packages(),
     package_data={"": ["config.yaml"]},
     include_package_data=True,
     install_requires=[
```

### Comparing `solution_harsha-0.7/solution_harsha/di_testcode.py` & `solution_harsha-0.8/solution_harsha/di_testcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         with open(self.file_path, "r") as file:
             lines = []
             for line in file: #a simple for loop to collect all the lines into a list. This goes easy on the memory for large files
                 lines.append(line)
             search_term = lines[-1].strip() #stores the last line as the search term
             return search_term,lines
              
-    def check_file_health(self) -> bool:
+    def check_file_health(self) -> None:
         """Checks the file health based on existence and extension of file path. 
         Returns:
         Error message or None."""
         if not Path(self.file_path).is_file(): #checks if it is a valid path 
             return f'{self.file_path} is not a valid file path. Make sure the file exists'
         if not self.file_path.endswith('.txt'): #checks if it is a .txt file
             return f'{self.file_path} is not text file.Please input a text file'
@@ -82,24 +82,24 @@
             if last_line in line: #sub string matching using python "in"
                 clean_line = re.sub(r'[^A-Za-zÀ-ÖØ-öø-ÿäüßàáâãäåæçèéêëìíîïñòóôõöøœùúûüý\s]+', ' ', line) #more filters can be added here
                 filter_list.append(clean_line)
                 print(f'[{clean_line.strip()}]') #output is printed here 
         return filter_list
 
     def run(self) -> None:
-        """Main block of the code."""
+        """Main block of the code.checks the file healthcand returns executes the string_operation function"""
         error_message = self.check_file_health()
         if error_message:
             log.error(error_message)
             return
 
         log.debug('opening a text file')
         last_line, lines_file = self.search_item()
         with open(self.file_path, "r") as file:
-            if not len(self.perform_string_operation(last_line, lines_file)):
+            if not len(self.perform_string_operation(last_line, lines_file)): #this checks if the length of counter is 0 then its prints the error
                 log.error(f'The search_term doesnt exist in the source_text for the file {self.file_path}')
         return None
 
 
 def main():
     """Creates an object of the type class StringMatcher and runs it"""
     stringapp = StringMatcher()
```

