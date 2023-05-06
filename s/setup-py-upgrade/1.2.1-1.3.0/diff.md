# Comparing `tmp/setup_py_upgrade-1.2.1.tar.gz` & `tmp/setup_py_upgrade-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setup_py_upgrade-1.2.1.tar", last modified: Thu Oct  8 17:17:24 2020, max compression
+gzip compressed data, was "setup_py_upgrade-1.3.0.tar", last modified: Sat May  6 21:17:04 2023, max compression
```

## Comparing `setup_py_upgrade-1.2.1.tar` & `setup_py_upgrade-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2020-10-08 17:17:24.239836 setup_py_upgrade-1.2.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2020-10-08 16:56:09.000000 setup_py_upgrade-1.2.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5112 2020-10-08 17:17:24.239836 setup_py_upgrade-1.2.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3472 2020-10-08 16:56:09.000000 setup_py_upgrade-1.2.1/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1095 2020-10-08 17:17:24.239836 setup_py_upgrade-1.2.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2020-10-08 16:56:09.000000 setup_py_upgrade-1.2.1/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2020-10-08 17:17:24.239836 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5112 2020-10-08 17:17:23.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      259 2020-10-08 17:17:24.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2020-10-08 17:17:23.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       60 2020-10-08 17:17:23.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2020-10-08 17:17:23.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8417 2020-10-08 17:16:33.000000 setup_py_upgrade-1.2.1/setup_py_upgrade.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3432 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1064 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      259 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       59 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8552 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.py
```

### Comparing `setup_py_upgrade-1.2.1/LICENSE` & `setup_py_upgrade-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_py_upgrade-1.2.1/PKG-INFO` & `setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,143 @@
 Metadata-Version: 2.1
-Name: setup_py_upgrade
-Version: 1.2.1
+Name: setup-py-upgrade
+Version: 1.3.0
 Summary: upgrade a setup.py to declarative metadata
 Home-page: https://github.com/asottile/setup-py-upgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Description: [![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-py-upgrade?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
-        [![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/37/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
-        
-        setup-py-upgrade
-        ================
-        
-        upgrade a setup.py to declarative metadata
-        
-        ## installation
-        
-        `pip install setup-py-upgrade`
-        
-        ## cli
-        
-        Consult the help for the latest usage:
-        
-        ```console
-        $ setup-py-upgrade --help
-        usage: setup-py-upgrade [-h] directory
-        
-        positional arguments:
-          directory
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        pass the root directory of the repository you'd like to convert
-        
-        the script overwrites `setup.py` and `setup.cfg` when run
-        
-        ## sample output
-        
-        ```console
-        $ setup-py-upgrade ../pre-commit
-        ../pre-commit/setup.py and ../pre-commit/setup.cfg written!
-        $ tail -n999 ../pre-commit/setup.{py,cfg}
-        ==> ../pre-commit/setup.py <==
-        from setuptools import setup
-        setup()
-        
-        ==> ../pre-commit/setup.cfg <==
-        [metadata]
-        name = pre_commit
-        description = A framework for managing and maintaining multi-language pre-commit hooks.
-        long_description = file: README.md
-        long_description_content_type = text/markdown
-        url = https://github.com/pre-commit/pre-commit
-        version = 1.14.2
-        author = Anthony Sottile
-        author_email = asottile@umich.edu
-        classifiers =
-            License :: OSI Approved :: MIT License
-            Programming Language :: Python :: 2
-            Programming Language :: Python :: 2.7
-            Programming Language :: Python :: 3
-            Programming Language :: Python :: 3.6
-            Programming Language :: Python :: 3.7
-            Programming Language :: Python :: Implementation :: CPython
-            Programming Language :: Python :: Implementation :: PyPy
-        
-        [options]
-        packages = find:
-        install_requires =
-            aspy.yaml
-            cfgv>=1.4.0
-            identify>=1.0.0
-            importlib-metadata
-            nodeenv>=0.11.1
-            pyyaml
-            six
-            toml
-            virtualenv
-            futures; python_version<"3.2"
-            importlib-resources; python_version<"3.7"
-        
-        [options.packages.find]
-        exclude =
-            tests*
-            testing*
-        
-        [options.entry_points]
-        console_scripts =
-            pre-commit = pre_commit.main:main
-            pre-commit-validate-config = pre_commit.clientlib:validate_config_main
-            pre-commit-validate-manifest = pre_commit.clientlib:validate_manifest_main
-        
-        [options.package_data]
-        pre_commit.resources =
-            *.tar.gz
-            empty_template_*
-            hook-tmpl
-        
-        [bdist_wheel]
-        universal = True
-        ```
-        
-        ## what versions of setuptools / pip does the output work with?
-        
-        - `pip>=1.5` (when installing from a wheel)
-            - released 2014-01-02
-        - `setuptools>=30.3` (when building from source)
-            - released 2016-12-08
-        - `virtualenv>=15.2` (to get a sufficient setuptools via `--no-download`)
-           - released 2018-03-21
-        
-        ## what is not supported
-        
-        declarative metadata does not support `ext_modules` or setuptools plugins --
-        those must stay in `setup.py`.  If you're converting a project which uses one
-        of those, you'll see a message like:
-        
-        ```console
-        $ setup-py-upgrade ../future-breakpoint/
-        ext_modules= is not supported in setup.cfg
-        ```
-        
-        To convert those, temporarily remove the offending constructs from `setup.py`,
-        then run `setup-py-upgrade`, then paste them back into the file.
-        
-        ## related projects
-        
-        - [setup-cfg-fmt]: apply a consistent format to `setup.cfg` files
-        
-        [setup-cfg-fmt]: https://github.com/asottile/setup-cfg-fmt
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6.1
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![build status](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-py-upgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-py-upgrade/main)
+
+setup-py-upgrade
+================
+
+upgrade a setup.py to declarative metadata
+
+## installation
+
+```bash
+pip install setup-py-upgrade
+```
+
+## cli
+
+Consult the help for the latest usage:
+
+```console
+$ setup-py-upgrade --help
+usage: setup-py-upgrade [-h] directory
+
+positional arguments:
+  directory
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+pass the root directory of the repository you'd like to convert
+
+the script overwrites `setup.py` and `setup.cfg` when run
+
+## sample output
+
+```console
+$ setup-py-upgrade ../pre-commit
+../pre-commit/setup.py and ../pre-commit/setup.cfg written!
+$ tail -n999 ../pre-commit/setup.{py,cfg}
+==> ../pre-commit/setup.py <==
+from setuptools import setup
+setup()
+
+==> ../pre-commit/setup.cfg <==
+[metadata]
+name = pre_commit
+description = A framework for managing and maintaining multi-language pre-commit hooks.
+long_description = file: README.md
+long_description_content_type = text/markdown
+url = https://github.com/pre-commit/pre-commit
+version = 1.14.2
+author = Anthony Sottile
+author_email = asottile@umich.edu
+classifiers =
+    License :: OSI Approved :: MIT License
+    Programming Language :: Python :: 2
+    Programming Language :: Python :: 2.7
+    Programming Language :: Python :: 3
+    Programming Language :: Python :: 3.6
+    Programming Language :: Python :: 3.7
+    Programming Language :: Python :: Implementation :: CPython
+    Programming Language :: Python :: Implementation :: PyPy
+
+[options]
+packages = find:
+install_requires =
+    aspy.yaml
+    cfgv>=1.4.0
+    identify>=1.0.0
+    importlib-metadata
+    nodeenv>=0.11.1
+    pyyaml
+    six
+    toml
+    virtualenv
+    futures; python_version<"3.2"
+    importlib-resources; python_version<"3.7"
+
+[options.packages.find]
+exclude =
+    tests*
+    testing*
+
+[options.entry_points]
+console_scripts =
+    pre-commit = pre_commit.main:main
+    pre-commit-validate-config = pre_commit.clientlib:validate_config_main
+    pre-commit-validate-manifest = pre_commit.clientlib:validate_manifest_main
+
+[options.package_data]
+pre_commit.resources =
+    *.tar.gz
+    empty_template_*
+    hook-tmpl
+
+[bdist_wheel]
+universal = True
+```
+
+## what versions of setuptools / pip does the output work with?
+
+- `pip>=1.5` (when installing from a wheel)
+    - released 2014-01-02
+- `setuptools>=30.3` (when building from source)
+    - released 2016-12-08
+- `virtualenv>=15.2` (to get a sufficient setuptools via `--no-download`)
+   - released 2018-03-21
+
+## what is not supported
+
+declarative metadata does not support `ext_modules` or setuptools plugins --
+those must stay in `setup.py`.  If you're converting a project which uses one
+of those, you'll see a message like:
+
+```console
+$ setup-py-upgrade ../future-breakpoint/
+ext_modules= is not supported in setup.cfg
+```
+
+To convert those, temporarily remove the offending constructs from `setup.py`,
+then run `setup-py-upgrade`, then paste them back into the file.
+
+## related projects
+
+- [setup-cfg-fmt]: apply a consistent format to `setup.cfg` files
+
+[setup-cfg-fmt]: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `setup_py_upgrade-1.2.1/README.md` & `setup_py_upgrade-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-py-upgrade?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/37/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
+[![build status](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-py-upgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-py-upgrade/main)
 
 setup-py-upgrade
 ================
 
 upgrade a setup.py to declarative metadata
 
 ## installation
 
-`pip install setup-py-upgrade`
+```bash
+pip install setup-py-upgrade
+```
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
 $ setup-py-upgrade --help
```

### Comparing `setup_py_upgrade-1.2.1/setup.cfg` & `setup_py_upgrade-1.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [metadata]
 name = setup_py_upgrade
-version = 1.2.1
+version = 1.3.0
 description = upgrade a setup.py to declarative metadata
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setup-py-upgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 py_modules = setup_py_upgrade
-python_requires = >=3.6.1
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	setup-py-upgrade=setup_py_upgrade:main
 
 [bdist_wheel]
 universal = True
@@ -32,15 +30,16 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
+warn_redundant_casts = true
+warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
 disallow_untyped_defs = false
```

### Comparing `setup_py_upgrade-1.2.1/setup_py_upgrade.egg-info/PKG-INFO` & `setup_py_upgrade-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,143 +1,143 @@
 Metadata-Version: 2.1
-Name: setup-py-upgrade
-Version: 1.2.1
+Name: setup_py_upgrade
+Version: 1.3.0
 Summary: upgrade a setup.py to declarative metadata
 Home-page: https://github.com/asottile/setup-py-upgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Description: [![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.setup-py-upgrade?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
-        [![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/37/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=37&branchName=master)
-        
-        setup-py-upgrade
-        ================
-        
-        upgrade a setup.py to declarative metadata
-        
-        ## installation
-        
-        `pip install setup-py-upgrade`
-        
-        ## cli
-        
-        Consult the help for the latest usage:
-        
-        ```console
-        $ setup-py-upgrade --help
-        usage: setup-py-upgrade [-h] directory
-        
-        positional arguments:
-          directory
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        pass the root directory of the repository you'd like to convert
-        
-        the script overwrites `setup.py` and `setup.cfg` when run
-        
-        ## sample output
-        
-        ```console
-        $ setup-py-upgrade ../pre-commit
-        ../pre-commit/setup.py and ../pre-commit/setup.cfg written!
-        $ tail -n999 ../pre-commit/setup.{py,cfg}
-        ==> ../pre-commit/setup.py <==
-        from setuptools import setup
-        setup()
-        
-        ==> ../pre-commit/setup.cfg <==
-        [metadata]
-        name = pre_commit
-        description = A framework for managing and maintaining multi-language pre-commit hooks.
-        long_description = file: README.md
-        long_description_content_type = text/markdown
-        url = https://github.com/pre-commit/pre-commit
-        version = 1.14.2
-        author = Anthony Sottile
-        author_email = asottile@umich.edu
-        classifiers =
-            License :: OSI Approved :: MIT License
-            Programming Language :: Python :: 2
-            Programming Language :: Python :: 2.7
-            Programming Language :: Python :: 3
-            Programming Language :: Python :: 3.6
-            Programming Language :: Python :: 3.7
-            Programming Language :: Python :: Implementation :: CPython
-            Programming Language :: Python :: Implementation :: PyPy
-        
-        [options]
-        packages = find:
-        install_requires =
-            aspy.yaml
-            cfgv>=1.4.0
-            identify>=1.0.0
-            importlib-metadata
-            nodeenv>=0.11.1
-            pyyaml
-            six
-            toml
-            virtualenv
-            futures; python_version<"3.2"
-            importlib-resources; python_version<"3.7"
-        
-        [options.packages.find]
-        exclude =
-            tests*
-            testing*
-        
-        [options.entry_points]
-        console_scripts =
-            pre-commit = pre_commit.main:main
-            pre-commit-validate-config = pre_commit.clientlib:validate_config_main
-            pre-commit-validate-manifest = pre_commit.clientlib:validate_manifest_main
-        
-        [options.package_data]
-        pre_commit.resources =
-            *.tar.gz
-            empty_template_*
-            hook-tmpl
-        
-        [bdist_wheel]
-        universal = True
-        ```
-        
-        ## what versions of setuptools / pip does the output work with?
-        
-        - `pip>=1.5` (when installing from a wheel)
-            - released 2014-01-02
-        - `setuptools>=30.3` (when building from source)
-            - released 2016-12-08
-        - `virtualenv>=15.2` (to get a sufficient setuptools via `--no-download`)
-           - released 2018-03-21
-        
-        ## what is not supported
-        
-        declarative metadata does not support `ext_modules` or setuptools plugins --
-        those must stay in `setup.py`.  If you're converting a project which uses one
-        of those, you'll see a message like:
-        
-        ```console
-        $ setup-py-upgrade ../future-breakpoint/
-        ext_modules= is not supported in setup.cfg
-        ```
-        
-        To convert those, temporarily remove the offending constructs from `setup.py`,
-        then run `setup-py-upgrade`, then paste them back into the file.
-        
-        ## related projects
-        
-        - [setup-cfg-fmt]: apply a consistent format to `setup.cfg` files
-        
-        [setup-cfg-fmt]: https://github.com/asottile/setup-cfg-fmt
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6.1
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![build status](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-py-upgrade/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-py-upgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-py-upgrade/main)
+
+setup-py-upgrade
+================
+
+upgrade a setup.py to declarative metadata
+
+## installation
+
+```bash
+pip install setup-py-upgrade
+```
+
+## cli
+
+Consult the help for the latest usage:
+
+```console
+$ setup-py-upgrade --help
+usage: setup-py-upgrade [-h] directory
+
+positional arguments:
+  directory
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+pass the root directory of the repository you'd like to convert
+
+the script overwrites `setup.py` and `setup.cfg` when run
+
+## sample output
+
+```console
+$ setup-py-upgrade ../pre-commit
+../pre-commit/setup.py and ../pre-commit/setup.cfg written!
+$ tail -n999 ../pre-commit/setup.{py,cfg}
+==> ../pre-commit/setup.py <==
+from setuptools import setup
+setup()
+
+==> ../pre-commit/setup.cfg <==
+[metadata]
+name = pre_commit
+description = A framework for managing and maintaining multi-language pre-commit hooks.
+long_description = file: README.md
+long_description_content_type = text/markdown
+url = https://github.com/pre-commit/pre-commit
+version = 1.14.2
+author = Anthony Sottile
+author_email = asottile@umich.edu
+classifiers =
+    License :: OSI Approved :: MIT License
+    Programming Language :: Python :: 2
+    Programming Language :: Python :: 2.7
+    Programming Language :: Python :: 3
+    Programming Language :: Python :: 3.6
+    Programming Language :: Python :: 3.7
+    Programming Language :: Python :: Implementation :: CPython
+    Programming Language :: Python :: Implementation :: PyPy
+
+[options]
+packages = find:
+install_requires =
+    aspy.yaml
+    cfgv>=1.4.0
+    identify>=1.0.0
+    importlib-metadata
+    nodeenv>=0.11.1
+    pyyaml
+    six
+    toml
+    virtualenv
+    futures; python_version<"3.2"
+    importlib-resources; python_version<"3.7"
+
+[options.packages.find]
+exclude =
+    tests*
+    testing*
+
+[options.entry_points]
+console_scripts =
+    pre-commit = pre_commit.main:main
+    pre-commit-validate-config = pre_commit.clientlib:validate_config_main
+    pre-commit-validate-manifest = pre_commit.clientlib:validate_manifest_main
+
+[options.package_data]
+pre_commit.resources =
+    *.tar.gz
+    empty_template_*
+    hook-tmpl
+
+[bdist_wheel]
+universal = True
+```
+
+## what versions of setuptools / pip does the output work with?
+
+- `pip>=1.5` (when installing from a wheel)
+    - released 2014-01-02
+- `setuptools>=30.3` (when building from source)
+    - released 2016-12-08
+- `virtualenv>=15.2` (to get a sufficient setuptools via `--no-download`)
+   - released 2018-03-21
+
+## what is not supported
+
+declarative metadata does not support `ext_modules` or setuptools plugins --
+those must stay in `setup.py`.  If you're converting a project which uses one
+of those, you'll see a message like:
+
+```console
+$ setup-py-upgrade ../future-breakpoint/
+ext_modules= is not supported in setup.cfg
+```
+
+To convert those, temporarily remove the offending constructs from `setup.py`,
+then run `setup-py-upgrade`, then paste them back into the file.
+
+## related projects
+
+- [setup-cfg-fmt]: apply a consistent format to `setup.cfg` files
+
+[setup-cfg-fmt]: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `setup_py_upgrade-1.2.1/setup_py_upgrade.py` & `setup_py_upgrade-1.3.0/setup_py_upgrade.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from __future__ import annotations
+
 import argparse
 import ast
 import configparser
 import io
 import os.path
 from typing import Any
-from typing import Dict
-from typing import Optional
 from typing import Sequence
 
 METADATA_KEYS = frozenset((
     'name', 'version', 'url', 'download_url', 'project_urls', 'author',
     'author_email', 'maintainer', 'maintainer_email', 'classifiers',
     'license', 'license_file', 'description', 'long_description',
     'long_description_content_type', 'keywords', 'platforms', 'provides',
@@ -43,32 +43,36 @@
             node.func.attr == attr
         )
     )
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self) -> None:
-        self.sections: Dict[str, Dict[str, Any]] = {}
+        self.sections: dict[str, dict[str, Any]] = {}
         self.sections['metadata'] = {}
         self.sections['options'] = {}
 
-        self._files: Dict[str, str] = {}
+        self._files: dict[str, str] = {}
 
     def visit_With(self, node: ast.With) -> None:
         # with open("filename", ...) as fvar:
         #     varname = fvar.read()
         if (
                 # with open(...)
                 len(node.items) == 1 and
                 isinstance(node.items[0].context_expr, ast.Call) and
                 isinstance(node.items[0].context_expr.func, ast.Name) and
                 node.items[0].context_expr.func.id == 'open' and
                 # "filename"
                 len(node.items[0].context_expr.args) > 0 and
-                isinstance(node.items[0].context_expr.args[0], ast.Str) and
+                isinstance(
+                    node.items[0].context_expr.args[0],
+                    ast.Constant,
+                ) and
+                isinstance(node.items[0].context_expr.args[0].value, str) and
                 # as fvar
                 isinstance(node.items[0].optional_vars, ast.Name) and
                 # varname =
                 len(node.body) == 1 and
                 isinstance(node.body[0], ast.Assign) and
                 len(node.body[0].targets) == 1 and
                 isinstance(node.body[0].targets[0], ast.Name) and
@@ -135,31 +139,31 @@
 def _list_as_str(lst: Sequence[str]) -> str:
     if len(lst) == 1:
         return lst[0]
     else:
         return '\n' + '\n'.join(lst)
 
 
-def _dict_as_str(dct: Dict[str, str]) -> str:
+def _dict_as_str(dct: dict[str, str]) -> str:
     return _list_as_str([f'{k}={v}' for k, v in dct.items()])
 
 
-def _reformat(section: Dict[str, Any]) -> Dict[str, Any]:
+def _reformat(section: dict[str, Any]) -> dict[str, Any]:
     new_section = {}
     for key, value in section.items():
         if isinstance(value, (list, tuple)):
             new_section[key] = _list_as_str(value)
         elif isinstance(value, dict):
             new_section[key] = _dict_as_str(value)
         else:
             new_section[key] = value
     return new_section
 
 
-def main(argv: Optional[Sequence[str]] = None) -> int:
+def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('directory')
     args = parser.parse_args(argv)
 
     setup_py = os.path.join(args.directory, 'setup.py')
     with open(setup_py, 'rb') as setup_py_f:
         tree = ast.parse(setup_py_f.read(), filename=setup_py)
@@ -223,8 +227,8 @@
         f.write(contents)
 
     print(f'{setup_py} and {setup_cfg} written!')
     return 0
 
 
 if __name__ == '__main__':
-    exit(main())
+    raise SystemExit(main())
```

