# Comparing `tmp/glotter2-0.6.0.tar.gz` & `tmp/glotter2-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glotter2-0.6.0.tar", max compression
+gzip compressed data, was "glotter2-0.6.1.tar", max compression
```

## Comparing `glotter2-0.6.0.tar` & `glotter2-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1105 2023-02-25 14:19:23.663270 glotter2-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2746 2023-04-01 20:13:08.899865 glotter2-0.6.0/README.md
--rw-r--r--   0        0        0      191 2023-04-01 17:41:06.994287 glotter2-0.6.0/glotter/__init__.py
--rw-r--r--   0        0        0     3271 2023-03-02 01:12:21.951067 glotter2-0.6.0/glotter/__main__.py
--rw-r--r--   0        0        0    12978 2023-03-28 18:23:01.742869 glotter2-0.6.0/glotter/auto_gen_test.py
--rw-r--r--   0        0        0     3781 2023-03-02 02:24:54.569331 glotter2-0.6.0/glotter/containerfactory.py
--rw-r--r--   0        0        0      680 2023-02-26 16:00:40.206266 glotter2-0.6.0/glotter/decorators.py
--rw-r--r--   0        0        0      959 2023-03-02 00:31:52.361647 glotter2-0.6.0/glotter/download.py
--rw-r--r--   0        0        0     4753 2023-03-18 14:28:46.995459 glotter2-0.6.0/glotter/project.py
--rw-r--r--   0        0        0     3087 2023-02-26 19:19:43.729458 glotter2-0.6.0/glotter/report.py
--rw-r--r--   0        0        0      728 2023-03-01 00:45:45.072395 glotter2-0.6.0/glotter/run.py
--rw-r--r--   0        0        0     7758 2023-03-18 19:56:57.285778 glotter2-0.6.0/glotter/settings.py
--rw-r--r--   0        0        0      327 2023-03-14 17:43:43.187564 glotter2-0.6.0/glotter/singleton.py
--rw-r--r--   0        0        0     6263 2023-03-17 22:38:08.039572 glotter2-0.6.0/glotter/source.py
--rw-r--r--   0        0        0     1933 2023-03-17 22:36:01.438407 glotter2-0.6.0/glotter/test.py
--rw-r--r--   0        0        0     5027 2023-04-01 18:00:31.534775 glotter2-0.6.0/glotter/test_doc_generator.py
--rw-r--r--   0        0        0     2161 2023-03-17 22:20:40.522430 glotter2-0.6.0/glotter/test_generator.py
--rw-r--r--   0        0        0     5490 2023-02-25 19:40:59.629278 glotter2-0.6.0/glotter/testinfo.py
--rw-r--r--   0        0        0      853 2023-03-17 22:34:49.362111 glotter2-0.6.0/glotter/utils.py
--rw-r--r--   0        0        0     1590 2023-04-01 19:54:21.439022 glotter2-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 glotter2-0.6.0/setup.py
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 glotter2-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-25 14:19:23.663270 glotter2-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     2820 2023-05-06 11:22:09.635606 glotter2-0.6.1/README.md
+-rw-r--r--   0        0        0      191 2023-04-01 17:41:06.994287 glotter2-0.6.1/glotter/__init__.py
+-rw-r--r--   0        0        0     3271 2023-03-02 01:12:21.951067 glotter2-0.6.1/glotter/__main__.py
+-rw-r--r--   0        0        0    12978 2023-03-28 18:23:01.742869 glotter2-0.6.1/glotter/auto_gen_test.py
+-rw-r--r--   0        0        0     3781 2023-03-02 02:24:54.569331 glotter2-0.6.1/glotter/containerfactory.py
+-rw-r--r--   0        0        0      680 2023-02-26 16:00:40.206266 glotter2-0.6.1/glotter/decorators.py
+-rw-r--r--   0        0        0      959 2023-03-02 00:31:52.361647 glotter2-0.6.1/glotter/download.py
+-rw-r--r--   0        0        0     4753 2023-03-18 14:28:46.995459 glotter2-0.6.1/glotter/project.py
+-rw-r--r--   0        0        0     3087 2023-02-26 19:19:43.729458 glotter2-0.6.1/glotter/report.py
+-rw-r--r--   0        0        0      728 2023-03-01 00:45:45.072395 glotter2-0.6.1/glotter/run.py
+-rw-r--r--   0        0        0     7758 2023-03-18 19:56:57.285778 glotter2-0.6.1/glotter/settings.py
+-rw-r--r--   0        0        0      327 2023-03-14 17:43:43.187564 glotter2-0.6.1/glotter/singleton.py
+-rw-r--r--   0        0        0     6263 2023-03-17 22:38:08.039572 glotter2-0.6.1/glotter/source.py
+-rw-r--r--   0        0        0     1933 2023-03-17 22:36:01.438407 glotter2-0.6.1/glotter/test.py
+-rw-r--r--   0        0        0     5027 2023-04-01 18:00:31.534775 glotter2-0.6.1/glotter/test_doc_generator.py
+-rw-r--r--   0        0        0     2161 2023-03-17 22:20:40.522430 glotter2-0.6.1/glotter/test_generator.py
+-rw-r--r--   0        0        0     5490 2023-02-25 19:40:59.629278 glotter2-0.6.1/glotter/testinfo.py
+-rw-r--r--   0        0        0      853 2023-03-17 22:34:49.362111 glotter2-0.6.1/glotter/utils.py
+-rw-r--r--   0        0        0     1590 2023-05-06 11:24:16.524057 glotter2-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 glotter2-0.6.1/PKG-INFO
```

### Comparing `glotter2-0.6.0/LICENSE.txt` & `glotter2-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/README.md` & `glotter2-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
 
 ## Changelog
 
 ### Glotter2 releases
 
+* 0.6.1:
+  * Update `docker` dependency to 6.1.0 to support `urllib3` 2.x
 * 0.6.0:
   * Add test documentation generation
 * 0.5.0:
   * Add test generation
   * Add `pydantic` dependency
 * 0.4.5:
   * Add link to documentation
```

### Comparing `glotter2-0.6.0/glotter/__main__.py` & `glotter2-0.6.1/glotter/__main__.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/auto_gen_test.py` & `glotter2-0.6.1/glotter/auto_gen_test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/containerfactory.py` & `glotter2-0.6.1/glotter/containerfactory.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/decorators.py` & `glotter2-0.6.1/glotter/decorators.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/download.py` & `glotter2-0.6.1/glotter/download.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/project.py` & `glotter2-0.6.1/glotter/project.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/report.py` & `glotter2-0.6.1/glotter/report.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/run.py` & `glotter2-0.6.1/glotter/run.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/settings.py` & `glotter2-0.6.1/glotter/settings.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/source.py` & `glotter2-0.6.1/glotter/source.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/test.py` & `glotter2-0.6.1/glotter/test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/test_doc_generator.py` & `glotter2-0.6.1/glotter/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/test_generator.py` & `glotter2-0.6.1/glotter/test_generator.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/testinfo.py` & `glotter2-0.6.1/glotter/testinfo.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/glotter/utils.py` & `glotter2-0.6.1/glotter/utils.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.6.0/pyproject.toml` & `glotter2-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "glotter2"
 packages = [{include="glotter"}]
-version = "0.6.0"
+version = "0.6.1"
 description = "An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter"
 authors = ["auroq", "rzuckerm"]
 readme = "README.md"
 license = "LICENSE.txt"
 homepage = "https://github.com/rzuckerm/glotter2"
 documentation = "https://rzuckerm.github.io/glotter2"
 classifiers = [
@@ -16,15 +16,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rzuckerm/glotter2/issues"
 "Changelog" = "https://github.com/rzuckerm/glotter2#changelog"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-docker = "^6.0.1"
+docker = "^6.1.0"
 jinja2 = "^3.1.2"
 pytest = "^7.2.1"
 pyyaml = "^6.0"
 pytest-xdist = "^3.2.0"
 black = "^23.1.0"
 pydantic = "^1.10.6"
```

### Comparing `glotter2-0.6.0/setup.py` & `glotter2-0.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: glotter2
+Version: 0.6.1
+Summary: An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter
+Home-page: https://github.com/rzuckerm/glotter2
+License: LICENSE.txt
+Author: auroq
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: black (>=23.1.0,<24.0.0)
+Requires-Dist: docker (>=6.1.0,<7.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: pytest (>=7.2.1,<8.0.0)
+Requires-Dist: pytest-xdist (>=3.2.0,<4.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Bug Tracker, https://github.com/rzuckerm/glotter2/issues
+Project-URL: Changelog, https://github.com/rzuckerm/glotter2#changelog
+Project-URL: Documentation, https://rzuckerm.github.io/glotter2
+Description-Content-Type: text/markdown
+
+# Glotter2
+
+[![Makefile CI](https://github.com/rzuckerm/glotter2/actions/workflows/makefile.yml/badge.svg)](https://github.com/rzuckerm/glotter2/actions/workflows/makefile.yml)
+[![Coverage](https://rzuckerm.github.io/glotter2/badge.svg)](https://rzuckerm.github.io/glotter2/html_cov)
+[![PyPI version](https://img.shields.io/pypi/v/glotter2)](https://pypi.org/project/glotter2)
+[![Python versions](https://img.shields.io/pypi/pyversions/glotter2)](https://pypi.org/project/glotter2)
+[![Python wheel](https://img.shields.io/pypi/wheel/glotter2)](https://pypi.org/project/glotter2)
+
+[![Glotter2 logo](https://rzuckerm.github.io/glotter2/_static/glotter2_small.png)](https://rzuckerm.github.io/glotter2/)
+
+*The programming language icons were downloaded from [pngegg.com](https://www.pngegg.com/)*
+
+This is a fork of the original [Glotter](https://github.com/auroq/glotter) repository, which
+appears to be unmaintained.
+
+Glotter2 is an execution library for collections of single file scripts. It uses Docker to be able to build, run, and optionally test scripts in any language without having to install a local sdk or development environment.
+
+For getting started with Glotter2, refer to our [documentation](https://rzuckerm.github.io/glotter2/).
+
+## Contributing
+
+If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
+
+## Changelog
+
+### Glotter2 releases
+
+* 0.6.1:
+  * Update `docker` dependency to 6.1.0 to support `urllib3` 2.x
+* 0.6.0:
+  * Add test documentation generation
+* 0.5.0:
+  * Add test generation
+  * Add `pydantic` dependency
+* 0.4.5:
+  * Add link to documentation
+* 0.4.4:
+  * Fix bug that would indicate "No tests were found" when filtering tests
+* 0.4.2:
+  * Remove call to `time.sleep` when pulling image
+* 0.4.1:
+  * Bump version since wrong version pushed to pypi
+* 0.4.0:
+  * Change test ID from `<filename>` to `<language>/<filename>`
+  * Speed up test collection by about 1 min and total test time by about
+    5 min in [sample-programs][sample-programs] by caching list of sources
+  * Modify `download`, `run`, and `test` commands so that `-p`, `-l`, and
+    `-s` are no longer mutually exclusive
+  * Add `--parallel` to `download` command to parallelize image downloads
+  * Add `--parallel` to `test` command to parallelize tests
+* 0.3.0:
+  * Fix crash when running tests for [sample-programs][sample-programs]
+    with glotter 0.2.x
+  * Upgrade dependencies to latest version:
+    * `docker >=6.0.1, <7`
+    * `Jinja >=3.1.2, <4`
+    * `pytest >=7.2.1, <8`
+    * `PyYAML >=6.0, <7`
+  * Upgrade python to 3.8 or above
 
-packages = \
-['glotter']
+### Original Glotter releases
 
-package_data = \
-{'': ['*']}
+* 0.2.x: Add reporting verb to output discovered sources as a table in stdout or to a csv
+* 0.1.x: Initial release of working code.
 
-install_requires = \
-['black>=23.1.0,<24.0.0',
- 'docker>=6.0.1,<7.0.0',
- 'jinja2>=3.1.2,<4.0.0',
- 'pydantic>=1.10.6,<2.0.0',
- 'pytest-xdist>=3.2.0,<4.0.0',
- 'pytest>=7.2.1,<8.0.0',
- 'pyyaml>=6.0,<7.0']
-
-entry_points = \
-{'console_scripts': ['glotter = glotter.__main__:main']}
-
-setup_kwargs = {
-    'name': 'glotter2',
-    'version': '0.6.0',
-    'description': 'An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter',
-    'long_description': '# Glotter2\n\n[![Makefile CI](https://github.com/rzuckerm/glotter2/actions/workflows/makefile.yml/badge.svg)](https://github.com/rzuckerm/glotter2/actions/workflows/makefile.yml)\n[![Coverage](https://rzuckerm.github.io/glotter2/badge.svg)](https://rzuckerm.github.io/glotter2/html_cov)\n[![PyPI version](https://img.shields.io/pypi/v/glotter2)](https://pypi.org/project/glotter2)\n[![Python versions](https://img.shields.io/pypi/pyversions/glotter2)](https://pypi.org/project/glotter2)\n[![Python wheel](https://img.shields.io/pypi/wheel/glotter2)](https://pypi.org/project/glotter2)\n\n[![Glotter2 logo](https://rzuckerm.github.io/glotter2/_static/glotter2_small.png)](https://rzuckerm.github.io/glotter2/)\n\n*The programming language icons were downloaded from [pngegg.com](https://www.pngegg.com/)*\n\nThis is a fork of the original [Glotter](https://github.com/auroq/glotter) repository, which\nappears to be unmaintained.\n\nGlotter2 is an execution library for collections of single file scripts. It uses Docker to be able to build, run, and optionally test scripts in any language without having to install a local sdk or development environment.\n\nFor getting started with Glotter2, refer to our [documentation](https://rzuckerm.github.io/glotter2/).\n\n## Contributing\n\nIf you\'d like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).\n\n## Changelog\n\n### Glotter2 releases\n\n* 0.6.0:\n  * Add test documentation generation\n* 0.5.0:\n  * Add test generation\n  * Add `pydantic` dependency\n* 0.4.5:\n  * Add link to documentation\n* 0.4.4:\n  * Fix bug that would indicate "No tests were found" when filtering tests\n* 0.4.2:\n  * Remove call to `time.sleep` when pulling image\n* 0.4.1:\n  * Bump version since wrong version pushed to pypi\n* 0.4.0:\n  * Change test ID from `<filename>` to `<language>/<filename>`\n  * Speed up test collection by about 1 min and total test time by about\n    5 min in [sample-programs][sample-programs] by caching list of sources\n  * Modify `download`, `run`, and `test` commands so that `-p`, `-l`, and\n    `-s` are no longer mutually exclusive\n  * Add `--parallel` to `download` command to parallelize image downloads\n  * Add `--parallel` to `test` command to parallelize tests\n* 0.3.0:\n  * Fix crash when running tests for [sample-programs][sample-programs]\n    with glotter 0.2.x\n  * Upgrade dependencies to latest version:\n    * `docker >=6.0.1, <7`\n    * `Jinja >=3.1.2, <4`\n    * `pytest >=7.2.1, <8`\n    * `PyYAML >=6.0, <7`\n  * Upgrade python to 3.8 or above\n\n### Original Glotter releases\n\n* 0.2.x: Add reporting verb to output discovered sources as a table in stdout or to a csv\n* 0.1.x: Initial release of working code.\n\n[sample-programs]: https://github.com/TheRenegadeCoder/sample-programs\n',
-    'author': 'auroq',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/rzuckerm/glotter2',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+[sample-programs]: https://github.com/TheRenegadeCoder/sample-programs
 
-
-setup(**setup_kwargs)
```

