# Comparing `tmp/openremote-cli-0.6.8.tar.gz` & `tmp/openremote-cli-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openremote-cli-0.6.8.tar", max compression
+gzip compressed data, was "openremote-cli-0.6.9.tar", max compression
```

## Comparing `openremote-cli-0.6.8.tar` & `openremote-cli-0.6.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   153837 2021-03-30 11:35:55.918613 openremote-cli-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     3582 2021-03-30 11:35:55.918613 openremote-cli-0.6.8/README.md
--rw-r--r--   0        0        0    20490 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/cli.py
--rw-r--r--   0        0        0     3314 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/config.py
--rw-r--r--   0        0        0     1795 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/email.py
--rw-r--r--   0        0        0     2010 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/gen_aws_smtp_credentials.py
--rw-r--r--   0        0        0    23336 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/scripts.py
--rw-r--r--   0        0        0     1371 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/openremote_cli/shell.py
--rw-r--r--   0        0        0     1006 2021-03-30 11:35:55.922613 openremote-cli-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     4663 2021-03-30 11:36:26.803890 openremote-cli-0.6.8/setup.py
--rw-r--r--   0        0        0     4619 2021-03-30 11:36:26.804880 openremote-cli-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0   153837 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     3582 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/README.md
+-rw-r--r--   0        0        0    20490 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/cli.py
+-rw-r--r--   0        0        0     3340 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/config.py
+-rw-r--r--   0        0        0     1795 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/email.py
+-rw-r--r--   0        0        0     2010 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/gen_aws_smtp_credentials.py
+-rw-r--r--   0        0        0    23525 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/scripts.py
+-rw-r--r--   0        0        0     1371 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/openremote_cli/shell.py
+-rw-r--r--   0        0        0     1006 2021-04-02 14:20:48.202035 openremote-cli-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     4663 2021-04-02 14:21:18.966489 openremote-cli-0.6.9/setup.py
+-rw-r--r--   0        0        0     4619 2021-04-02 14:21:18.967515 openremote-cli-0.6.9/PKG-INFO
```

### Comparing `openremote-cli-0.6.8/LICENSE.txt` & `openremote-cli-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/README.md` & `openremote-cli-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/openremote_cli/cli.py` & `openremote-cli-0.6.9/openremote_cli/cli.py`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/openremote_cli/config.py` & `openremote-cli-0.6.9/openremote_cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,22 @@
     aws = config['AWS']
     PROFILE = aws['profile']
     BUCKET = aws['bucket']
     REGION = aws['region']
     SMTP_SERVER = f'email-smtp.{REGION}.amazonaws.com'
 
     # Runtime config
-    global DRY_RUN, LEVEL, VERBOSE, TELEMETRY, QUIET
+    global DRY_RUN, LEVEL, VERBOSE, TELEMETRY, QUIET, TIMEOUT
 
     VERBOSE = False
     DRY_RUN = False
     TELEMETRY = True
     QUIET = False
     LEVEL = 'logging.ERROR'
+    TIMEOUT = 20
 
 
 def store_token(url, username, password, refresh):
     config = configparser.ConfigParser()
     config.read(_config_file_name())
     try:
         # first try to update
```

### Comparing `openremote-cli-0.6.8/openremote_cli/email.py` & `openremote-cli-0.6.9/openremote_cli/email.py`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/openremote_cli/gen_aws_smtp_credentials.py` & `openremote-cli-0.6.9/openremote_cli/gen_aws_smtp_credentials.py`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/openremote_cli/scripts.py` & `openremote-cli-0.6.9/openremote_cli/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import string
 import requests
 import ssl
 import time
 import emojis
 import re
+import functools
 
 
 from keycloak import KeycloakOpenID
 from random import choice, randint
 from openremote_cli import shell
 from openremote_cli import config
 from openremote_cli import gen_aws_smtp_credentials, email
@@ -548,36 +549,78 @@
             raise Exception(f'{url}: no login page after {delay}s')
     driver.type(user, into='username')
     driver.type(config.get_password(url, user), into='password')
     driver.click('SIGN IN')
     driver.click('LOG IN')
     end = time.time()
     if not config.QUIET:
-        print(f'{url} login time\t{end-start}s')
+        print(f'{url} login time\t{end-start:.2f}s')
     return driver
 
 
-def _manager_ui_wait_map(driver, url, delay=20):
-    start = time.time()
-    end = start
-    while end - start < delay:
-        try:
-            driver.execute_script(
-                "document.querySelector('or-app').shadowRoot"
-                ".querySelector('page-map').shadowRoot"
-            )
-            if not config.QUIET:
-                print(f"{url} map OK\t{end-start}s")
-            return 0
-        except:
-            if not config.QUIET:
-                print('.', end='', flush=True)
-            time.sleep(0.2)
-            end = time.time()
-    raise Exception(f"{url}: No map shown after login after {delay}s")
+def timeout(func):
+    @functools.wraps(func)
+    def inner(*args, **kwargs):
+        start = time.time()
+        while time.time() - start < config.TIMEOUT:
+            try:
+                result = func(*args, **kwargs)
+                if not config.QUIET:
+                    print(f' {func.__name__!r}: OK {time.time() - start:.2f}s')
+                return result
+            except:
+                if not config.QUIET:
+                    print('.', end='', flush=True)
+                time.sleep(0.1)
+        raise Exception(f'{func.__name__!r}: timeout {config.TIMEOUT}s')
+
+    return inner
+
+
+@timeout
+def _manager_ui_wait_map(driver, url):
+    driver.execute_script(
+        "document.querySelector('or-app').shadowRoot"
+        ".querySelector('page-map').shadowRoot"
+    )
+
+
+@timeout
+def _manager_ui_add_asset_dialog(driver, url):
+    driver.execute_script(
+        "document.querySelector('or-app').shadowRoot"
+        ".querySelector('page-assets').shadowRoot"
+        ".querySelector('or-asset-tree').shadowRoot"
+        ".querySelector('or-input[icon=plus]').shadowRoot"
+        ".querySelector('button').click()"
+    )
+
+
+@timeout
+def _manager_ui_add_http_weather_agent(driver, url):
+    driver.execute_script(
+        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-input').shadowRoot.querySelector('input').value = 'Weather Agent'"
+    )
+    driver.execute_script(
+        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-input').shadowRoot.querySelector('input').dispatchEvent(new Event('change'))"
+    )
+
+
+@timeout
+def _manager_ui_select_http_agent(driver, url):
+    driver.execute_script(
+        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-mwc-list').shadowRoot.querySelectorAll('span')[3].click()"
+    )
+
+
+@timeout
+def _manager_ui_press_add(driver, url):
+    driver.execute_script(
+        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-input[id=add-btn]').click()"
+    )
 
 
 def manager_test_http_rest(delay, quit):
     url = 'staging.demo.openremote.io'
     user = 'admin'
     print(f"0. Login into {url}")
     driver = _manager_ui_login(url, user)
@@ -586,51 +629,24 @@
     print("1. Go to the 'Assets' page in the webapp")
     time.sleep(delay)
     driver.go_to(f'https://{url}/manager/#!assets')
     print(
         "2. Open the add asset dialog by clicking the '+' icon in the asset tree on the left."
     )
     time.sleep(delay)
-    cnt = 0
-    while cnt < 1000000:
-        try:
-            driver.execute_script(
-                "document.querySelector('or-app').shadowRoot"
-                ".querySelector('page-assets').shadowRoot"
-                ".querySelector('or-asset-tree').shadowRoot"
-                ".querySelector('or-input[icon=plus]').shadowRoot"
-                ".querySelector('button').click()"
-            )
-            cnt = 1000000
-        except:
-            if not config.QUIET:
-                print('.', end='', flush=True)
-            time.sleep(0.2)
-            cnt += 1
-            time.sleep(0.2)
-            if cnt > 150:
-                raise Exception(f"{url}: Timeout waiting for dialog")
+    _manager_ui_add_asset_dialog(driver, url)
     print("3. Give the asset the name 'Weather Agent'")
     time.sleep(delay)
-    driver.execute_script(
-        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-input').shadowRoot.querySelector('input').value = 'Weather Agent'"
-    )
-    driver.execute_script(
-        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-input').shadowRoot.querySelector('input').dispatchEvent(new Event('change'))"
-    )
+    _manager_ui_add_http_weather_agent(driver, url)
     print("4. and select the asset type 'HTTP Client Agent' from the list.")
     time.sleep(delay)
-    driver.execute_script(
-        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-add-asset-dialog').shadowRoot.querySelector('or-mwc-list').shadowRoot.querySelectorAll('span')[3].click()"
-    )
+    _manager_ui_select_http_agent(driver, url)
     print("5. Press 'Add'")
     time.sleep(delay)
-    driver.execute_script(
-        "document.querySelector('or-mwc-dialog').shadowRoot.querySelector('or-input[id=add-btn]').click()"
-    )
+    _manager_ui_press_add(driver, url)
     print(
         "6. First we set the Base URI of the weather service that we will use for further queries. TODO"
     )
     if quit:
         # Need this for manager to act (maybe some confirmation TODO)
         time.sleep(1)
     else:
```

### Comparing `openremote-cli-0.6.8/openremote_cli/shell.py` & `openremote-cli-0.6.9/openremote_cli/shell.py`

 * *Files identical despite different names*

### Comparing `openremote-cli-0.6.8/pyproject.toml` & `openremote-cli-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openremote-cli"
-version = "0.6.8"
+version = "0.6.9"
 description = "OpenRemote Command-line interface"
 readme = "README.md"
 authors = ["Michal Rutka <michal@openremote.io>"]
 maintainers = ["OpenRemote <developers@openremote.io>"]
 license = "AGPLv3"
 repository = "https://github.com/openremote/openremote"
 homepage = "https://www.openremote.io"
```

### Comparing `openremote-cli-0.6.8/setup.py` & `openremote-cli-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'console_scripts': ['openremote-cli = openremote_cli.cli:main',
                      'or = openremote_cli.cli:main']}
 
 setup_kwargs = {
     'name': 'openremote-cli',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': 'OpenRemote Command-line interface',
     'long_description': "![CI/CD](https://github.com/openremote/openremote-cli/workflows/CI/CD/badge.svg)\n![docker](https://github.com/openremote/openremote-cli/workflows/docker/badge.svg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)\n[![Donate](https://img.shields.io/badge/donations-appreciated-green.svg)](https://www.paypal.com/webapps/shoppingcart?flowlogging_id=4b5432e8ad1a8&mfid=1616517920020_4b5432e8ad1a8#/checkout/openButton)\n\n# OpenRemote CLI\n\n## Intro\n\nThis is Command Line Interface to OpenRemote IoT platform. It's purpose is to reduce friction of using OpenRemote by Do It Yourself users.\n\nIt is published as a Python package on [PyPi.org](https://pypi.org/project/openremote-cli/)\n\n## About OR\n\nOpenRemote is a great real OpenSource IoT platform.\n\n## Usage\n\nTo install/upgrade the CLI:\n```bash\npip install --upgrade openremote-cli\nor --version\n```\n\n### Deploy local OpenRemote stack\n\n```bash\nor deploy\n```\n\nWhen it finishes you should be able to open https://localhost and login with admin:secret to the manager. Depending on your machine it can take few minutes to\nstart or services (usually less than 10 minutes). If it does not work yet, check it with ```docker ps``` to see if all services are in healthy or starting stage.\n\n### Remove local OpenRemote stack\n\n```bash\nor deploy --action remove\n```\n\n### Deploy OpenRemote stack on AWS with DNS entry\n\n```bash\nor deploy --platform aws --dnsname myiot.mydomain.com\n```\n### Check health of the openremote stack\n```bash\nor deploy -a health --dnsname myiot.mydomain.com -v\n```\n\n### Install shell completion extension\n\n#### zsh\n\n```bash\nTODO\n```\n\n#### bash\n\n```\nTODO\n```\n\n## Configure existing OpenRemote instance\n\n### Add users\n\n### Add assets\n\n### Add customization\n\n## Develop openremote-cli\n\nFollowing tools are used:\n- python (pip, poetry, black, PyPI.org)\n- git (pre-commit, actions)\n- docker (docker-compose, swarm)\n- AWS (CloudFormation)\n- make\n\n### Adding feature\n\nIn this project we use Behavior-driven development (or BDD). BDD is an agile\nsoftware development technique that encourages collaboration between developers,\nQA and non-technical or business participants in a software project.\n\nThis project uses Gherkin to define what features which should be covered. Features\nfiles can be generated by people on manager level or even higher. An example\nof file defining a feature:\n\n```gherkin\nFeature: deploy\n\n  Scenario: deploy to localhost\n    Given we have docker and docker-compose installed\n    When we call openremote-cli --dry-run deploy --action create\n    Then show what will be done\n```\n\nWhen the feature is implemented it can be checked with behave:\n\n```bash\n> behave\nFeature: deploy # features/deploy.feature:1\n\n  Scenario: deploy to localhost                                  # features/deploy.feature:3\n    Given we have docker and docker-compose installed            # features/steps/deploy_steps.py:8 0.453s\n    When we call openremote-cli --dry-run deploy --action create # features/steps/deploy_steps.py:16 0.591s\n    Then show what will be done                                  # features/steps/deploy_steps.py:24 0.000s\n\n1 feature passed, 0 failed, 0 skipped\n1 scenario passed, 0 failed, 0 skipped\n3 steps passed, 0 failed, 0 skipped, 0 undefined\nTook 0m1.044s\n```\n",
     'author': 'Michal Rutka',
     'author_email': 'michal@openremote.io',
     'maintainer': 'OpenRemote',
     'maintainer_email': 'developers@openremote.io',
     'url': 'https://www.openremote.io',
```

### Comparing `openremote-cli-0.6.8/PKG-INFO` & `openremote-cli-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openremote-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: OpenRemote Command-line interface
 Home-page: https://www.openremote.io
 License: AGPLv3
 Keywords: openremote,iot,cli
 Author: Michal Rutka
 Author-email: michal@openremote.io
 Maintainer: OpenRemote
```

