# Comparing `tmp/jupyter-references-0.5.tar.gz` & `tmp/jupyter-references-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-references-0.5.tar", last modified: Fri May  5 18:44:54 2023, max compression
+gzip compressed data, was "jupyter-references-0.6.tar", last modified: Sat May  6 09:14:43 2023, max compression
```

## Comparing `jupyter-references-0.5.tar` & `jupyter-references-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.335440 jupyter-references-0.5/
--rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.5/LICENSE
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:44:54.335176 jupyter-references-0.5/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.5/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.327954 jupyter-references-0.5/jupyter_references/
--rw-r--r--   0 kmt        (501) staff       (20)     3632 2023-05-05 18:44:11.000000 jupyter-references-0.5/jupyter_references/__init__.py
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 18:44:54.334792 jupyter-references-0.5/jupyter_references.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/requires.txt
--rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 18:44:54.000000 jupyter-references-0.5/jupyter_references.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 18:44:54.335494 jupyter-references-0.5/setup.cfg
--rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 18:44:19.000000 jupyter-references-0.5/setup.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.446964 jupyter-references-0.6/
+-rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.6/LICENSE
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-06 09:14:43.446724 jupyter-references-0.6/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.6/README.md
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.443013 jupyter-references-0.6/jupyter_references/
+-rw-r--r--   0 kmt        (501) staff       (20)     3904 2023-05-06 09:11:24.000000 jupyter-references-0.6/jupyter_references/__init__.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.446183 jupyter-references-0.6/jupyter_references.egg-info/
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/SOURCES.txt
+-rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/dependency_links.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/requires.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/top_level.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-06 09:14:43.447019 jupyter-references-0.6/setup.cfg
+-rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-06 09:10:58.000000 jupyter-references-0.6/setup.py
```

### Comparing `jupyter-references-0.5/LICENSE` & `jupyter-references-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.5/PKG-INFO` & `jupyter-references-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.5
+Version: 0.6
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.5/README.md` & `jupyter-references-0.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.5/jupyter_references/__init__.py` & `jupyter-references-0.6/jupyter_references/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
         
 import os
+import sys
 import ipynbname
 import json
 import re
 from IPython.lib import clipboard
 from IPython.core.magic import Magics, magics_class, line_magic
 
 @magics_class
@@ -54,15 +55,19 @@
             ref_list = {}
             url, year, title, author = match.groups()
             content = f'{author} et al. [({year})](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")'
             get_ipython().run_line_magic('replace_content', f"{content}") 
         else:
             print('clipboard is not bibtex:', cb)
         
-def reflist(file_base_name=None):
+
+def ref_format_callback(i, ref):
+    return f"{i}. {ref['author']}, {ref['year']}, _{ref['title']}_, [{ref['doi']}](https://doi.org/{ref['doi'].replace('DOI:', '')})"
+
+def reflist(file_base_name=None, format_fun=ref_format_callback):
     regex = re.compile(r'\d+\s+"([^"]+)"')
     references = {}
     if file_base_name is None:
         file_base_name = ipynbname.name()
     if type(file_base_name) is not list:
         file_base_names = [file_base_name]
     else:
@@ -70,20 +75,24 @@
     for name in file_base_names:
         with open(os.path.abspath(name+'.ipynb')) as f:
             notebook_json = json.load(f)
         for cell in notebook_json['cells']:
             if cell['cell_type'] == 'markdown':
                 source = ''.join(cell['source'])
                 for ref in regex.findall(source):
-                    author, year, title, doi = ref.split('\n')
-                    references[ref] = dict(author=author.strip(),
-                                        year=year.strip(), 
-                                        title=title.strip(),
-                                        doi=doi.strip())
+                    try:
+                        author, year, title, doi = ref.split('\n')
+                        references[ref] = dict(author=author.strip(),
+                                            year=year.strip(), 
+                                            title=title.strip(),
+                                            doi=doi.strip())
+                    except ValueError:
+                        print(f'Skipping invalid ref: {ref}', file=sys.stderr)
+
     lst = []
     for i, (key, ref) in enumerate(sorted(references.items())):
-        lst.append(f"{i+1}. {ref['author']}, {ref['year']}, _{ref['title']}_, [{ref['doi']}](https://doi.org/{ref['doi'].replace('DOI:', '')})")
+        lst.append(format_fun(i+1, ref))
     content = "\n".join(lst)
     content = '## References\n\n' + content
     get_ipython().run_line_magic('replace_content', f"{content}")
```

### Comparing `jupyter-references-0.5/jupyter_references.egg-info/PKG-INFO` & `jupyter-references-0.6/jupyter_references.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.5
+Version: 0.6
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.5/setup.py` & `jupyter-references-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 # package name must be the git repository name
 package_name = path.basename(this_directory)
 
 setuptools.setup(
     name=package_name,
-    version="0.5",
+    version="0.6",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Lightweight system for citing papers and making a reference list in jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f'https://github.com/kaspermunch/{package_name}',
     packages=setuptools.find_packages(),
```

