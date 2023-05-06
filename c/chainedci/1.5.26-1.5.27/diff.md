# Comparing `tmp/chainedci-1.5.26.tar.gz` & `tmp/chainedci-1.5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainedci-1.5.26.tar", last modified: Thu May  4 11:06:59 2023, max compression
+gzip compressed data, was "chainedci-1.5.27.tar", last modified: Sat May  6 15:15:44 2023, max compression
```

## Comparing `chainedci-1.5.26.tar` & `chainedci-1.5.27.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.662661 chainedci-1.5.26/
--rw-rw-rw-   0 root         (0)    59417      331 2023-05-04 11:06:32.000000 chainedci-1.5.26/MANIFEST.in
--rw-r--r--   0 root         (0)    59417      923 2023-05-04 11:06:59.662661 chainedci-1.5.26/PKG-INFO
--rw-rw-rw-   0 root         (0)    59417      677 2023-05-04 11:06:32.000000 chainedci-1.5.26/README.md
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.658661 chainedci-1.5.26/chainedci/
--rw-rw-rw-   0 root         (0)    59417      285 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/__init__.py
--rw-rw-rw-   0 root         (0)    59417    11472 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/artifact.py
--rw-rw-rw-   0 root         (0)    59417     9356 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/artifact_src.py
--rwxrwxrwx   0 root         (0)    59417      131 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/chainedci
--rw-rw-rw-   0 root         (0)    59417     6338 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/cli.py
--rw-rw-rw-   0 root         (0)    59417     6819 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/config.py
--rw-rw-rw-   0 root         (0)    59417     3663 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/default_chainedci.yml
--rw-rw-rw-   0 root         (0)    59417     3926 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/env_vars.py
--rw-rw-rw-   0 root         (0)    59417     2924 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/http_adapter.py
--rw-rw-rw-   0 root         (0)    59417     3932 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/init_project.py
--rw-rw-rw-   0 root         (0)    59417     4174 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/inventory.py
--rw-rw-rw-   0 root         (0)    59417     4850 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/log.py
--rw-rw-rw-   0 root         (0)    59417     5935 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/options.py
--rw-rw-rw-   0 root         (0)    59417     3888 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/parser.py
--rw-rw-rw-   0 root         (0)    59417    10532 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/pipeline.py
--rw-rw-rw-   0 root         (0)    59417     4890 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/scenario.py
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.662661 chainedci-1.5.26/chainedci/static/
--rw-rw-rw-   0 root         (0)    59417        8 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/static/inventory
--rw-rw-rw-   0 root         (0)    59417      390 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/static/projectA.yml
--rw-rw-rw-   0 root         (0)    59417       30 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/static/projectA_config1.yml
--rw-rw-rw-   0 root         (0)    59417       30 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/static/projectA_config2.yml
--rw-rw-rw-   0 root         (0)    59417    15020 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/step.py
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.662661 chainedci-1.5.26/chainedci/templates/
--rw-rw-rw-   0 root         (0)    59417     1165 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/templates/all.yml.tpl
--rw-rw-rw-   0 root         (0)    59417     3974 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/templates/main.yml.tpl
--rw-rw-rw-   0 root         (0)    59417     2532 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/templates/scenario.yml.tpl
--rw-rw-rw-   0 root         (0)    59417     2782 2023-05-04 11:06:32.000000 chainedci-1.5.26/chainedci/tools.py
--rw-rw-rw-   0 root         (0)    59417      664 2023-05-04 11:06:43.000000 chainedci-1.5.26/chainedci/version.py
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.662661 chainedci-1.5.26/chainedci.egg-info/
--rw-r--r--   0 root         (0)    59417      923 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)    59417      924 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)    59417        1 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)    59417        1 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)    59417      101 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/requires.txt
--rw-r--r--   0 root         (0)    59417       22 2023-05-04 11:06:59.000000 chainedci-1.5.26/chainedci.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0)    59417      240 2023-05-04 11:06:59.666662 chainedci-1.5.26/setup.cfg
--rw-rw-rw-   0 root         (0)    59417     1243 2023-05-04 11:06:43.000000 chainedci-1.5.26/setup.py
-drwxr-sr-x   0 root         (0)    59417        0 2023-05-04 11:06:59.662661 chainedci-1.5.26/tests/
--rw-rw-rw-   0 root         (0)    59417        0 2023-05-04 11:06:32.000000 chainedci-1.5.26/tests/__init__.py
--rw-rw-rw-   0 root         (0)    59417     1318 2023-05-04 11:06:32.000000 chainedci-1.5.26/tests/tests_lib.py
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.576779 chainedci-1.5.27/
+-rw-rw-rw-   0 root         (0)    59417      331 2023-05-06 15:15:17.000000 chainedci-1.5.27/MANIFEST.in
+-rw-r--r--   0 root         (0)    59417      923 2023-05-06 15:15:44.576779 chainedci-1.5.27/PKG-INFO
+-rw-rw-rw-   0 root         (0)    59417      677 2023-05-06 15:15:17.000000 chainedci-1.5.27/README.md
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.572779 chainedci-1.5.27/chainedci/
+-rw-rw-rw-   0 root         (0)    59417      285 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/__init__.py
+-rw-rw-rw-   0 root         (0)    59417    11472 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/artifact.py
+-rw-rw-rw-   0 root         (0)    59417     9356 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/artifact_src.py
+-rwxrwxrwx   0 root         (0)    59417      131 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/chainedci
+-rw-rw-rw-   0 root         (0)    59417     6338 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/cli.py
+-rw-rw-rw-   0 root         (0)    59417     6819 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/config.py
+-rw-rw-rw-   0 root         (0)    59417     3663 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/default_chainedci.yml
+-rw-rw-rw-   0 root         (0)    59417     3926 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/env_vars.py
+-rw-rw-rw-   0 root         (0)    59417     2924 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/http_adapter.py
+-rw-rw-rw-   0 root         (0)    59417     3932 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/init_project.py
+-rw-rw-rw-   0 root         (0)    59417     4174 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/inventory.py
+-rw-rw-rw-   0 root         (0)    59417     4850 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/log.py
+-rw-rw-rw-   0 root         (0)    59417     5935 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/options.py
+-rw-rw-rw-   0 root         (0)    59417     3888 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/parser.py
+-rw-rw-rw-   0 root         (0)    59417    10532 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/pipeline.py
+-rw-rw-rw-   0 root         (0)    59417     4890 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/scenario.py
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.572779 chainedci-1.5.27/chainedci/static/
+-rw-rw-rw-   0 root         (0)    59417        8 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/static/inventory
+-rw-rw-rw-   0 root         (0)    59417      390 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/static/projectA.yml
+-rw-rw-rw-   0 root         (0)    59417       30 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/static/projectA_config1.yml
+-rw-rw-rw-   0 root         (0)    59417       30 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/static/projectA_config2.yml
+-rw-rw-rw-   0 root         (0)    59417    15020 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/step.py
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.576779 chainedci-1.5.27/chainedci/templates/
+-rw-rw-rw-   0 root         (0)    59417     1165 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/templates/all.yml.tpl
+-rw-rw-rw-   0 root         (0)    59417     3974 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/templates/main.yml.tpl
+-rw-rw-rw-   0 root         (0)    59417     2532 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/templates/scenario.yml.tpl
+-rw-rw-rw-   0 root         (0)    59417     2782 2023-05-06 15:15:17.000000 chainedci-1.5.27/chainedci/tools.py
+-rw-rw-rw-   0 root         (0)    59417      664 2023-05-06 15:15:29.000000 chainedci-1.5.27/chainedci/version.py
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.572779 chainedci-1.5.27/chainedci.egg-info/
+-rw-r--r--   0 root         (0)    59417      923 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)    59417      924 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)    59417        1 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)    59417        1 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)    59417       99 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/requires.txt
+-rw-r--r--   0 root         (0)    59417       22 2023-05-06 15:15:44.000000 chainedci-1.5.27/chainedci.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0)    59417      240 2023-05-06 15:15:44.576779 chainedci-1.5.27/setup.cfg
+-rw-rw-rw-   0 root         (0)    59417     1241 2023-05-06 15:15:29.000000 chainedci-1.5.27/setup.py
+drwxr-sr-x   0 root         (0)    59417        0 2023-05-06 15:15:44.576779 chainedci-1.5.27/tests/
+-rw-rw-rw-   0 root         (0)    59417        0 2023-05-06 15:15:17.000000 chainedci-1.5.27/tests/__init__.py
+-rw-rw-rw-   0 root         (0)    59417     1318 2023-05-06 15:15:17.000000 chainedci-1.5.27/tests/tests_lib.py
```

### Comparing `chainedci-1.5.26/PKG-INFO` & `chainedci-1.5.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.26
+Version: 1.5.27
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.26/README.md` & `chainedci-1.5.27/README.md`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/artifact.py` & `chainedci-1.5.27/chainedci/artifact.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/artifact_src.py` & `chainedci-1.5.27/chainedci/artifact_src.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/cli.py` & `chainedci-1.5.27/chainedci/cli.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/config.py` & `chainedci-1.5.27/chainedci/config.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/default_chainedci.yml` & `chainedci-1.5.27/chainedci/default_chainedci.yml`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/env_vars.py` & `chainedci-1.5.27/chainedci/env_vars.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/http_adapter.py` & `chainedci-1.5.27/chainedci/http_adapter.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/init_project.py` & `chainedci-1.5.27/chainedci/init_project.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/inventory.py` & `chainedci-1.5.27/chainedci/inventory.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/log.py` & `chainedci-1.5.27/chainedci/log.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/options.py` & `chainedci-1.5.27/chainedci/options.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/parser.py` & `chainedci-1.5.27/chainedci/parser.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/pipeline.py` & `chainedci-1.5.27/chainedci/pipeline.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/scenario.py` & `chainedci-1.5.27/chainedci/scenario.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/step.py` & `chainedci-1.5.27/chainedci/step.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/templates/all.yml.tpl` & `chainedci-1.5.27/chainedci/templates/all.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/templates/main.yml.tpl` & `chainedci-1.5.27/chainedci/templates/main.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/templates/scenario.yml.tpl` & `chainedci-1.5.27/chainedci/templates/scenario.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/tools.py` & `chainedci-1.5.27/chainedci/tools.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/chainedci/version.py` & `chainedci-1.5.27/chainedci/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 """Version module."""
 
-__version__ = "1.5.26"
+__version__ = "1.5.27"
```

### Comparing `chainedci-1.5.26/chainedci.egg-info/PKG-INFO` & `chainedci-1.5.27/chainedci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.26
+Version: 1.5.27
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.26/chainedci.egg-info/SOURCES.txt` & `chainedci-1.5.27/chainedci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.26/setup.py` & `chainedci-1.5.27/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 def readme():
     """Set Readme from file."""
     with open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 setup(name='chainedci',
-      version='1.5.26',
+      version='1.5.27',
       description='Chaine Gitlab CI pipelines',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci',
       author='Orange OpenSource',
       license='Apache 2.0',
       packages=find_packages(),
       py_modules=[splitext(basename(path))[0] for path in glob('*.py')],
       include_package_data=True,
       scripts=["chainedci/chainedci"],
       install_requires=[
-          "ansible-core==2.14.4",
+          "ansible-core==2.14.5",
           "GitPython==3.1.31",
           "Jinja2==3.1.2",
-          "requests==2.28.2",
+          "requests==2.30.0",
           "schema==0.7.5",
-          "urllib3 ==1.26.15"
+          "urllib3 ==2.0.2"
       ],
       setup_requires=["pytest-runner"],
       tests_require=[
           "pytest",
           "pytest-cov",
           "pytest-mock",
           "mock",
```

### Comparing `chainedci-1.5.26/tests/tests_lib.py` & `chainedci-1.5.27/tests/tests_lib.py`

 * *Files identical despite different names*

