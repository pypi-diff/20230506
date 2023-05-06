# Comparing `tmp/didicli-0.0.8.tar.gz` & `tmp/didicli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didicli-0.0.8.tar", last modified: Thu Apr 20 10:04:26 2023, max compression
+gzip compressed data, was "didicli-0.0.9.tar", last modified: Thu Apr 20 10:11:59 2023, max compression
```

## Comparing `didicli-0.0.8.tar` & `didicli-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:04:26.817740 didicli-0.0.8/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      335 2023-04-20 10:04:26.817348 didicli-0.0.8/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-04-20 09:08:52.000000 didicli-0.0.8/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:04:26.816725 didicli-0.0.8/didicli.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      335 2023-04-20 10:04:26.000000 didicli-0.0.8/didicli.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      191 2023-04-20 10:04:26.000000 didicli-0.0.8/didicli.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 10:04:26.000000 didicli-0.0.8/didicli.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-04-20 10:04:26.000000 didicli-0.0.8/didicli.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 10:04:26.000000 didicli-0.0.8/didicli.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      275 2023-04-20 09:10:57.000000 didicli-0.0.8/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 10:04:26.817859 didicli-0.0.8/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1174 2023-04-20 10:04:04.000000 didicli-0.0.8/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.332564 didicli-0.0.9/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      335 2023-04-20 10:11:59.332290 didicli-0.0.9/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-04-20 09:08:52.000000 didicli-0.0.9/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.327977 didicli-0.0.9/didicli.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      335 2023-04-20 10:11:59.000000 didicli-0.0.9/didicli.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      375 2023-04-20 10:11:59.000000 didicli-0.0.9/didicli.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 10:11:59.000000 didicli-0.0.9/didicli.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-04-20 10:11:59.000000 didicli-0.0.9/didicli.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        7 2023-04-20 10:11:59.000000 didicli-0.0.9/didicli.egg-info/top_level.txt
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.329332 didicli-0.0.9/didigo/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-20 08:49:33.000000 didicli-0.0.9/didigo/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3129 2023-04-20 09:46:16.000000 didicli-0.0.9/didigo/cli.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      936 2023-04-20 09:27:25.000000 didicli-0.0.9/didigo/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.330153 didicli-0.0.9/didigo/constant/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-20 09:45:40.000000 didicli-0.0.9/didigo/constant/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       63 2023-04-20 10:11:53.000000 didicli-0.0.9/didigo/constant/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.331037 didicli-0.0.9/didigo/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 didicli-0.0.9/didigo/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 didicli-0.0.9/didigo/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 10:11:59.331626 didicli-0.0.9/didigo/version/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      383 2023-04-20 09:46:16.000000 didicli-0.0.9/didigo/version/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      275 2023-04-20 09:10:57.000000 didicli-0.0.9/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 10:11:59.332664 didicli-0.0.9/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1204 2023-04-20 10:11:41.000000 didicli-0.0.9/setup.py
```

### Comparing `didicli-0.0.8/setup.py` & `didicli-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     long_description= utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='didicli contributors',
     author_email='myname@example.com',
     keywords='didicli,  ll',
     url='https://github.com/xxx/xxxx',
     # packages=find_packages(exclude=('configs', 'tools', 'demo')),
+    packages=find_packages(),
     include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
     ],
     license='Apache License 2.0',
     # install_requires=utils.parse_requirements('requirements/runtime.txt'),
     # extras_require={
```

