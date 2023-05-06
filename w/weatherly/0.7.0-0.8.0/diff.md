# Comparing `tmp/weatherly-0.7.0.tar.gz` & `tmp/weatherly-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherly-0.7.0.tar", last modified: Thu May  4 21:39:23 2023, max compression
+gzip compressed data, was "weatherly-0.8.0.tar", last modified: Sat May  6 11:20:26 2023, max compression
```

## Comparing `weatherly-0.7.0.tar` & `weatherly-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-04 21:39:23.371873 weatherly-0.7.0/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1076 2023-04-14 20:22:17.000000 weatherly-0.7.0/LICENSE
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     3501 2023-05-04 21:39:23.371873 weatherly-0.7.0/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2434 2023-05-03 20:11:13.000000 weatherly-0.7.0/README.rst
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       38 2023-05-04 21:39:23.371873 weatherly-0.7.0/setup.cfg
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1956 2023-05-01 21:27:37.000000 weatherly-0.7.0/setup.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-04 21:39:23.363873 weatherly-0.7.0/weatherly/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      783 2023-05-04 21:29:45.000000 weatherly-0.7.0/weatherly/__init__.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-04 21:39:23.371873 weatherly-0.7.0/weatherly/api/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     1227 2023-04-30 21:49:39.000000 weatherly-0.7.0/weatherly/api/__init__.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    24705 2023-05-04 21:32:28.000000 weatherly-0.7.0/weatherly/api/client.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2657 2023-04-23 19:24:58.000000 weatherly-0.7.0/weatherly/api/core.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     4916 2023-05-04 21:27:52.000000 weatherly-0.7.0/weatherly/enums.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     3905 2023-04-30 21:01:53.000000 weatherly-0.7.0/weatherly/errors.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)    31002 2023-05-04 21:06:48.000000 weatherly-0.7.0/weatherly/responses.py
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     2798 2023-04-27 19:47:53.000000 weatherly-0.7.0/weatherly/utils.py
-drwxrwxr-x   0 konrad    (1000) konrad    (1000)        0 2023-05-04 21:39:23.367873 weatherly-0.7.0/weatherly.egg-info/
--rw-rw-r--   0 konrad    (1000) konrad    (1000)     3501 2023-05-04 21:39:23.000000 weatherly-0.7.0/weatherly.egg-info/PKG-INFO
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      366 2023-05-04 21:39:23.000000 weatherly-0.7.0/weatherly.egg-info/SOURCES.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)        1 2023-05-04 21:39:23.000000 weatherly-0.7.0/weatherly.egg-info/dependency_links.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)      116 2023-05-04 21:39:23.000000 weatherly-0.7.0/weatherly.egg-info/requires.txt
--rw-rw-r--   0 konrad    (1000) konrad    (1000)       10 2023-05-04 21:39:23.000000 weatherly-0.7.0/weatherly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.522344 weatherly-0.8.0/
+-rw-rw-rw-   0        0        0     1097 2023-04-15 14:32:24.000000 weatherly-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3574 2023-05-06 11:20:26.519347 weatherly-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2500 2023-05-06 11:06:37.000000 weatherly-0.8.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:20:26.522344 weatherly-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2024 2023-05-02 14:16:37.000000 weatherly-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.468378 weatherly-0.8.0/weatherly/
+-rw-rw-rw-   0        0        0      817 2023-05-06 11:15:22.000000 weatherly-0.8.0/weatherly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.514397 weatherly-0.8.0/weatherly/api/
+-rw-rw-rw-   0        0        0     1257 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/api/__init__.py
+-rw-rw-rw-   0        0        0    26795 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/api/client.py
+-rw-rw-rw-   0        0        0     2742 2023-04-24 06:52:08.000000 weatherly-0.8.0/weatherly/api/core.py
+-rw-rw-rw-   0        0        0     5346 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/enums.py
+-rw-rw-rw-   0        0        0     4035 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/errors.py
+-rw-rw-rw-   0        0        0    43189 2023-05-06 11:06:37.000000 weatherly-0.8.0/weatherly/responses.py
+-rw-rw-rw-   0        0        0     2894 2023-05-02 14:16:37.000000 weatherly-0.8.0/weatherly/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:20:26.500357 weatherly-0.8.0/weatherly.egg-info/
+-rw-rw-rw-   0        0        0     3574 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 11:20:26.000000 weatherly-0.8.0/weatherly.egg-info/top_level.txt
```

### Comparing `weatherly-0.7.0/LICENSE` & `weatherly-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `weatherly-0.7.0/PKG-INFO` & `weatherly-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,92 @@
-Metadata-Version: 2.1
-Name: weatherly
-Version: 0.7.0
-Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
-Home-page: https://github.com/konradsic/weatherly
-Author: konradsic
-License: MIT
-Project-URL: Issues, https://github.com/konradsic/weatherly/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-⛅ weatherly
-====================
-.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
-    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
-    :alt: Weatherly license
-.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Weatherly version on PyPI
-.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Supported Python versions
-.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Project status
-.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
-    :target: https://github.com/konradsic/weatherly
-    :alt: Build status
-
-Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
-
-Features
----------------
-* Easy to use,
-* Intuitive design,
-* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
-* Modern and typed Python package,
-* Support for languages (provided by WeatherAPI)
-
-Installing
-------------
-To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
-
-.. code:: shell
-    
-    # Windows
-    py -3 -m pip install -U weatherly
-
-    # MacOS / Linux
-    python3 -m pip install -U weatherly
-
-Congratulations! Now weatherly is ready to use on your machine.
-
-Code example
----------------------
-
-.. code:: python
-
-    import weatherly
-    
-    client = weatherly.Client(api_key="your WeatherAPI key")
-    # you can set language to all request, or pass it manually
-    client.set_language("fr")     # lang code
-    client.set_language("German") # language full name
-
-    # getting weather info
-    current_weather = client.get_current_weather(query="London")
-
-    # getting forecast info
-    forecast = client.get_forecast_data(query="Paris", days=3)
-
-    # historical data
-    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
-
-    # marine data
-    marine = client.get_marine_data(query="Madrid")
-
-
+Metadata-Version: 2.1
+Name: weatherly
+Version: 0.8.0
+Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
+Home-page: https://github.com/konradsic/weatherly
+Author: konradsic
+License: MIT
+Project-URL: Issues, https://github.com/konradsic/weatherly/issues
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+⛅ weatherly
+====================
+.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
+    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
+    :alt: Weatherly license
+.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Weatherly version on PyPI
+.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Supported Python versions
+.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Project status
+.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
+    :target: https://github.com/konradsic/weatherly
+    :alt: Build status
+
+Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
+
+Features
+---------------
+* Easy to use,
+* Intuitive design,
+* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
+* Modern and typed Python package,
+* Support for languages (provided by WeatherAPI)
+
+Installing
+------------
+To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
+
+.. code:: shell
+    
+    # Windows
+    py -3 -m pip install -U weatherly
+
+    # MacOS / Linux
+    python3 -m pip install -U weatherly
+
+Congratulations! Now weatherly is ready to use on your machine.
+
+Code example
+---------------------
+
+.. code:: python
+
+    import weatherly
+    
+    client = weatherly.Client(api_key="your WeatherAPI key")
+    # you can set language to all requests, or pass it manually
+    client.set_language("fr")     # lang code
+    client.set_language("German") # language full name
+
+    # getting weather info
+    current_weather = client.get_current_weather(query="London")
+
+    # getting forecast info
+    forecast = client.get_forecast_data(query="Paris", days=3)
+
+    # historical data
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
+
+    # marine data
+    marine = client.get_marine_data(query="Madrid")
```

### Comparing `weatherly-0.7.0/README.rst` & `weatherly-0.8.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-⛅ weatherly
-====================
-.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
-    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
-    :alt: Weatherly license
-.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Weatherly version on PyPI
-.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Supported Python versions
-.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Project status
-.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
-    :target: https://github.com/konradsic/weatherly
-    :alt: Build status
-
-Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
-
-Features
----------------
-* Easy to use,
-* Intuitive design,
-* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
-* Modern and typed Python package,
-* Support for languages (provided by WeatherAPI)
-
-Installing
-------------
-To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
-
-.. code:: shell
-    
-    # Windows
-    py -3 -m pip install -U weatherly
-
-    # MacOS / Linux
-    python3 -m pip install -U weatherly
-
-Congratulations! Now weatherly is ready to use on your machine.
-
-Code example
----------------------
-
-.. code:: python
-
-    import weatherly
-    
-    client = weatherly.Client(api_key="your WeatherAPI key")
-    # you can set language to all request, or pass it manually
-    client.set_language("fr")     # lang code
-    client.set_language("German") # language full name
-
-    # getting weather info
-    current_weather = client.get_current_weather(query="London")
-
-    # getting forecast info
-    forecast = client.get_forecast_data(query="Paris", days=3)
-
-    # historical data
-    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
-
-    # marine data
-    marine = client.get_marine_data(query="Madrid")
+⛅ weatherly
+====================
+.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
+    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
+    :alt: Weatherly license
+.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Weatherly version on PyPI
+.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Supported Python versions
+.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Project status
+.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
+    :target: https://github.com/konradsic/weatherly
+    :alt: Build status
+
+Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
+
+Features
+---------------
+* Easy to use,
+* Intuitive design,
+* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
+* Modern and typed Python package,
+* Support for languages (provided by WeatherAPI)
+
+Installing
+------------
+To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
+
+.. code:: shell
+    
+    # Windows
+    py -3 -m pip install -U weatherly
+
+    # MacOS / Linux
+    python3 -m pip install -U weatherly
+
+Congratulations! Now weatherly is ready to use on your machine.
+
+Code example
+---------------------
+
+.. code:: python
+
+    import weatherly
+    
+    client = weatherly.Client(api_key="your WeatherAPI key")
+    # you can set language to all requests, or pass it manually
+    client.set_language("fr")     # lang code
+    client.set_language("German") # language full name
+
+    # getting weather info
+    current_weather = client.get_current_weather(query="London")
+
+    # getting forecast info
+    forecast = client.get_forecast_data(query="Paris", days=3)
+
+    # historical data
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
+
+    # marine data
+    marine = client.get_marine_data(query="Madrid")
```

### Comparing `weatherly-0.7.0/setup.py` & `weatherly-0.8.0/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from setuptools import setup
-import re
-
-version = None
-with open('weatherly/__init__.py') as f:
-    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
-
-if not version:
-    raise RuntimeError('version is not set')
-
-readme = ''
-with open('README.rst', encoding='utf-8') as readme_file: 
-    readme = readme_file.read()
-
-
-requirements = []
-with open('requirements.txt') as requirements_file: 
-    requirements = requirements_file.read().splitlines()
-
-extras_require = {
-    'docs': [
-        'sphinx==5.3.0',
-        'sphinx_book_theme==1.0.1',
-        'sphinxcontrib_trio==1.1.2'
-    ],
-    'test': [
-        'pytest',
-        'pytest-cov'
-    ]
-}
-
-packages = [
-    'weatherly',
-    'weatherly.api',
-]
-
-setup(
-    name='weatherly',
-    author='konradsic',
-    url='https://github.com/konradsic/weatherly',
-    project_urls={
-        'Issues': 'https://github.com/konradsic/weatherly/issues',
-    },
-    version=version,
-    packages=packages,
-    license='MIT',
-    description='A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...',
-    long_description=readme,
-    long_description_content_type='text/x-rst',
-    include_package_data=True,
-    install_requires=requirements,
-    extras_require=extras_require,
-    python_requires='>=3.10.0',
-    classifiers=[
-        'Development Status :: 1 - Planning',
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Internet',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Topic :: Scientific/Engineering :: Atmospheric Science',
-        'Typing :: Typed',
-    ],
+from setuptools import setup
+import re
+
+version = None
+with open('weatherly/__init__.py') as f:
+    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
+
+if not version:
+    raise RuntimeError('version is not set')
+
+readme = ''
+with open('README.rst', encoding='utf-8') as readme_file: 
+    readme = readme_file.read()
+
+
+requirements = []
+with open('requirements.txt') as requirements_file: 
+    requirements = requirements_file.read().splitlines()
+
+extras_require = {
+    'docs': [
+        'sphinx==5.3.0',
+        'sphinx_book_theme==1.0.1',
+        'sphinxcontrib_trio==1.1.2'
+    ],
+    'test': [
+        'pytest',
+        'pytest-cov'
+    ]
+}
+
+packages = [
+    'weatherly',
+    'weatherly.api',
+]
+
+setup(
+    name='weatherly',
+    author='konradsic',
+    url='https://github.com/konradsic/weatherly',
+    project_urls={
+        'Issues': 'https://github.com/konradsic/weatherly/issues',
+    },
+    version=version,
+    packages=packages,
+    license='MIT',
+    description='A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...',
+    long_description=readme,
+    long_description_content_type='text/x-rst',
+    include_package_data=True,
+    install_requires=requirements,
+    extras_require=extras_require,
+    python_requires='>=3.10.0',
+    classifiers=[
+        'Development Status :: 1 - Planning',
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Internet',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Topic :: Scientific/Engineering :: Atmospheric Science',
+        'Typing :: Typed',
+    ],
 )
```

### Comparing `weatherly-0.7.0/weatherly/api/client.py` & `weatherly-0.8.0/weatherly/api/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,653 +1,686 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-import datetime
-from typing import Any, Dict, List, Literal, Optional, Union
-
-from .. import utils as utils
-from ..enums import Languages
-from ..errors import (AccessDenied, APIKeyDisabled, APILimitExceeded,
-                      InternalApplicationError, InvalidAPIKey, InvalidDate,
-                      NoLocationFound, WeatherAPIException)
-from ..responses import (AstronomicalData, CurrentWeatherData, ForecastData,
-                         FutureData, IPData, LocationData, SportsData)
-from .core import BaseAPIClient
-
-WEATHERAPI_BASE_URL = "https://api.weatherapi.com/v1/"
-BOOL_REPLACE = {True: "yes", False: "no"}
-
-__all__ = (
-    "Client",
-)
-
-class Client(BaseAPIClient):
-    """
-    A WeatherAPI.com client for fetching various weather information
-
-    Parameters
-    ----------
-    api_key: :class:`str`
-        API Key used to authenticate when sending requests
-    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]
-        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
-    dt: Optional[:class:`int`]
-        Restrict date output for Forecast and History API method. (Required for History and Future API)
-    end_dt: Optional[:class:`int`]
-        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)
-    hour: Optional[:class:`int`]
-        Restricting forecast or history output to a specific hour in a given day.
-    aqi: :class:`bool`
-        Enable/Disable Air Quality data in forecast API output. Defaults to "no".
-    tides: :class:`bool`
-        Enable/Disable Tide data in Marine API output. Defaults to "no".
-    kwargs: Dict[:class:`str`, Any]
-        Additional keyword arguments passed by default to requests made by the client
-        
-    Attributes
-    -------------
-    lang: Optional[:class:`Languages`]
-        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
-    dt: Optional[:class:`int`]
-        Restricted date output for Forecast and History API method. (Required for History and Future API)
-    end_dt: Optional[:class:`int`]
-        Restricted date output for History API method. Only works for API on Pro plan and above.
-    hour: Optional[:class:`int`]
-        Restricted forecast or history output to a specific hour in a given day.
-    aqi: :class:`bool`
-        Indicates if Air Quality data has been enabled
-    tides: :class:`bool`
-        Indicates if tides data in the Marine API has been enabled
-    kwargs: Dict[:class:`str`, Any]
-        Additional keyword arguments passed by default to requests made by the client
-    """
-    def __init__(
-        self,
-        api_key: str,
-        lang: Optional[Union[str, Languages]] = None,
-        dt: Optional[int] = None,
-        end_dt: Optional[int] = None,
-        hour: Optional[int] = None,
-        aqi: bool = False,
-        tides: bool = False,
-        **kwargs: Dict[str, Any]
-    ) -> None:
-        lang_code = None
-        if lang is not None: 
-            lang_code = utils.find_language(lang, asobj=True)
-        opts = {
-            "key": api_key,
-            **kwargs
-        }
-        if lang_code: opts.update(lang = lang_code.value if lang_code is not None else None)
-
-        super().__init__(base_url=WEATHERAPI_BASE_URL,
-                         default_options=opts)
-        
-        self.dt = dt
-        self.end_dt = end_dt
-        self.hour = hour
-        self.aqi = aqi
-        self.tides = tides
-        self.kwargs = kwargs
-        self.lang = Languages(lang_code) if lang_code else None
-    
-    
-    def _call_request(self, endpoint: str, options: Dict[str, Any]) -> Dict[str, Any]:
-        """Private method used to make requests to WeatherAPI"""
-        final_options = self.default_options.copy()
-
-        for k,v in final_options.items(): # check - remove NoneType values
-            if v is None: del final_options[k]
-        # add options to final_options
-        for k,v in options.items():
-            # also - replace bool with "yes"/"no"
-            if v is not None: final_options[k] = BOOL_REPLACE.get(v, v)
-
-        resp = self._request(endpoint, **final_options)
-
-        if not resp[1].status_code < 400:
-            # raise errors yay
-            error_data = resp[0]["error"]
-            code = error_data["code"]
-            status = resp[1].status_code
-            msg = error_data["message"]
-
-            if code == 1006: raise NoLocationFound(status, code, msg)
-            elif code == 2006: raise InvalidAPIKey(status, code, msg)
-            elif code == 2007: raise APILimitExceeded(status, code, msg)
-            elif code == 2008: raise APIKeyDisabled(status, code, msg)
-            elif code == 2009: raise AccessDenied(status, code, msg)
-            elif code == 9999: raise InternalApplicationError(status, code, msg)
-            else: raise WeatherAPIException(status, code, msg)
-
-        return resp
-    
-    def event(self):
-        """A decorator that turns a function into an event. For example
-
-        .. code:: python
-
-            import weatherly
-            client = weatherly.Client(api_key=...)
-
-            @client.event
-            def on_error(payload):
-                print(f"An error occured! Payload: {payload}")
-        
-        In the example above, by adding ``@client.event`` the ``on_error`` function has turned into an error handler function
-        """
-        raise NotImplementedError
-
-    def set_language(self, lang: Union[str, Languages]) -> Optional[Languages]:
-        """
-        Set client's language when requesting data.
-        
-        Parameters
-        -----------
-        lang: Union[:class:`str`, :class:`Languages`]
-            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
-            
-        Returns
-        ---------
-        Optional[:class:`Languages`]
-            An enum class representing the language of the client. Is ``None`` when something went wrong and the language was not set.
-        """
-        lang_class = utils.find_language(lang, asobj=True)
-        if not lang_class:
-            return None
-
-        self.lang = lang_class 
-        return self.lang
-
-    def get_current_weather(self, 
-        query: str, 
-        *,
-        lang: Optional[Union[str, Languages]] = None,
-        aqi: Optional[bool] = None,
-        **kwargs: Dict[str, Any]
-    ) -> CurrentWeatherData:
-        """
-        Get current weather data
-
-        Parameters
-        ----------
-        query: :class:`str`
-            Query string - location you want to get weather data for
-        lang: Optional[Union[:class:`str`, Languages]]
-            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-            To get a list of languages visit :class:`Languages`.
-        aqi: Optional[:class:`bool`]
-            Enable/Disable Air Quality data in forecast API output. If nothing is passed, then it defaults to client default value.
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments to request
-
-        Returns
-        -------
-        :class:`CurrentWeatherData`
-            Current weather data class
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "aqi": aqi or self.aqi,
-            "q": query,
-            **kwargs
-        }
-        if lang is not None: options["lang"] = lang
-        resp = self._call_request("current.json", options)
-
-        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
-        return weather
-
-    def get_locations(self, query: str):
-        """
-        Get locations for given query
-
-        Parameters
-        ---------------
-        query: :class:`str`
-            Query string, a location you are searching for
-
-        Returns
-        -----------
-        List[:class:`LocationData`]
-            A list of :class:`LocationData` classes.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        resp = self._call_request("search.json",{"q": query})
-
-        locations = []
-        for loc in resp[0]:
-            locations.append(LocationData(loc, resp[1].status_code, None))
-        return locations
-
-    def get_forecast_data(
-        self,
-        query: str, 
-        days: int,
-        *,
-        aqi: Optional[bool] = None,
-        alerts: Optional[bool] = None,
-        lang: Optional[Union[str, Languages]] = None,
-        **kwargs: Dict[str, Any]
-    ) -> ForecastData:
-        """
-        Get forecast data from Forecast API
-
-        Parameters
-        -------------
-        query: :class:`str`
-            Query string, location you want to get forecast data for
-        days: :class:`int`
-            Number of days of weather forecast. Value ranges from 1 to 10
-        aqi: Optional[:class:`bool`]
-            Enable/Disable Air Quality data. Defaults to ``None`` (will use client's default)
-        alerts: Optional[:class:`bool`]
-            Enable/Disable alerts data. Defaults to ``None`` (will use client's default)
-        lang: Optional[Union[:class`str`, :class`Languages`]]
-            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-            To get a list of languages visit :class:`Languages`.
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-            
-        Returns
-        ----------
-        :class:`ForecastData`
-            Fetched forecast data as a class.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "aqi": aqi or self.aqi,
-            "q": query,
-            "alerts": alerts or self.kwargs.get("alerts"),
-            "days": days,
-            **kwargs
-        }
-        if lang is not None: options["lang"] = lang
-
-        resp = self._call_request("forecast.json", options)
-        forecast = ForecastData(resp[0], resp[1].status_code, None)
-        return forecast
-
-    def get_historical_data(
-        self,
-        query: str,
-        date: str,
-        *,
-        aqi: Optional[bool] = None,
-        alerts: Optional[bool] = None,
-        lang: Optional[Union[str, Languages]] = None,
-        **kwargs: Dict[str, Any]
-    ) -> ForecastData:
-        """
-        Retrieve historical data for given day and query. Uses History API.
-
-        Parameters
-        -----------------
-        query: :class:`str`
-            Query string, location you want to get forecast data for
-        date: :class:`str`
-            A date string in format yyyy-mm-dd representing the day you want to get data for
-        aqi: Optional[:class:`bool`]
-            Enable/Disable Air Quality data. Defaults to ``None`` (will use client's default)
-        alerts: Optional[:class:`bool`]
-            Enable/Disable alerts data. Defaults to ``None`` (will use client's default)
-        lang: Optional[Union[:class`str`, :class`Languages`]]
-            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-            To get a list of languages visit :class:`Languages`.
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-        
-        Returns
-        ----------
-        :class:`ForecastData`
-            Forecast data for given day and query.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        :exc:`InvalidDate`
-            Raised when the ``date`` parameter is invalid (doesn't match the format or isn't a date before (or) today)
-        """
-        options = {
-            "aqi": aqi or self.aqi,
-            "q": query,
-            "alerts": alerts or self.kwargs.get("alerts"),
-            "dt": date,
-            **kwargs
-        }
-        if lang is not None: options["lang"] = lang
-
-        # check if given date is really "historical"
-        try:
-            splitted = date.split("-")
-            datetuple = datetime.datetime(
-                int(splitted[0]), 
-                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
-                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
-                0,0)
-            epoch = datetuple.timestamp()
-        except Exception as exc:
-            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
-
-        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
-
-        if epoch > now: raise InvalidDate("Date should be before current time, switch from History API to Future to use future dates.")
-
-        resp = self._call_request("history.json", options)
-        history = ForecastData(resp[0], resp[1].status_code, None)
-        return history
-        
-    def get_future_data(
-        self,
-        query: str,
-        date: str,
-        *,
-        lang: Optional[Union[str, Languages]] = None,
-        **kwargs: Dict[str, Any]
-    ) -> FutureData:
-        """
-        Retrieve future data for given day and query. Uses Future API.
-
-        Parameters
-        -----------------
-        query: :class:`str`
-            Query string, location you want to get forecast data for
-        date: :class:`str`
-            A date string in format yyyy-mm-dd representing the day you want to get data for
-        lang: Optional[Union[:class`str`, :class`Languages`]]
-            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-            To get a list of languages visit :class:`Languages`.
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-        
-        Returns
-        ----------
-        :class:`FutureData`
-            Future data for given day and query.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        :exc:`InvalidDate`
-            Raised when the ``date`` parameter is invalid (doesn't match the format or isn't a date after today)
-        """
-        options = {
-            "q": query,
-            "dt": date,
-            **kwargs
-        }
-        if lang is not None: options["lang"] = lang
-
-        # check if given date is really "historical"
-        try:
-            splitted = date.split("-")
-            datetuple = datetime.datetime(
-                int(splitted[0]), 
-                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
-                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
-                0,0)
-            epoch = datetuple.timestamp()
-        except Exception as exc:
-            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
-
-        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
-
-        if epoch < now: raise InvalidDate("Date should be after current time, switch from Future API to History to use past dates.")
-
-        resp = self._call_request("future.json", options)
-        future = FutureData(resp[0], resp[1].status_code, None)
-        return future
-        
-    def get_astronomical_data(
-        self,
-        query: str,
-        date: str,
-        **kwargs: Dict[str, Any]
-    ) -> AstronomicalData:
-        """
-        Get astronomical data from Astronomy API
-
-        Parameters
-        -------------
-        query: :class:`str`
-            Query string, location you want to get forecast data for
-        date: :class:`str`
-            Date in format yyyy-MM-dd and on or after 1st Jan, 2010 (2010-01-01)
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-            
-        Returns
-        ----------
-        :class:`AstronomicalData`
-            Fetched astronomical data as a class.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "q": query,
-            "dt": date,
-            **kwargs
-        }
-        resp = self._call_request("astronomy.json", options)
-        astro = AstronomicalData(resp[0], resp[1].status_code, None)
-        return astro
-
-    def get_marine_data(
-        self,
-        query: str,
-        *,
-        tides: Optional[bool],
-        **kwargs: Dict[str, Any]
-    ):
-        raise NotImplementedError
-
-    def get_ip_data(
-        self,
-        ip_address: str,
-        **kwargs: Dict[str, Any]
-    ) -> IPData:
-        """
-        Look for data for the given IP address.
-
-        Parameters
-        -------------
-        ip_address: :class:`str`
-            IP address you want to get data for. Can be ipv4 or ipv6
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-            
-        Returns
-        ----------
-        :class:`IPData`
-            Fetched IP data as a class.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when either IP address was invalid or no matching location was found.
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "q": ip_address,
-            **kwargs
-        }
-        resp = self._call_request("ip.json", options)
-        ip = IPData(resp[0], resp[1].status_code, None)
-        return ip
-
-    def get_sports_data(
-        self,
-        query: str,
-        **kwargs: Dict[str, Any]
-    ) -> SportsData:
-        """
-        Get sports data for a given query. Uses Sports API.
-
-        Parameters
-        -------------
-        query: :class:`str`
-            Query string, location you want to get sports data for
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments that will be passed to the request.
-            
-        Returns
-        ----------
-        :class:`SportsData`
-            Retrieved sports data as a class.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when either IP address was invalid or no matching location was found.
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "q": query,
-            **kwargs
-        }
-        resp = self._call_request("sports.json", options)
-        sports = SportsData(resp[0], resp[1].status_code, None)
-        return sports
-
-
-    
-    def __str__(self):
-        return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
-    
-    def __repr__(self):
-        return repr(self.__str__())
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+import datetime
+from typing import Any, Dict, List, Literal, Optional, Union
+
+from .. import utils as utils
+from ..enums import Languages
+from ..errors import (AccessDenied, APIKeyDisabled, APILimitExceeded,
+                      InternalApplicationError, InvalidAPIKey, InvalidDate,
+                      NoLocationFound, WeatherAPIException)
+from ..responses import (AstronomicalData, CurrentWeatherData, ForecastData,
+                         FutureData, IPData, LocationData, SportsData, MarineData)
+from .core import BaseAPIClient
+
+WEATHERAPI_BASE_URL = "https://api.weatherapi.com/v1/"
+BOOL_REPLACE = {True: "yes", False: "no"}
+
+__all__ = (
+    "Client",
+)
+
+class Client(BaseAPIClient):
+    """
+    A WeatherAPI.com client for fetching various weather information
+
+    Parameters
+    ----------
+    api_key: :class:`str`
+        API Key used to authenticate when sending requests
+    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]
+        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
+    dt: Optional[:class:`int`]
+        Restrict date output for Forecast and History API method. (Required for History and Future API)
+    end_dt: Optional[:class:`int`]
+        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)
+    hour: Optional[:class:`int`]
+        Restricting forecast or history output to a specific hour in a given day.
+    aqi: :class:`bool`
+        Enable/Disable Air Quality data in forecast API output. Defaults to "no".
+    tides: :class:`bool`
+        Enable/Disable Tide data in Marine API output. Defaults to "no".
+    kwargs: Dict[:class:`str`, Any]
+        Additional keyword arguments passed by default to requests made by the client
+        
+    Attributes
+    -------------
+    lang: Optional[:class:`Languages`]
+        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
+    dt: Optional[:class:`int`]
+        Restricted date output for Forecast and History API method. (Required for History and Future API)
+    end_dt: Optional[:class:`int`]
+        Restricted date output for History API method. Only works for API on Pro plan and above.
+    hour: Optional[:class:`int`]
+        Restricted forecast or history output to a specific hour in a given day.
+    aqi: :class:`bool`
+        Indicates if Air Quality data has been enabled
+    tides: :class:`bool`
+        Indicates if tides data in the Marine API has been enabled
+    kwargs: Dict[:class:`str`, Any]
+        Additional keyword arguments passed by default to requests made by the client
+    """
+    def __init__(
+        self,
+        api_key: str,
+        lang: Optional[Union[str, Languages]] = None,
+        dt: Optional[int] = None,
+        end_dt: Optional[int] = None,
+        hour: Optional[int] = None,
+        aqi: bool = False,
+        tides: bool = False,
+        **kwargs: Dict[str, Any]
+    ) -> None:
+        lang_code = None
+        if lang is not None: 
+            lang_code = utils.find_language(lang, asobj=True)
+        opts = {
+            "key": api_key,
+            **kwargs
+        }
+        if lang_code: opts.update(lang = lang_code.value if lang_code is not None else None)
+
+        super().__init__(base_url=WEATHERAPI_BASE_URL,
+                         default_options=opts)
+        
+        self.dt = dt
+        self.end_dt = end_dt
+        self.hour = hour
+        self.aqi = aqi
+        self.tides = tides
+        self.kwargs = kwargs
+        self.lang = Languages(lang_code) if lang_code else None
+    
+    
+    def _call_request(self, endpoint: str, options: Dict[str, Any]) -> Dict[str, Any]:
+        """Private method used to make requests to WeatherAPI"""
+        final_options = self.default_options.copy()
+
+        for k,v in final_options.items(): # check - remove NoneType values
+            if v is None: del final_options[k]
+        # add options to final_options
+        for k,v in options.items():
+            # also - replace bool with "yes"/"no"
+            if v is not None: final_options[k] = BOOL_REPLACE.get(v, v)
+
+        resp = self._request(endpoint, **final_options)
+
+        if not resp[1].status_code < 400:
+            # raise errors yay
+            error_data = resp[0]["error"]
+            code = error_data["code"]
+            status = resp[1].status_code
+            msg = error_data["message"]
+
+            if code == 1006: raise NoLocationFound(status, code, msg)
+            elif code == 2006: raise InvalidAPIKey(status, code, msg)
+            elif code == 2007: raise APILimitExceeded(status, code, msg)
+            elif code == 2008: raise APIKeyDisabled(status, code, msg)
+            elif code == 2009: raise AccessDenied(status, code, msg)
+            elif code == 9999: raise InternalApplicationError(status, code, msg)
+            else: raise WeatherAPIException(status, code, msg)
+
+        return resp
+    
+    def event(self):
+        """A decorator that turns a function into an event. For example
+
+        .. code:: python
+
+            import weatherly
+            client = weatherly.Client(api_key=...)
+
+            @client.event
+            def on_error(payload):
+                print(f"An error occured! Payload: {payload}")
+        
+        In the example above, by adding ``@client.event`` the ``on_error`` function has turned into an error handler function
+        """
+        raise NotImplementedError
+
+    def set_language(self, lang: Union[str, Languages]) -> Optional[Languages]:
+        """Set client's language when requesting data.
+        
+        Parameters
+        -----------
+        lang: Union[:class:`str`, :class:`Languages`]
+            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
+            
+        Returns
+        ---------
+        Optional[:class:`Languages`]
+            An enum class representing the language of the client. Is ``None`` when something went wrong and the language was not set.
+        """
+        lang_class = utils.find_language(lang, asobj=True)
+        if not lang_class:
+            return None
+
+        self.lang = lang_class 
+        return self.lang
+
+    def get_current_weather(self, 
+        query: str, 
+        *,
+        lang: Optional[Union[str, Languages]] = None,
+        aqi: Optional[bool] = None,
+        **kwargs: Dict[str, Any]
+    ) -> CurrentWeatherData:
+        """Get current weather data
+
+        Parameters
+        ----------
+        query: :class:`str`
+            Query string - location you want to get weather data for
+        lang: Optional[Union[:class:`str`, Languages]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        aqi: Optional[:class:`bool`]
+            Enable/Disable Air Quality data in forecast API output. If nothing is passed, then it defaults to client default value.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments to request
+
+        Returns
+        -------
+        :class:`CurrentWeatherData`
+            Current weather data class
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "aqi": aqi or self.aqi,
+            "q": query,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+        resp = self._call_request("current.json", options)
+
+        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
+        return weather
+
+    def get_locations(self, query: str):
+        """Get locations for given query
+
+        Parameters
+        ---------------
+        query: :class:`str`
+            Query string, a location you are searching for
+
+        Returns
+        -----------
+        List[:class:`LocationData`]
+            A list of :class:`LocationData` classes.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        resp = self._call_request("search.json",{"q": query})
+
+        locations = []
+        for loc in resp[0]:
+            locations.append(LocationData(loc, resp[1].status_code, None))
+        return locations
+
+    def get_forecast_data(
+        self,
+        query: str, 
+        days: int,
+        *,
+        aqi: Optional[bool] = None,
+        alerts: Optional[bool] = None,
+        lang: Optional[Union[str, Languages]] = None,
+        **kwargs: Dict[str, Any]
+    ) -> ForecastData:
+        """Get forecast data from Forecast API
+
+        Parameters
+        -------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        days: :class:`int`
+            Number of days of weather forecast. Value ranges from 1 to 10
+        aqi: Optional[:class:`bool`]
+            Enable/Disable Air Quality data. Defaults to ``None`` (will use client's default)
+        alerts: Optional[:class:`bool`]
+            Enable/Disable alerts data. Defaults to ``None`` (will use client's default)
+        lang: Optional[Union[:class`str`, :class`Languages`]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`ForecastData`
+            Fetched forecast data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "aqi": aqi or self.aqi,
+            "q": query,
+            "alerts": alerts or self.kwargs.get("alerts"),
+            "days": days,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+
+        resp = self._call_request("forecast.json", options)
+        forecast = ForecastData(resp[0], resp[1].status_code, None)
+        return forecast
+
+    def get_historical_data(
+        self,
+        query: str,
+        date: str,
+        *,
+        aqi: Optional[bool] = None,
+        alerts: Optional[bool] = None,
+        lang: Optional[Union[str, Languages]] = None,
+        **kwargs: Dict[str, Any]
+    ) -> ForecastData:
+        """Retrieve historical data for given day and query. Uses History API.
+
+        Parameters
+        -----------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        date: :class:`str`
+            A date string in format yyyy-mm-dd representing the day you want to get data for
+        aqi: Optional[:class:`bool`]
+            Enable/Disable Air Quality data. Defaults to ``None`` (will use client's default)
+        alerts: Optional[:class:`bool`]
+            Enable/Disable alerts data. Defaults to ``None`` (will use client's default)
+        lang: Optional[Union[:class`str`, :class`Languages`]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+        
+        Returns
+        ----------
+        :class:`ForecastData`
+            Forecast data for given day and query.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        :exc:`InvalidDate`
+            Raised when the ``date`` parameter is invalid (doesn't match the format or isn't a date before (or) today)
+        """
+        options = {
+            "aqi": aqi or self.aqi,
+            "q": query,
+            "alerts": alerts or self.kwargs.get("alerts"),
+            "dt": date,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+
+        # check if given date is really "historical"
+        try:
+            splitted = date.split("-")
+            datetuple = datetime.datetime(
+                int(splitted[0]), 
+                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
+                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
+                0,0)
+            epoch = datetuple.timestamp()
+        except Exception as exc:
+            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
+
+        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
+
+        if epoch > now: raise InvalidDate("Date should be before current time, switch from History API to Future to use future dates.")
+
+        resp = self._call_request("history.json", options)
+        history = ForecastData(resp[0], resp[1].status_code, None)
+        return history
+        
+    def get_future_data(
+        self,
+        query: str,
+        date: str,
+        *,
+        lang: Optional[Union[str, Languages]] = None,
+        **kwargs: Dict[str, Any]
+    ) -> FutureData:
+        """Retrieve future data for given day and query. Uses Future API.
+
+        Parameters
+        -----------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        date: :class:`str`
+            A date string in format yyyy-mm-dd representing the day you want to get data for
+        lang: Optional[Union[:class`str`, :class`Languages`]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+        
+        Returns
+        ----------
+        :class:`FutureData`
+            Future data for given day and query.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        :exc:`InvalidDate`
+            Raised when the ``date`` parameter is invalid (doesn't match the format or isn't a date after today)
+        """
+        options = {
+            "q": query,
+            "dt": date,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+
+        # check if given date is really "historical"
+        try:
+            splitted = date.split("-")
+            datetuple = datetime.datetime(
+                int(splitted[0]), 
+                int(splitted[1][1:]) if splitted[1].startswith("0") else int(splitted[1]), 
+                int(splitted[2][1:]) if splitted[2].startswith("0") else int(splitted[2]),
+                0,0)
+            epoch = datetuple.timestamp()
+        except Exception as exc:
+            raise InvalidDate(f"Failed to convert date {date}: Invalid format") from exc
+
+        now = datetime.datetime.timestamp(datetime.datetime.utcnow())
+
+        if epoch < now: raise InvalidDate("Date should be after current time, switch from Future API to History to use past dates.")
+
+        resp = self._call_request("future.json", options)
+        future = FutureData(resp[0], resp[1].status_code, None)
+        return future
+        
+    def get_astronomical_data(
+        self,
+        query: str,
+        date: str,
+        **kwargs: Dict[str, Any]
+    ) -> AstronomicalData:
+        """Get astronomical data from Astronomy API
+
+        Parameters
+        -------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        date: :class:`str`
+            Date in format yyyy-MM-dd and on or after 1st Jan, 2010 (2010-01-01)
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`AstronomicalData`
+            Fetched astronomical data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "q": query,
+            "dt": date,
+            **kwargs
+        }
+        resp = self._call_request("astronomy.json", options)
+        astro = AstronomicalData(resp[0], resp[1].status_code, None)
+        return astro
+
+    def get_marine_data(
+        self,
+        query: str,
+        *,
+        tides: Optional[bool] = None,
+        **kwargs: Dict[str, Any]
+    ) -> MarineData:
+        """Get marine data from Marine API
+
+        Parameters
+        -------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        tides: Optional[:class:`bool`]
+            Enable/disable tide data.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`MarineData`
+            Fetched marine data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "q": query,
+            "tides": tides or self.tides,
+            **kwargs
+        }
+        resp = self._call_request("marine.json", options)
+        marine = MarineData(resp[0], resp[1].status_code, None)
+        return marine
+
+    def get_ip_data(
+        self,
+        ip_address: str,
+        **kwargs: Dict[str, Any]
+    ) -> IPData:
+        """
+        Look for data for the given IP address.
+
+        Parameters
+        -------------
+        ip_address: :class:`str`
+            IP address you want to get data for. Can be ipv4 or ipv6
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`IPData`
+            Fetched IP data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when either IP address was invalid or no matching location was found.
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "q": ip_address,
+            **kwargs
+        }
+        resp = self._call_request("ip.json", options)
+        ip = IPData(resp[0], resp[1].status_code, None)
+        return ip
+
+    def get_sports_data(
+        self,
+        query: str,
+        **kwargs: Dict[str, Any]
+    ) -> SportsData:
+        """
+        Get sports data for a given query. Uses Sports API.
+
+        Parameters
+        -------------
+        query: :class:`str`
+            Query string, location you want to get sports data for
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`SportsData`
+            Retrieved sports data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when either IP address was invalid or no matching location was found.
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "q": query,
+            **kwargs
+        }
+        resp = self._call_request("sports.json", options)
+        sports = SportsData(resp[0], resp[1].status_code, None)
+        return sports
+
+
+    
+    def __str__(self):
+        return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
+    
+    def __repr__(self):
+        return repr(self.__str__())
```

### Comparing `weatherly-0.7.0/weatherly/api/core.py` & `weatherly-0.8.0/weatherly/api/core.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from typing import (
-    Any,
-    Optional,
-    List,
-    Tuple,
-    Literal,
-    Dict,
-    TypeVar
-)
-import urllib
-import requests
-from ..utils import parse_kwargs_to_urlargs
-import json
-
-T = TypeVar("T")
-
-__all__ = (
-    "BaseAPIClient",
-)
-
-class BaseAPIClient():
-    """
-    Represents a base API client that can handle requests. Used as a base class for :class:`Client`
-    
-    Parameters
-    ----------
-    base_url: :class:`str`
-        An URL that will be used as a base for requests.
-    default_options: Optional[Dict[:class:`str`, Any]]
-        Default options for requests made by the client that will be automatically added.
-    """
-    def __init__(
-        self,
-        base_url: str,
-        default_options: Optional[Dict[str, Any]]
-    ) -> None:
-        self.url = base_url
-        self.default_options = default_options or {}
-        
-    def _request(
-        self,
-        path: str,
-        **kwargs: Optional[Dict[str, str]]
-    ) -> Tuple[Dict[Any, Any], requests.Response]:
-        """
-        Request data from the base URL + path.
-        Private function, use :class:`Client` methods instead
-        
-        Parameters
-        ----------
-        path: :class:`str`
-            A path that will be used as an endpoint for the request.
-        kwargs: Optional[Dict[str, str]]
-            Additional parameters for the request.
-        """
-        full_url = self.url + path + parse_kwargs_to_urlargs({**self.default_options, **kwargs})
-
-        response = requests.get(full_url)
-        return response.json(), response
-        
-        
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import (
+    Any,
+    Optional,
+    List,
+    Tuple,
+    Literal,
+    Dict,
+    TypeVar
+)
+import urllib
+import requests
+from ..utils import parse_kwargs_to_urlargs
+import json
+
+T = TypeVar("T")
+
+__all__ = (
+    "BaseAPIClient",
+)
+
+class BaseAPIClient():
+    """
+    Represents a base API client that can handle requests. Used as a base class for :class:`Client`
+    
+    Parameters
+    ----------
+    base_url: :class:`str`
+        An URL that will be used as a base for requests.
+    default_options: Optional[Dict[:class:`str`, Any]]
+        Default options for requests made by the client that will be automatically added.
+    """
+    def __init__(
+        self,
+        base_url: str,
+        default_options: Optional[Dict[str, Any]]
+    ) -> None:
+        self.url = base_url
+        self.default_options = default_options or {}
+        
+    def _request(
+        self,
+        path: str,
+        **kwargs: Optional[Dict[str, str]]
+    ) -> Tuple[Dict[Any, Any], requests.Response]:
+        """
+        Request data from the base URL + path.
+        Private function, use :class:`Client` methods instead
+        
+        Parameters
+        ----------
+        path: :class:`str`
+            A path that will be used as an endpoint for the request.
+        kwargs: Optional[Dict[str, str]]
+            Additional parameters for the request.
+        """
+        full_url = self.url + path + parse_kwargs_to_urlargs({**self.default_options, **kwargs})
+
+        response = requests.get(full_url)
+        return response.json(), response
+        
+
```

### Comparing `weatherly-0.7.0/weatherly/enums.py` & `weatherly-0.8.0/weatherly/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,195 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from enum import Enum
-
-__all__ = (
-    "Languages",
-    "SportsEventType",
-)
-
-class Languages(Enum):
-    """
-    Languages - an enum representing languages available for use in the WeatherAPI requests.
-    
-    Attributes are languages and language codes
-    
-    Attributes
-    ----------
-    Arabic: :class:`str`
-        Language code: ar
-    Bengali: :class:`str`
-        Language code: bn
-    Bulgarian: :class:`str`
-        Language code: bg
-    ChineseSimplified: :class:`str`
-        Language code: zh
-    ChineseTraditional: :class:`str`
-        Language code: zh_tw
-    Czech: :class:`str`
-        Language code: cs
-    Danish: :class:`str`
-        Language code: da
-    Dutch: :class:`str`
-        Language code: nl
-    Finnish: :class:`str`
-        Language code: fi
-    French: :class:`str`
-        Language code: fr
-    German: :class:`str`
-        Language code: de
-    Greek: :class:`str`
-        Language code: el
-    Hindi: :class:`str`
-        Language code: hi
-    Hungarian: :class:`str`
-        Language code: hu
-    Italian: :class:`str`
-        Language code: it
-    Japanese: :class:`str`
-        Language code: ja
-    Javanese: :class:`str`
-        Language code: jv
-    Korean: :class:`str`
-        Language code: ko
-    Mandarin: :class:`str`
-        Language code: zh_cmn
-    Marathi: :class:`str`
-        Language code: mr
-    Polish: :class:`str`
-        Language code: pl
-    Portuguese: :class:`str`
-        Language code: pt
-    Punjabi: :class:`str`
-        Language code: pa
-    Romanian: :class:`str`
-        Language code: ro
-    Russian: :class:`str`
-        Language code: ru
-    Serbian: :class:`str`
-        Language code: sr
-    Sinhalese: :class:`str`
-        Language code: si
-    Slovak: :class:`str`
-        Language code: sk
-    Spanish: :class:`str`
-        Language code: es
-    Swedish: :class:`str`
-        Language code: sv
-    Tamil: :class:`str`
-        Language code: ta
-    Telugu: :class:`str`
-        Language code: te
-    Turkish: :class:`str`
-        Language code: tr
-    Ukrainian: :class:`str`
-        Language code: uk
-    Urdu: :class:`str`
-        Language code: ur
-    Vietnamese: :class:`str`
-        Language code: vi
-    WuShanghainese: :class:`str`
-        Language code: zh_wuu
-    Xiang: :class:`str`
-        Language code: zh_hsn
-    YueCantonese: :class:`str`
-        Language code: zh_yue
-    Zulu: :class:`str`
-        Language code: zu
-    """
-    Arabic: str = "ar"
-    Bengali: str = "bn"
-    Bulgarian: str = "bg"
-    ChineseSimplified: str = "zh"
-    ChineseTraditional: str = "zh_tw"
-    Czech: str = "cs"
-    Danish: str = "da"
-    Dutch: str = "nl"
-    Finnish: str = "fi"
-    French: str = "fr"
-    German: str = "de"
-    Greek: str = "el"
-    Hindi: str = "hi"
-    Hungarian: str = "hu"
-    Italian: str = "it"
-    Japanese: str = "ja"
-    Javanese: str = "jv"
-    Korean: str = "ko"
-    Mandarin: str = "zh_cmn"
-    Marathi: str = "mr"
-    Polish: str = "pl"
-    Portuguese: str = "pt"
-    Punjabi: str = "pa"
-    Romanian: str = "ro"
-    Russian: str = "ru"
-    Serbian: str = "sr"
-    Sinhalese: str = "si"
-    Slovak: str = "sk"
-    Spanish: str = "es"
-    Swedish: str = "sv"
-    Tamil: str = "ta"
-    Telugu: str = "te"
-    Turkish: str =	"tr"
-    Ukrainian: str = "uk"
-    Urdu: str = "ur"
-    Vietnamese: str = "vi"
-    WuShanghainese: str = "zh_wuu"
-    Xiang: str = "zh_hsn"
-    YueCantonese: str =	"zh_yue"
-    Zulu: str = "zu"
-
-class SportsEventType(Enum):
-    """
-    An enum representing type of sports event
-
-    Attributes
-    ---------------
-    football
-        Football event
-    cricket
-        Cricket event
-    golf
-        Golf event
-    """
-    football = 1
-    cricket = 2
-    golf = 3
-
-    def __str__(self):
-        return f"<SportsEventType: {self.name}>"
-
-    def __repr__(self):
-        return repr(self.__str__())
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from enum import Enum
+
+__all__ = (
+    "Languages",
+    "SportsEventType",
+    "TideHeight",
+)
+
+class Languages(Enum):
+    """Languages - an enum representing languages available for use in the WeatherAPI requests.
+    
+    Attributes are languages and language codes
+    
+    Attributes
+    ----------
+    Arabic: :class:`str`
+        Language code: ar
+    Bengali: :class:`str`
+        Language code: bn
+    Bulgarian: :class:`str`
+        Language code: bg
+    ChineseSimplified: :class:`str`
+        Language code: zh
+    ChineseTraditional: :class:`str`
+        Language code: zh_tw
+    Czech: :class:`str`
+        Language code: cs
+    Danish: :class:`str`
+        Language code: da
+    Dutch: :class:`str`
+        Language code: nl
+    Finnish: :class:`str`
+        Language code: fi
+    French: :class:`str`
+        Language code: fr
+    German: :class:`str`
+        Language code: de
+    Greek: :class:`str`
+        Language code: el
+    Hindi: :class:`str`
+        Language code: hi
+    Hungarian: :class:`str`
+        Language code: hu
+    Italian: :class:`str`
+        Language code: it
+    Japanese: :class:`str`
+        Language code: ja
+    Javanese: :class:`str`
+        Language code: jv
+    Korean: :class:`str`
+        Language code: ko
+    Mandarin: :class:`str`
+        Language code: zh_cmn
+    Marathi: :class:`str`
+        Language code: mr
+    Polish: :class:`str`
+        Language code: pl
+    Portuguese: :class:`str`
+        Language code: pt
+    Punjabi: :class:`str`
+        Language code: pa
+    Romanian: :class:`str`
+        Language code: ro
+    Russian: :class:`str`
+        Language code: ru
+    Serbian: :class:`str`
+        Language code: sr
+    Sinhalese: :class:`str`
+        Language code: si
+    Slovak: :class:`str`
+        Language code: sk
+    Spanish: :class:`str`
+        Language code: es
+    Swedish: :class:`str`
+        Language code: sv
+    Tamil: :class:`str`
+        Language code: ta
+    Telugu: :class:`str`
+        Language code: te
+    Turkish: :class:`str`
+        Language code: tr
+    Ukrainian: :class:`str`
+        Language code: uk
+    Urdu: :class:`str`
+        Language code: ur
+    Vietnamese: :class:`str`
+        Language code: vi
+    WuShanghainese: :class:`str`
+        Language code: zh_wuu
+    Xiang: :class:`str`
+        Language code: zh_hsn
+    YueCantonese: :class:`str`
+        Language code: zh_yue
+    Zulu: :class:`str`
+        Language code: zu
+    """
+    Arabic: str = "ar"
+    Bengali: str = "bn"
+    Bulgarian: str = "bg"
+    ChineseSimplified: str = "zh"
+    ChineseTraditional: str = "zh_tw"
+    Czech: str = "cs"
+    Danish: str = "da"
+    Dutch: str = "nl"
+    Finnish: str = "fi"
+    French: str = "fr"
+    German: str = "de"
+    Greek: str = "el"
+    Hindi: str = "hi"
+    Hungarian: str = "hu"
+    Italian: str = "it"
+    Japanese: str = "ja"
+    Javanese: str = "jv"
+    Korean: str = "ko"
+    Mandarin: str = "zh_cmn"
+    Marathi: str = "mr"
+    Polish: str = "pl"
+    Portuguese: str = "pt"
+    Punjabi: str = "pa"
+    Romanian: str = "ro"
+    Russian: str = "ru"
+    Serbian: str = "sr"
+    Sinhalese: str = "si"
+    Slovak: str = "sk"
+    Spanish: str = "es"
+    Swedish: str = "sv"
+    Tamil: str = "ta"
+    Telugu: str = "te"
+    Turkish: str =	"tr"
+    Ukrainian: str = "uk"
+    Urdu: str = "ur"
+    Vietnamese: str = "vi"
+    WuShanghainese: str = "zh_wuu"
+    Xiang: str = "zh_hsn"
+    YueCantonese: str =	"zh_yue"
+    Zulu: str = "zu"
+
+class SportsEventType(Enum):
+    """An enum representing type of sports event
+
+    Attributes
+    ---------------
+    football
+        Football event
+    cricket
+        Cricket event
+    golf
+        Golf event
+    """
+    football = 1
+    cricket = 2
+    golf = 3
+
+    def __str__(self):
+        return f"<SportsEventType: {self.name}>"
+
+    def __repr__(self):
+        return repr(self.__str__())
+
+class TideHeight(Enum):
+    """An enum representing tide height i.e. HIGH or LOW
+
+    Attributes
+    ----------------
+    HIGH
+        When the tide is high
+    LOW
+        When the tide is low
+    """
+    LOW = 0
+    HIGH = 1
```

### Comparing `weatherly-0.7.0/weatherly/errors.py` & `weatherly-0.8.0/weatherly/errors.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-__all__ = (
-    "WeatherlyException",
-    "WeatherAPIException",
-    "NoLocationFound",
-    "InvalidAPIKey",
-    "APILimitExceeded",
-    "APIKeyDisabled",
-    "AccessDenied",
-    "InternalApplicationError",
-    "InvalidDate",
-)
-
-class WeatherlyException(Exception):
-    """
-    A base class for all ``weatherly`` exceptions. Almost all exceptions of this module inherit from this class.
-
-    Inherits from :class:`Exception`.
-    """
-    pass
-
-class InvalidDate(WeatherlyException):
-    """
-    Raised when a date (for History/Future API) is invalid.
-
-    Inherits from :class:`WeatherlyException`.
-    """
-    pass
-
-class WeatherAPIException(WeatherlyException): 
-    """
-    The base class for :class:`Client` weather requests exceptions.
-    
-    Parameters
-    ----------
-    status: :class:`int`
-        HTTP status code
-    code: :class:`int`
-        Error code
-    message: :class:`str`
-        Message provided with the error
-    """
-    def __init__(self, status: int, code: int, message: str, *args):
-        self.status = status
-        self.code = code
-        self.message = message
-        self.formatted_message = f"{self.status} (error code {self.code}): {message}"
-        super().__init__(self.formatted_message, *args)
-
-class NoLocationFound(WeatherAPIException): 
-    """
-    Exception like this is raised when no location was found when searching for weather data.
-
-    Usually has status code  400 and error code 1006.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class InvalidAPIKey(WeatherAPIException): 
-    """
-    Exception like this is raised when provided API key is invalid
-
-    Usually has status code 401 and error code 2006.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class APILimitExceeded(WeatherAPIException): 
-    """
-    Exception like this is raised when API key has exceeded monthly calls limit.
-
-    Usually has status code 400 and error code 2007.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class APIKeyDisabled(WeatherAPIException): 
-    """
-    Exception like this is raised when API key has been disabled.
-
-    Usually has status code 403 and error code 2008.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class AccessDenied(WeatherAPIException): 
-    """
-    Exception like this is raised when API key does not have access to requested resource.
-
-    Usually has status code 403 and error code 2009.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class InternalApplicationError(WeatherAPIException): 
-    """
-    Exception like this is raised when an internal application error occured. There is nothing to do about it.
-
-    Usually has status code 400 and error code 9999.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+__all__ = (
+    "WeatherlyException",
+    "WeatherAPIException",
+    "NoLocationFound",
+    "InvalidAPIKey",
+    "APILimitExceeded",
+    "APIKeyDisabled",
+    "AccessDenied",
+    "InternalApplicationError",
+    "InvalidDate",
+)
+
+class WeatherlyException(Exception):
+    """
+    A base class for all ``weatherly`` exceptions. Almost all exceptions of this module inherit from this class.
+
+    Inherits from :class:`Exception`.
+    """
+    pass
+
+class InvalidDate(WeatherlyException):
+    """
+    Raised when a date (for History/Future API) is invalid.
+
+    Inherits from :class:`WeatherlyException`.
+    """
+    pass
+
+class WeatherAPIException(WeatherlyException): 
+    """
+    The base class for :class:`Client` weather requests exceptions.
+    
+    Parameters
+    ----------
+    status: :class:`int`
+        HTTP status code
+    code: :class:`int`
+        Error code
+    message: :class:`str`
+        Message provided with the error
+    """
+    def __init__(self, status: int, code: int, message: str, *args):
+        self.status = status
+        self.code = code
+        self.message = message
+        self.formatted_message = f"{self.status} (error code {self.code}): {message}"
+        super().__init__(self.formatted_message, *args)
+
+class NoLocationFound(WeatherAPIException): 
+    """
+    Exception like this is raised when no location was found when searching for weather data.
+
+    Usually has status code  400 and error code 1006.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class InvalidAPIKey(WeatherAPIException): 
+    """
+    Exception like this is raised when provided API key is invalid
+
+    Usually has status code 401 and error code 2006.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class APILimitExceeded(WeatherAPIException): 
+    """
+    Exception like this is raised when API key has exceeded monthly calls limit.
+
+    Usually has status code 400 and error code 2007.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class APIKeyDisabled(WeatherAPIException): 
+    """
+    Exception like this is raised when API key has been disabled.
+
+    Usually has status code 403 and error code 2008.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class AccessDenied(WeatherAPIException): 
+    """
+    Exception like this is raised when API key does not have access to requested resource.
+
+    Usually has status code 403 and error code 2009.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class InternalApplicationError(WeatherAPIException): 
+    """
+    Exception like this is raised when an internal application error occured. There is nothing to do about it.
+
+    Usually has status code 400 and error code 9999.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
     pass
```

### Comparing `weatherly-0.7.0/weatherly/utils.py` & `weatherly-0.8.0/weatherly/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from typing import (
-    Dict,
-    Any,
-    overload
-)
-from .enums import Languages
-
-gray = "#535353"
-white = "#ffffff"
-
-def parse_kwargs_to_urlargs(kwargs: Dict[str, Any]) -> str:
-    """
-    Parses keyword arguments (kwargs) to format fitting URLs
-    Example: ``{"some_key": "some value", "yes": "no"}`` -> ``?some_key=some_value&yes=no``
-    
-    Parameters
-    ----------
-    kwargs: Dict[:class:`str`, Any]
-        A dictionary of keyword arguments to be parsed.
-        
-    Returns
-    -------
-    args_string: :class:`str`
-        A string - formatted keyword arguments
-    """
-    if not kwargs: return ""
-    
-    args_string = ""
-    first = True
-    
-    for k,v in kwargs.items():
-        args_string += f"{'?' if first else '&'}{k}={v}"
-        first = False
-    return args_string
-
-@overload
-def find_language(lang: str, asobj: bool=False) -> None:
-    ...
-    
-@overload
-def find_language(lang: str, asobj: bool=False) -> Languages:
-    ...
-
-def find_language(lang: str, asobj: bool=False) -> str:
-    """
-    Used to find language code from available languages.
-
-    Paremeters
-    ----------
-    lang: :class:`str`
-        A language you want to search for
-
-    Returns
-    -------
-    Union[:class:`str`, :class:`Languages`, None]
-        Language code, could be ``None``, could be a :class:`Languages` enum.
-    """
-
-    if isinstance(lang, Languages):
-        try:
-            if asobj: return lang
-            return lang.value
-        except: 
-            return None
-
-    lang = lang.lower()
-
-    for language in Languages:
-        if language.name.lower() == lang or language.value == lang:
-            if asobj: return language
-            return language.value
-        
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import (
+    Dict,
+    Any,
+    overload
+)
+from .enums import Languages
+
+gray = "#535353"
+white = "#ffffff"
+
+def parse_kwargs_to_urlargs(kwargs: Dict[str, Any]) -> str:
+    """
+    Parses keyword arguments (kwargs) to format fitting URLs
+    Example: ``{"some_key": "some value", "yes": "no"}`` -> ``?some_key=some_value&yes=no``
+    
+    Parameters
+    ----------
+    kwargs: Dict[:class:`str`, Any]
+        A dictionary of keyword arguments to be parsed.
+        
+    Returns
+    -------
+    args_string: :class:`str`
+        A string - formatted keyword arguments
+    """
+    if not kwargs: return ""
+    
+    args_string = ""
+    first = True
+    
+    for k,v in kwargs.items():
+        args_string += f"{'?' if first else '&'}{k}={v}"
+        first = False
+    return args_string
+
+@overload
+def find_language(lang: str, asobj: bool=False) -> None:
+    ...
+    
+@overload
+def find_language(lang: str, asobj: bool=False) -> Languages:
+    ...
+
+def find_language(lang: str, asobj: bool=False) -> str:
+    """
+    Used to find language code from available languages.
+
+    Paremeters
+    ----------
+    lang: :class:`str`
+        A language you want to search for
+
+    Returns
+    -------
+    Union[:class:`str`, :class:`Languages`, None]
+        Language code, could be ``None``, could be a :class:`Languages` enum.
+    """
+
+    if isinstance(lang, Languages):
+        try:
+            if asobj: return lang
+            return lang.value
+        except: 
+            return None
+
+    lang = lang.lower()
+
+    for language in Languages:
+        if language.name.lower() == lang or language.value == lang:
+            if asobj: return language
+            return language.value
+        
     return None
```

### Comparing `weatherly-0.7.0/weatherly.egg-info/PKG-INFO` & `weatherly-0.8.0/weatherly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,92 @@
-Metadata-Version: 2.1
-Name: weatherly
-Version: 0.7.0
-Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
-Home-page: https://github.com/konradsic/weatherly
-Author: konradsic
-License: MIT
-Project-URL: Issues, https://github.com/konradsic/weatherly/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-⛅ weatherly
-====================
-.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
-    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
-    :alt: Weatherly license
-.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Weatherly version on PyPI
-.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Supported Python versions
-.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Project status
-.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
-    :target: https://github.com/konradsic/weatherly
-    :alt: Build status
-
-Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
-
-Features
----------------
-* Easy to use,
-* Intuitive design,
-* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
-* Modern and typed Python package,
-* Support for languages (provided by WeatherAPI)
-
-Installing
-------------
-To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
-
-.. code:: shell
-    
-    # Windows
-    py -3 -m pip install -U weatherly
-
-    # MacOS / Linux
-    python3 -m pip install -U weatherly
-
-Congratulations! Now weatherly is ready to use on your machine.
-
-Code example
----------------------
-
-.. code:: python
-
-    import weatherly
-    
-    client = weatherly.Client(api_key="your WeatherAPI key")
-    # you can set language to all request, or pass it manually
-    client.set_language("fr")     # lang code
-    client.set_language("German") # language full name
-
-    # getting weather info
-    current_weather = client.get_current_weather(query="London")
-
-    # getting forecast info
-    forecast = client.get_forecast_data(query="Paris", days=3)
-
-    # historical data
-    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
-
-    # marine data
-    marine = client.get_marine_data(query="Madrid")
-
-
+Metadata-Version: 2.1
+Name: weatherly
+Version: 0.8.0
+Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
+Home-page: https://github.com/konradsic/weatherly
+Author: konradsic
+License: MIT
+Project-URL: Issues, https://github.com/konradsic/weatherly/issues
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+⛅ weatherly
+====================
+.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
+    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
+    :alt: Weatherly license
+.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Weatherly version on PyPI
+.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Supported Python versions
+.. image:: https://img.shields.io/pypi/status/weatherly?style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Project status
+.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
+    :target: https://github.com/konradsic/weatherly
+    :alt: Build status
+
+Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
+
+Features
+---------------
+* Easy to use,
+* Intuitive design,
+* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
+* Modern and typed Python package,
+* Support for languages (provided by WeatherAPI)
+
+Installing
+------------
+To install weatherly on your computer Python 3.10 or higher is required. If your python version meets the requirements run:
+
+.. code:: shell
+    
+    # Windows
+    py -3 -m pip install -U weatherly
+
+    # MacOS / Linux
+    python3 -m pip install -U weatherly
+
+Congratulations! Now weatherly is ready to use on your machine.
+
+Code example
+---------------------
+
+.. code:: python
+
+    import weatherly
+    
+    client = weatherly.Client(api_key="your WeatherAPI key")
+    # you can set language to all requests, or pass it manually
+    client.set_language("fr")     # lang code
+    client.set_language("German") # language full name
+
+    # getting weather info
+    current_weather = client.get_current_weather(query="London")
+
+    # getting forecast info
+    forecast = client.get_forecast_data(query="Paris", days=3)
+
+    # historical data
+    history = client.get_historical_data(query="48.8567,2.3508", date="2010-01-01") # query could also be latitude,longitude
+
+    # marine data
+    marine = client.get_marine_data(query="Madrid")
```

