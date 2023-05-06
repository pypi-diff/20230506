# Comparing `tmp/solution_harsha-0.8.tar.gz` & `tmp/solution_harsha-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solution_harsha-0.8.tar", last modified: Sat May  6 18:42:28 2023, max compression
+gzip compressed data, was "solution_harsha-0.9.tar", last modified: Sat May  6 19:27:05 2023, max compression
```

## Comparing `solution_harsha-0.8.tar` & `solution_harsha-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.973876 solution_harsha-0.8/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:42:28.973876 solution_harsha-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-05-06 18:25:16.000000 solution_harsha-0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:42:28.974893 solution_harsha-0.8/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-05-06 18:36:27.000000 solution_harsha-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.963876 solution_harsha-0.8/solution_harsha/
--rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.8/solution_harsha/__init__.py
--rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.8/solution_harsha/config.yaml
--rw-rw-rw-   0        0        0     5021 2023-05-06 18:36:01.000000 solution_harsha-0.8/solution_harsha/di_testcode.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:42:28.971877 solution_harsha-0.8/solution_harsha.egg-info/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 18:42:28.000000 solution_harsha-0.8/solution_harsha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:05.578295 solution_harsha-0.9/
+-rw-rw-rw-   0        0        0      196 2023-05-06 19:27:05.577298 solution_harsha-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3958 2023-05-06 19:20:11.000000 solution_harsha-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:27:05.578295 solution_harsha-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-05-06 19:26:56.000000 solution_harsha-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:05.566299 solution_harsha-0.9/solution_harsha/
+-rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.9/solution_harsha/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-05-06 18:23:24.000000 solution_harsha-0.9/solution_harsha/config.yaml
+-rw-rw-rw-   0        0        0     4907 2023-05-06 19:24:44.000000 solution_harsha-0.9/solution_harsha/di_testcode.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:05.575300 solution_harsha-0.9/solution_harsha.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:27:05.000000 solution_harsha-0.9/solution_harsha.egg-info/top_level.txt
```

### Comparing `solution_harsha-0.8/README.md` & `solution_harsha-0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Deeper Insights Test Code Repo
 deeper insights test code
 
 This program lets user pass a textfile path as a arguement to the script.
-The script then looks for the search term in the last line of the file and looks for that search item in the other lines of the file.
+The script then looks for the search term in the last line of the file and looks for that search item in the other lines of the file. 
+
+Clone this repo first 
 
 **USER HELP** - Use the help function by running -h as an arguement to the program
 
 **DEVELOPER HELP** - Please refer to comments and doc strings in the di_testcode.py file
 
 The file should be a txt file
 
@@ -18,49 +20,59 @@
 
 **TEST CASE USAGE**
 
 In order to use the test case set the debug parameter in config.yaml to True and add the path directly in the path parameter of config.yaml
 
     python test.py  
 
-The whole solution was packaged. Although Clare Walsh suggested i leave as it is. I wanted to package the solution. These are the steps I followed to package it into solution. 
+> Please keep in mind to change the test parameter in the config.yaml to False while actually running the app. Its only meant to be True when you are running test cases.
+
+**The whole solution was packaged. Although Clare Walsh suggested i leave as it is. I wanted to package the solution. These are the steps I followed to package it into solution.** 
 
 1. create a setup.py with all the requirements in the first directory.
 2. added all dependencies to requirements.txt
 3. build the package using 
 
-    python setup.py sdist bdist_wheel
+        python setup.py sdist bdist_wheel
 
 4. uploaded the build distribution to Pypi using
 
-    twine upload dist/*
+        twine upload dist/*
 
-5. This is available on https://pypi.org/project/solution-harsha/0.5/ To install this use this command
+5. This is available on https://pypi.org/project/solution-harsha/ To install this use this command
 
-    pip install solution-harsha
+        pip install solution-harsha
 
 6. To install this package run this command 
 
-    pip install solution_harsha
+        pip install solution_harsha
 
 7. After installing run this command with path to the text file and get result. 
 
-    stringapp_di <<path_of_the_file>>
+        stringapp_di <<path_of_the_file>>
 
-    **for some bizzare reason I don't know why this prints the result twice**
+    **for some reason I don't know why this prints the result twice**
 
-Since I have confirmed with the Clare Walsh 
+> I didn't fix the issue of the solution printing the result twice when run from installed package.When run using the script manually it worKs just fine. I have confirmed with the Clare Walsh and she said it is okay if the solution IS to be executed manually using python script
+Example :- python solution.py <file_path>. If you run the code directly without the package command line then it works normally.  
 
 Assumptions:
-The search term is always a alphabetical string. It never has any numbers in it.  As described in the problem statement it is a word. It takes special characters like german umlaut, greek alphabets (I have checked with Clare Walsh and she confirmed this)
+---------------
+
+The user has python 3 and uses linux or windows OS. (I have checked with Clare Walsh and she confirmed this that I can assume the user environment)
 
-Or the search_term can be dirty and it would shall need cleaning before using it as search term. ( I have checked with Clare Walsh and she confirmed this)
+The search term is always an alphabetical string. It never has any numbers in it.  As described in the problem statement it is a word. It takes special characters like german umlaut, greek alphabets, and romance language letters. But from my testing experience it doesnt print that result properly in the terminal.
+
+Or the search_term can be dirty and it shall need cleaning before using it as search term. ( I have checked with Clare Walsh and she confirmed this)
 
 This program runs on python3 not python2.7 as it no longer has support. 
 
 File is a text file as this is a basic program that checks for text files. (I have checked with Clare Walsh and she confirmed this)
 
 There are no empty lines between the search term and source text. 
 
-Also what happens if there are no search terms in source files? Its just means the program can return a statement to the user saying "No search_term found in the source_text". The drawback being its going to do it everytime 
+Files will fit into memory. (I have checked with Clare Walsh and she confirmed this)
+
+Also what happens if there are no search terms in source files? Its just means the program can log an error to the user saying "The search_term doesnt exist in the source_text for the file <path_of_file>". 
 
+Originally I wanted to write this is a docker file. But I wasnt sure if this application would be used in cloud or user has docker installed. I confirmed with Clare Walsh that I can put it in readme saying assume user has docker. But I ultimately decided not to do docker container for this application and instead made a pip package. Although the package has a bug, I am more than willing to learn from people on solving the issue.
```

### Comparing `solution_harsha-0.8/setup.py` & `solution_harsha-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solution_harsha',
-    version='0.8',
+    version='0.9',
     description='A tool for performing string matching on text files',
     author='Sriharsha Aryasomayajula',
     author_email='harshaarya17@outlook.com',
     packages=find_packages(),
     package_data={"": ["config.yaml"]},
     include_package_data=True,
     install_requires=[
```

### Comparing `solution_harsha-0.8/solution_harsha/di_testcode.py` & `solution_harsha-0.9/solution_harsha/di_testcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,14 @@
     argparse.ArgumentParser object: A configured argument parser object."""
     parser = ArgumentParser(add_help=False)
     args = parser.add_argument_group('Options')
     args.add_argument('-h','--help',action='help',help = 'Please follow the readme.md file for instructions on how to run this program') #adds a -h flag to help the user with the program
     args.add_argument('file',help = 'Required. Path to an .txt file')
     return parser
 
-
-#if and else statement with yaml config to describe what the status is
-#package this into a pip cli package
-
 class StringMatcher():
     """A simple switch case to decide what to use as file path depending on the configuration from config.yaml"""
     def __init__(self) -> None:
         if debug == False:
             self.args = build_argparser().parse_args()
             self.file_path = self.args.file
         else:
```

