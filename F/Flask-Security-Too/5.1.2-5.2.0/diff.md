# Comparing `tmp/Flask-Security-Too-5.1.2.tar.gz` & `tmp/Flask-Security-Too-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Security-Too-5.1.2.tar", last modified: Mon Mar 13 15:21:20 2023, max compression
+gzip compressed data, was "Flask-Security-Too-5.2.0.tar", last modified: Sat May  6 00:15:13 2023, max compression
```

## Comparing `Flask-Security-Too-5.1.2.tar` & `Flask-Security-Too-5.2.0.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    66410 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.087645 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-03-13 15:21:20.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-03-13 15:21:20.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 15:21:20.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 15:21:15.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-13 15:21:20.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-13 15:21:20.000000 Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.091645 Flask-Security-Too-5.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.091645 Flask-Security-Too-5.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/_static/logo-owl-105.png
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/_static/logo-owl-68.png
--rw-r--r--   0 runner    (1001) docker     (123)    68319 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/_static/logo-owl-full-240.png
--rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/_static/logo-owl-full.png
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/_static/openapi_view.html
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    60264 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    83455 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/patterns.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/spa.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/two_factor_configurations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/docs/webauthn.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.095645 Flask-Security-Too-5.1.2/flask_security/
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/babel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/changeable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/confirmable.py
--rw-r--r--   0 runner    (1001) docker     (123)    78286 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    40261 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    22186 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/mail_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.095645 Flask-Security-Too-5.1.2/flask_security/models/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/models/fsqla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/models/fsqla_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/models/fsqla_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/oauth_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/password_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/phone_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/quart_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/recoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/registerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.071644 Flask-Security-Too-5.1.2/flask_security/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.095645 Flask-Security-Too-5.1.2/flask_security/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/static/js/base64.js
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/static/js/webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.071644 Flask-Security-Too-5.1.2/flask_security/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.099645 Flask-Security-Too-5.1.2/flask_security/templates/security/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/_macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/change_password.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/change_notice.html
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/change_notice.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/confirmation_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/confirmation_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/login_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/login_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/reset_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/reset_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/reset_notice.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/reset_notice.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/two_factor_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/two_factor_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/two_factor_rescue.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/two_factor_rescue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/us_instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/us_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome.html
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome.txt
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing.html
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing_username.html
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing_username.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/mf_recovery.html
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/mf_recovery_codes.html
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/send_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_verify_code.html
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/us_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/us_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/us_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/verify.html
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/wan_register.html
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/wan_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/templates/security/wan_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/tf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/totp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.071644 Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.071644 Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.071644 Flask-Security-Too-5.1.2/flask_security/translations/da_DK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/da_DK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36389 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32765 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31999 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/flask_security.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30981 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.075645 Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    36020 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/is_IS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/is_IS/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28576 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.103645 Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29444 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32194 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    28959 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.079645 Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/pwl.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.083645 Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44056 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.083645 Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.083645 Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-03-13 15:21:19.000000 Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/twofactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    37104 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/unified_signin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/username_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    42192 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45167 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/flask_security/webauthn_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.107645 Flask-Security-Too-5.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2354 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.111645 Flask-Security-Too-5.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.111645 Flask-Security-Too-5.1.2/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/_nav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/tests/templates/custom_security/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/change_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/mf_recovery.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/mf_recovery_codes.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/send_login.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/tf_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/tf_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/us_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/us_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/us_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/wan_register.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/wan_signin.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/custom_security/wan_verify.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.083645 Flask-Security-Too-5.1.2/tests/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/tests/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/security/email/confirmation_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/security/email/login_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/security/email/reset_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/security/email/us_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/templates/security/email/welcome.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_changeable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    36452 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21957 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_confirmable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    47794 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_oauthglue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_passwordless.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_recoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_registerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_tf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_trackable.py
--rw-r--r--   0 runner    (1001) docker     (123)    52984 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_two_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    77549 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_unified_signin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    63909 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/test_webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.087645 Flask-Security-Too-5.1.2/tests/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.087645 Flask-Security-Too-5.1.2/tests/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:21:20.115645 Flask-Security-Too-5.1.2/tests/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/translations/fr_FR/LC_MESSAGES/flask_security.mo
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/translations/fr_FR/LC_MESSAGES/flask_security.po
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tests/view_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-13 15:20:25.000000 Flask-Security-Too-5.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    67572 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.554405 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:15:08.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.562405 Flask-Security-Too-5.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.566405 Flask-Security-Too-5.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-105.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-68.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68319 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-full-240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/logo-owl-full.png
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/_static/openapi_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60607 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27459 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    83455 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/patterns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/spa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/two_factor_configurations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/docs/webauthn.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.578405 Flask-Security-Too-5.2.0/flask_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/babel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/changeable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77677 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40261 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/mail_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.582405 Flask-Security-Too-5.2.0/flask_security/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/models/fsqla_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/oauth_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/password_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/phone_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/quart_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/recoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/registerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.526405 Flask-Security-Too-5.2.0/flask_security/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.586405 Flask-Security-Too-5.2.0/flask_security/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/static/js/base64.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/static/js/webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.586405 Flask-Security-Too-5.2.0/flask_security/templates/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/change_password.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/change_notice.html
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/change_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/confirmation_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/confirmation_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/login_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/login_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_notice.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/reset_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_rescue.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/two_factor_rescue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.html
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.html
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery_codes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/send_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_verify_code.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/us_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/templates/security/wan_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/tf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/totp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.530405 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36389 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32765 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31999 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/flask_security.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30981 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.534405 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    36020 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.590405 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    28576 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29444 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.538405 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32194 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    28959 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/pwl.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44056 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.542405 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-06 00:15:13.000000 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/twofactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37104 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/unified_signin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/username_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41895 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45167 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/flask_security/webauthn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.594406 Flask-Security-Too-5.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-06 00:15:13.606406 Flask-Security-Too-5.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.598405 Flask-Security-Too-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/_nav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/custom_security/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/mf_recovery.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/mf_recovery_codes.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/send_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/tf_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/tf_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/us_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_register.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/custom_security/wan_verify.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/confirmation_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/login_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/reset_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/us_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/templates/security/email/welcome.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_changeable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35949 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21957 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19918 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48026 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_oauthglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_recoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_registerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_tf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_trackable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52643 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_two_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77284 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_unified_signin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63732 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/test_webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.546405 Flask-Security-Too-5.2.0/tests/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:15:13.602405 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/translations/fr_FR/LC_MESSAGES/flask_security.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tests/view_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-06 00:14:09.000000 Flask-Security-Too-5.2.0/tox.ini
```

### Comparing `Flask-Security-Too-5.1.2/.editorconfig` & `Flask-Security-Too-5.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/AUTHORS` & `Flask-Security-Too-5.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/CHANGES.rst` & `Flask-Security-Too-5.2.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 Flask-Security Changelog
 ========================
 
 Here you can see the full list of changes between each Flask-Security release.
 
+Version 5.2.0
+-------------
+
+Released May 6, 2023
+
+Note: Due to rapid deprecation and removal of APIs from the Pallets team,
+maintaining the testing of back versions of various packages is taking too
+much time and effort. In this release only current versions of the various
+dependent packages are being tested.
+
+Fixes
++++++
+
+- (:issue:`764`) Remove old Werkzeug compatibility check.
+- (:issue:`777`) Compatibility with Quart.
+- (:pr:`780`) Remove dependence on pkg_resources / setuptools (use importlib_resources package)
+- (:pr:`792`) Fix tests to work with latest Werkzeug/Flask. Update requirements_low to match current releases.
+- (:pr:`792`) Drop support for Python 3.7
+
+Known Issues
+++++++++++++
+
+- Flask-mongoengine hasn't released in a while and currently will not work with latest Flask and Flask-Security-Too
+  (this is due to the JSONEncoder being deprecated and removed).
+
+Backwards Compatibility Concerns
++++++++++++++++++++++++++++++++++
+- The removal of pkg_resources required changing the config variable :py:data:`SECURITY_I18N_DIRNAME`.
+  If your application modified or extended this configuration variable, a small change will be required.
+
 Version 5.1.2
 -------------
 
 Released March 12, 2023
 
 Fixes
 +++++
```

### Comparing `Flask-Security-Too-5.1.2/CONTRIBUTING.rst` & `Flask-Security-Too-5.2.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     file:///usr/local/lib/node_modules/swagger-editor-dist/index.html#
 
 
 Edit - it is a WYSIWYG editor and will show you errors. Once you save (as yaml) you
 need to look at what it will render as::
 
-    $ python setup.py build_sphinx
+    $ sphinx-build docs docs/_build/html
     $ http-server -p 8081
 
 Then in your browser navigate to::
 
     http://localhost:8081/docs/_build/html/index.html
     or
     http://localhost:8081/docs/_build/html/_static/openapi_view.html
```

### Comparing `Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/PKG-INFO` & `Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Security-Too
-Version: 5.1.2
+Version: 5.2.0
 Summary: Simple security for Flask apps.
 Home-page: https://github.com/Flask-Middleware/flask-security
 Author: Matt Wright & Chris Wagner
 Author-email: jwag.wagner+github@gmail.com
 License: MIT
 Project-URL: Documentation, https://flask-security-too.readthedocs.io
 Project-URL: Releases, https://pypi.org/project/Flask-Security-Too/
@@ -17,23 +17,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: babel
 Provides-Extra: fsqla
 Provides-Extra: common
 Provides-Extra: mfa
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `Flask-Security-Too-5.1.2/Flask_Security_Too.egg-info/SOURCES.txt` & `Flask-Security-Too-5.2.0/Flask_Security_Too.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/LICENSE` & `Flask-Security-Too-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/MANIFEST.in` & `Flask-Security-Too-5.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/PKG-INFO` & `Flask-Security-Too-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Security-Too
-Version: 5.1.2
+Version: 5.2.0
 Summary: Simple security for Flask apps.
 Home-page: https://github.com/Flask-Middleware/flask-security
 Author: Matt Wright & Chris Wagner
 Author-email: jwag.wagner+github@gmail.com
 License: MIT
 Project-URL: Documentation, https://flask-security-too.readthedocs.io
 Project-URL: Releases, https://pypi.org/project/Flask-Security-Too/
@@ -17,23 +17,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: babel
 Provides-Extra: fsqla
 Provides-Extra: common
 Provides-Extra: mfa
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `Flask-Security-Too-5.1.2/README.rst` & `Flask-Security-Too-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/Makefile` & `Flask-Security-Too-5.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/_static/logo-owl-105.png` & `Flask-Security-Too-5.2.0/docs/_static/logo-owl-105.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/_static/logo-owl-68.png` & `Flask-Security-Too-5.2.0/docs/_static/logo-owl-68.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/_static/logo-owl-full-240.png` & `Flask-Security-Too-5.2.0/docs/_static/logo-owl-full-240.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/_static/logo-owl-full.png` & `Flask-Security-Too-5.2.0/docs/_static/logo-owl-full.png`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/_static/openapi_view.html` & `Flask-Security-Too-5.2.0/docs/_static/openapi_view.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/api.rst` & `Flask-Security-Too-5.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/conf.py` & `Flask-Security-Too-5.2.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 author = "Matt Wright & Chris Wagner"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "5.1.2"
+version = "5.2.0"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `Flask-Security-Too-5.1.2/docs/configuration.rst` & `Flask-Security-Too-5.2.0/docs/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     This is actually part of Flask - but is used by Flask-Security to sign all tokens.
     It is critical this is set to a strong value. For python3 consider using: ``secrets.token_urlsafe()``
 
 .. py:data:: SECURITY_BLUEPRINT_NAME
 
     Specifies the name for the Flask-Security blueprint.
 
-    Default: ``security``.
+    Default: ``"security"``.
 
 .. py:data:: SECURITY_URL_PREFIX
 
     Specifies the URL prefix for the Flask-Security blueprint.
 
     Default: ``None``.
 
@@ -53,30 +53,35 @@
     Specifies whether or not to flash messages during security procedures.
 
     Default: ``True``.
 .. py:data:: SECURITY_I18N_DOMAIN
 
     Specifies the name for domain used for translations.
 
-    Default: ``flask_security``.
+    Default: ``"flask_security"``.
 .. py:data:: SECURITY_I18N_DIRNAME
 
     Specifies the directory containing the ``MO`` files used for translations.
     When using flask-babel this can also be a list of directory names - this
-    enables application to override a subset of messages if desired.
+    enables application to override a subset of messages if desired. The
+    default ``builtin`` uses translations shipped with Flask-Security.
 
-    Default: ``[PATH_LIB]/flask_security/translations``.
+    Default: ``"builtin"``.
+
+    .. versionchanged:: 5.2.0
+        "builtin" is a special name which will be interpreted as the ``translations``
+        directory within the installation of Flask-Security.
 
 .. py:data:: SECURITY_PASSWORD_HASH
 
     Specifies the password hash algorithm to use when hashing passwords.
     Recommended values for production systems are ``bcrypt``, ``argon2``, ``sha512_crypt``, or
     ``pbkdf2_sha512``. Some algorithms require the installation  of a backend package (e.g. `bcrypt`_, `argon2`_).
 
-    Default:``bcrypt``.
+    Default: ``"bcrypt"``.
 
 .. py:data:: SECURITY_PASSWORD_SCHEMES
 
     List of support password hash algorithms. ``SECURITY_PASSWORD_HASH``
     must be from this list. Passwords encrypted with any of these schemes will be honored.
 
 .. py:data:: SECURITY_DEPRECATED_PASSWORD_SCHEMES
@@ -104,20 +109,20 @@
     Default: a list of known schemes not working with double hashing (`django_{digest}`, `plaintext`).
 
 .. py:data:: SECURITY_HASHING_SCHEMES
 
     List of algorithms used for encrypting/hashing sensitive data within a token
     (Such as is sent with confirmation or reset password).
 
-    Default: ``sha256_crypt``.
+    Default: ``["sha256_crypt", "hex_md5"]``.
 .. py:data:: SECURITY_DEPRECATED_HASHING_SCHEMES
 
     List of deprecated algorithms used for creating and validating tokens.
 
-    Default: ``hex_md5``.
+    Default: ``["hex_md5"]``.
 
 .. py:data:: SECURITY_PASSWORD_HASH_OPTIONS
 
     Specifies additional options to be passed to the hashing method. This is deprecated as of passlib 1.7.
 
     .. deprecated:: 3.4.0 see: :py:data:`SECURITY_PASSWORD_HASH_PASSLIB_OPTIONS`
 
@@ -129,15 +134,15 @@
 
     .. versionadded:: 3.3.1
 
 .. py:data:: SECURITY_PASSWORD_LENGTH_MIN
 
     Minimum required length for passwords.
 
-    Default: 8
+    Default: ``8``
 
     .. versionadded:: 3.4.0
 .. py:data:: SECURITY_PASSWORD_COMPLEXITY_CHECKER
 
     Set to complexity checker to use (Only ``zxcvbn`` supported).
 
     Default: ``None``
@@ -173,15 +178,15 @@
 
 .. py:data:: SECURITY_PASSWORD_NORMALIZE_FORM
 
     Passwords are normalized prior to changing or comparing. This satisfies
     the NIST requirement: `5.1.1.2 Memorized Secret Verifiers`_.
     Normalization is performed using the Python unicodedata.normalize() method.
 
-    Default: "NFKD"
+    Default: ``"NFKD"``
 
     .. versionadded:: 4.0.0
 
 .. _5.1.1.2 Memorized Secret Verifiers: https://pages.nist.gov/800-63-3/sp800-63b.html#sec5
 
 .. py:data:: SECURITY_PASSWORD_REQUIRED
 
@@ -195,21 +200,21 @@
 
     .. versionadded:: 5.0.0
 
 .. py:data:: SECURITY_TOKEN_AUTHENTICATION_KEY
 
     Specifies the query string parameter to read when using token authentication.
 
-    Default: ``auth_token``.
+    Default: ``"auth_token"``.
 
 .. py:data:: SECURITY_TOKEN_AUTHENTICATION_HEADER
 
     Specifies the HTTP header to read when using token authentication.
 
-    Default: ``Authentication-Token``.
+    Default: ``"Authentication-Token"``.
 
 .. py:data:: SECURITY_TOKEN_MAX_AGE
 
     Specifies the number of seconds before an authentication token expires.
 
     Default: ``None``, meaning the token never expires.
 
@@ -346,15 +351,15 @@
         variable ``SECURITY_CSRF_COOKIE_NAME``.
 
 .. py:data:: SECURITY_CSRF_HEADER
 
     The HTTP Header name that will contain the CSRF token. ``X-XSRF-Token``
     is used by packages such as `axios`_.
 
-    Default: ``X-XSRF-Token``.
+    Default: ``"X-XSRF-Token"``.
 
 .. py:data:: SECURITY_CSRF_COOKIE_REFRESH_EACH_REQUEST
 
     By default, csrf_tokens have an expiration (controlled
     by the configuration variable ``WTF_CSRF_TIME_LIMIT``.
     This can cause CSRF failures if say an application is left
     idle for a long time. You can set that time limit to ``None``
@@ -529,15 +534,15 @@
 
 .. py:data:: SECURITY_PHONE_REGION_DEFAULT
 
     Assigns a default 'region' for phone numbers used for two-factor or
     unified sign in. All other phone numbers will require a region prefix to
     be accepted.
 
-    Default: ``US``
+    Default: ``"US"``
 
     .. versionadded:: 3.4.0
 
 .. py:data:: SECURITY_FRESHNESS
 
     A timedelta used to protect endpoints that alter sensitive information.
     This is used to protect the following endpoints:
@@ -640,21 +645,21 @@
 
     Default: ``True``.
 
 .. py:data:: SECURITY_CLI_USERS_NAME
 
     Specifies the name for the command managing users. Disable by setting ``False``.
 
-    Default: ``users``.
+    Default: ``"users"``.
 
 .. py:data:: SECURITY_CLI_ROLES_NAME
 
     Specifies the name for the command managing roles. Disable by setting ``False``.
 
-    Default: ``roles``.
+    Default: ``"roles"``.
 
 .. py:data:: SECURITY_JOIN_USER_ROLES
 
     Specifies whether to set the ``UserModel.roles`` loading relationship to ``joined`` when a ``roles`` attribute
     is present for a SQLAlchemy Datastore. Setting this to ``False`` restores pre 3.3.0 behavior and is required if the ``roles`` attribute
     is not a joinable attribute on the ``UserModel``. The default setting improves performance by only requiring a single
     DB call.
@@ -765,20 +770,20 @@
     Specifies whether registration email is sent.
 
     Default: ``True``.
 .. py:data:: SECURITY_EMAIL_SUBJECT_REGISTER
 
     Sets the subject for the confirmation email.
 
-    Default: ``"Welcome"``.
+    Default: ``_("Welcome")``.
 .. py:data:: SECURITY_REGISTER_USER_TEMPLATE
 
     Specifies the path to the template for the user registration page.
 
-    Default: ``security/register_user.html``.
+    Default: ``"security/register_user.html"``.
 .. py:data:: SECURITY_POST_REGISTER_VIEW
 
     Specifies the view to redirect to after a user successfully registers.
     This value can be set to a URL or an endpoint name. If this value is
     ``None``, the user is redirected to the value of ``SECURITY_POST_LOGIN_VIEW``.
     Note that if the request URL or form has a ``next`` parameter, that will take precedence.
 
@@ -853,30 +858,30 @@
 
     Default: ``False``.
 .. py:data:: SECURITY_CONFIRM_EMAIL_WITHIN
 
     Specifies the amount of time a user has before their confirmation
     link expires. Always pluralize the time unit for this value.
 
-    Default: ``5 days``.
+    Default: ``"5 days"``.
 .. py:data:: SECURITY_CONFIRM_URL
 
     Specifies the email confirmation URL.
 
     Default: ``"/confirm"``.
 .. py:data:: SECURITY_SEND_CONFIRMATION_TEMPLATE
 
     Specifies the path to the template for the resend confirmation instructions page.
 
-    Default: ``security/send_confirmation.html``.
+    Default: ``"security/send_confirmation.html"``.
 .. py:data:: SECURITY_EMAIL_SUBJECT_CONFIRM
 
     Sets the subject for the email confirmation message.
 
-    Default: ``Please confirm your email``.
+    Default: ``_("Please confirm your email")``.
 .. py:data:: SECURITY_CONFIRM_ERROR_VIEW
 
     Specifies the view to redirect to if a confirmation error occurs.
     This value can be set to a URL or an endpoint name.
     If this value is ``None``, the user is presented the default view
     to resend a confirmation link. In the case of ``SECURITY_REDIRECT_BEHAVIOR`` == ``spa``
     query params in the redirect will contain the error.
@@ -934,27 +939,27 @@
     value of ``SECURITY_POST_LOGIN_VIEW``.
 
     Default: ``None``.
 .. py:data:: SECURITY_CHANGE_PASSWORD_TEMPLATE
 
     Specifies the path to the template for the change password page.
 
-    Default: ``security/change_password.html``.
+    Default: ``"security/change_password.html"``.
 
 .. py:data:: SECURITY_SEND_PASSWORD_CHANGE_EMAIL
 
     Specifies whether password change email is sent.
 
     Default: ``True``.
 
 .. py:data:: SECURITY_EMAIL_SUBJECT_PASSWORD_CHANGE_NOTICE
 
     Sets the subject for the password change notice.
 
-    Default: ``Your password has been changed``.
+    Default: ``_("Your password has been changed")``.
 
 Recoverable
 -----------
 
 .. py:data:: SECURITY_RECOVERABLE
 
     Specifies if Flask-Security should create a password reset/recover endpoint.
@@ -967,21 +972,21 @@
 
     Default: ``"/reset"``.
 
 .. py:data:: SECURITY_RESET_PASSWORD_TEMPLATE
 
     Specifies the path to the template for the reset password page.
 
-    Default: ``security/reset_password.html``.
+    Default: ``"security/reset_password.html"``.
 
 .. py:data:: SECURITY_FORGOT_PASSWORD_TEMPLATE
 
     Specifies the path to the template for the forgot password page.
 
-    Default: ``security/forgot_password.html``.
+    Default: ``"security/forgot_password.html"``.
 
 .. py:data:: SECURITY_POST_RESET_VIEW
 
     Specifies the view to redirect to after a user successfully resets their password.
     This value can be set to a URL or an endpoint name. If this
     value is ``None``, the user is redirected  to the value of ``SECURITY_POST_LOGIN_VIEW``.
 
@@ -1004,15 +1009,15 @@
     Default: ``None``.
 
 .. py:data:: SECURITY_RESET_PASSWORD_WITHIN
 
     Specifies the amount of time a user has before their password reset link expires.
     Always pluralize the time unit for this value.
 
-    Default: ``5 days``.
+    Default: ``"5 days"``.
 
 .. py:data:: SECURITY_SEND_PASSWORD_RESET_EMAIL
 
     Specifies whether password reset email is sent. These are instructions
     including a link that can be clicked on.
 
     Default: ``True``.
@@ -1024,21 +1029,21 @@
 
     Default: ``True``.
 
 .. py:data:: SECURITY_EMAIL_SUBJECT_PASSWORD_RESET
 
     Sets the subject for the password reset email.
 
-    Default: ``Password reset instructions``.
+    Default: ``_("Password reset instructions")``.
 
 .. py:data:: SECURITY_EMAIL_SUBJECT_PASSWORD_NOTICE
 
     Sets subject for the password notice.
 
-    Default: ``Your password has been reset``.
+    Default: ``_("Your password has been reset")``.
 
 Two-Factor
 -----------
 Configuration related to the two-factor authentication feature.
 
 .. versionadded:: 3.2.0
 
@@ -1093,36 +1098,36 @@
 
     Default: ``120``.
 .. py:data:: SECURITY_TWO_FACTOR_RESCUE_MAIL
 
     Specifies the email address users send mail to when they can't complete the
     two-factor authentication login.
 
-    Default: ``no-reply@localhost``.
+    Default: ``"no-reply@localhost"``.
 
 .. py:data:: SECURITY_EMAIL_SUBJECT_TWO_FACTOR
 
     Sets the subject for the two factor feature.
 
-    Default: ``Two-factor Login``
+    Default: ``_("Two-factor Login")``
 .. py:data:: SECURITY_EMAIL_SUBJECT_TWO_FACTOR_RESCUE
 
     Sets the subject for the two factor help function.
 
-    Default: ``Two-factor Rescue``
+    Default: ``_("Two-factor Rescue")``
 .. py:data:: SECURITY_TWO_FACTOR_VERIFY_CODE_TEMPLATE
 
     Specifies the path to the template for the verify code page for the two-factor authentication process.
 
-    Default: ``security/two_factor_verify_code.html``.
+    Default: ``"security/two_factor_verify_code.html"``.
 .. py:data:: SECURITY_TWO_FACTOR_SETUP_TEMPLATE
 
     Specifies the path to the template for the setup page for the two factor authentication process.
 
-    Default: ``security/two_factor_setup.html``.
+    Default: ``"security/two_factor_setup.html"``.
 
 .. py:data:: SECURITY_TWO_FACTOR_SETUP_URL
 
     Specifies the two factor setup URL.
 
     Default: ``"/tf-setup"``.
 .. py:data:: SECURITY_TWO_FACTOR_TOKEN_VALIDATION_URL
@@ -1167,15 +1172,15 @@
     .. versionadded:: 5.1.0
 
 .. py:data:: SECURITY_TWO_FACTOR_SELECT_TEMPLATE
 
     Specifies the path to the template for the select method page for the two-factor authentication process.
     This is used when more than one two-factor method has been setup (e.g. SMS and Webauthn).
 
-    Default: ``security/two_factor_select.html``.
+    Default: ``"security/two_factor_select.html"``.
 
     .. versionadded:: 5.0.0
 
 .. py:data:: SECURITY_TWO_FACTOR_ALWAYS_VALIDATE
 
     Specifies whether the application should require a two factor code upon every login.
     If set to ``False`` then the 2 values below are used to determine when
@@ -1183,15 +1188,15 @@
     session will always require a fresh two-factor code.
 
     Default: ``True``.
 .. py:data:: SECURITY_TWO_FACTOR_LOGIN_VALIDITY
 
     Specifies the expiration of the two factor validity cookie and verification of the token.
 
-    Default: ``30 Days``.
+    Default: ``"30 Days"``.
 
 
 .. py:data:: SECURITY_TWO_FACTOR_VALIDITY_COOKIE
 
     A dictionary containing the parameters of the two factor validity cookie.
     The complete set of parameters is described in Flask's `set_cookie`_ documentation.
 
@@ -1328,15 +1333,15 @@
     Default: ``_("Verification Code")``
 
 .. py:data:: SECURITY_US_SETUP_WITHIN
 
     Specifies the amount of time a user has before their setup
     token expires. Always pluralize the time unit for this value.
 
-    Default: "30 minutes"
+    Default: ``"30 minutes"``
 
 .. py:data:: SECURITY_US_SIGNIN_REPLACES_LOGIN
 
     If set, then the :py:data:`SECURITY_LOGIN_URL` will be registered to the ``us-signin`` endpoint.
     Doing this will mean that logout will properly redirect to the us-signin endpoint.
 
     Default: ``False``
@@ -1374,28 +1379,28 @@
     Default: ``False``.
 
 .. py:data:: SECURITY_SEND_LOGIN_TEMPLATE
 
     Specifies the path to the template for the send login instructions page for
     passwordless logins.
 
-    Default:``security/send_login.html``.
+    Default:``"security/send_login.html"``.
 
 .. py:data:: SECURITY_EMAIL_SUBJECT_PASSWORDLESS
 
     Sets the subject for the passwordless feature.
 
-    Default: ``Login instructions``.
+    Default: ``_("Login instructions")``.
 
 .. py:data:: SECURITY_LOGIN_WITHIN
 
     Specifies the amount of time a user has before a login link expires.
     Always pluralize the time unit for this value.
 
-    Default: ``1 days``.
+    Default: ``"1 days"``.
 
 .. py:data:: SECURITY_LOGIN_ERROR_VIEW
 
     Specifies the view/URL to redirect to after the following login/authentication errors:
 
     * GET passwordless link where the link is expired/incorrect
     * GET unified sign in magic link when there is an error.
@@ -1545,15 +1550,15 @@
 
         - ``"first"`` - just keys registered as "first" usage are allowed
         - ``"secondary"`` - just keys registered as "secondary" are allowed
 
     If list is empty or ``None`` WebAuthn keys aren't allowed. This also means that the
             :py:data:``SECURITY_WAN_VERIFY`` endpoint won't be registered.
 
-    Default:: ``["first", "secondary"]``
+    Default: ``["first", "secondary"]``
 
 
 Additional relevant configuration variables:
 
     * :py:data:`SECURITY_FRESHNESS` - Used to protect /us-setup.
     * :py:data:`SECURITY_FRESHNESS_GRACE_PERIOD` - Used to protect /us-setup.
 
@@ -1773,15 +1778,15 @@
 * ``SECURITY_MSG_INVALID_PASSWORD_CODE``
 * ``SECURITY_MSG_INVALID_RECOVERY_CODE``
 * ``SECURITY_MSG_INVALID_REDIRECT``
 * ``SECURITY_MSG_INVALID_RESET_PASSWORD_TOKEN``
 * ``SECURITY_MSG_LOGIN``
 * ``SECURITY_MSG_LOGIN_EMAIL_SENT``
 * ``SECURITY_MSG_LOGIN_EXPIRED``
-* ``SECURITY_NO_RECOVERY_CODES_SETUP``
+* ``SECURITY_MSG_NO_RECOVERY_CODES_SETUP``
 * ``SECURITY_MSG_OAUTH_HANDSHAKE_ERROR``
 * ``SECURITY_MSG_PASSWORDLESS_LOGIN_SUCCESSFUL``
 * ``SECURITY_MSG_PASSWORD_BREACHED``
 * ``SECURITY_MSG_PASSWORD_BREACHED_SITE_ERROR``
 * ``SECURITY_MSG_PASSWORD_CHANGE``
 * ``SECURITY_MSG_PASSWORD_INVALID_LENGTH``
 * ``SECURITY_MSG_PASSWORD_IS_THE_SAME``
```

### Comparing `Flask-Security-Too-5.1.2/docs/customizing.rst` & `Flask-Security-Too-5.2.0/docs/customizing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 ++++++++++++++++++++
 
 It is possible to change one or more messages (either the original default english
 and/or a specific translation). Adding the following to your app::
 
     app.config["SECURITY_MSG_INVALID_PASSWORD"] = ("Password no-worky", "error")
 
-Will change the default message in english.
+will change the default message in english.
 
 .. tip::
     The string messages themselves are a 'key' into the translation .po/.mo files.
     Do not pass in gettext('string') or lazy_gettext('string).
 
 If you need translations then you
 need to create your own ``translations`` directory and add the appropriate .po files
@@ -340,15 +340,15 @@
 
 Then compile it with::
 
     pybabel compile -d translations/ -i translations/fr_FR/LC_MESSAGES/flask_security.po -l fr_FR -D flask_security
 
 Finally add your translations directory to your configuration::
 
-    app.config["SECURITY_I18N_DIRNAME"] = [pkg_resources.resource_filename("flask_security", "translations"), "translations"]
+    app.config["SECURITY_I18N_DIRNAME"] = ["builtin", "translations"]
 
 .. note::
     This only works when using Flask-Babel since Flask-BabelEx doesn't support a list of translation directories.
 
 .. _emails_topic:
 
 Emails
```

### Comparing `Flask-Security-Too-5.1.2/docs/features.rst` & `Flask-Security-Too-5.2.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/index.rst` & `Flask-Security-Too-5.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/installation.rst` & `Flask-Security-Too-5.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/models.rst` & `Flask-Security-Too-5.2.0/docs/models.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/openapi.yaml` & `Flask-Security-Too-5.2.0/docs/openapi.yaml`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/patterns.rst` & `Flask-Security-Too-5.2.0/docs/patterns.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/quickstart.rst` & `Flask-Security-Too-5.2.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/spa.rst` & `Flask-Security-Too-5.2.0/docs/spa.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/docs/two_factor_configurations.rst` & `Flask-Security-Too-5.2.0/docs/two_factor_configurations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,18 @@
 the desired 2FA method, and finally have the user enter the code and POST to ``/tf-validate``.
 
 Rescue
 ~~~~~~
 Life happens - if the user doesn't have their mobile devices (SMS) or authenticator app, then they can use the ``/tf-rescue`` endpoint to
 see possible recovery options. Flask-Security supports the following:
 
-    - Have a one-time code sent to their email.
+    - Have a one-time code sent to their email (if :py:data:`SECURITY_TWO_FACTOR_RESCUE_EMAIL` is set to ``True``).
     - Send an email to the application administrators.
     - Use a previously setup one-time recovery code (see :py:data:`SECURITY_MULTI_FACTOR_RECOVERY_CODES`)
 
 Validity
 ++++++++
 Sometimes it can be preferable to enter the 2FA code once a day/week/month, especially if a user logs in and out of a website multiple times.  This allows the
-security of a two factor authentication but with a slightly better user experience.  This can be achieved by setting ``SECURITY_TWO_FACTOR_ALWAYS_VALIDATE`` to ``False``,
+security of a two factor authentication but with a slightly better user experience.  This can be achieved by setting :py:data:`SECURITY_TWO_FACTOR_ALWAYS_VALIDATE` to ``False``,
 and clicking the 'Remember' button on the login form. Once the two factor code is validated, a cookie is set to allow skipping the validation step.  The cookie is named
 ``tf_validity`` and contains the signed token containing the user's ``fs_uniquifier``.  The cookie and token are both set to expire after the time delta given in
-``SECURITY_TWO_FACTOR_LOGIN_VALIDITY``.  Note that setting ``SECURITY_TWO_FACTOR_LOGIN_VALIDITY`` to 0 is equivalent to ``SECURITY_TWO_FACTOR_ALWAYS_VALIDATE`` being ``True``.
+:py:data:`SECURITY_TWO_FACTOR_LOGIN_VALIDITY`.  Note that setting ``SECURITY_TWO_FACTOR_LOGIN_VALIDITY`` to 0 is equivalent to ``SECURITY_TWO_FACTOR_ALWAYS_VALIDATE`` being ``True``.
```

### Comparing `Flask-Security-Too-5.1.2/docs/webauthn.rst` & `Flask-Security-Too-5.2.0/docs/webauthn.rst`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/__init__.py` & `Flask-Security-Too-5.2.0/flask_security/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
     WebAuthnSigninForm,
     WebAuthnSigninResponseForm,
     WebAuthnDeleteForm,
     WebAuthnVerifyForm,
 )
 from .webauthn_util import WebauthnUtil
 
-__version__ = "5.1.2"
+__version__ = "5.2.0"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/changeable.py` & `Flask-Security-Too-5.2.0/flask_security/changeable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/cli.py` & `Flask-Security-Too-5.2.0/flask_security/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/confirmable.py` & `Flask-Security-Too-5.2.0/flask_security/confirmable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/core.py` & `Flask-Security-Too-5.2.0/flask_security/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from datetime import datetime, timedelta
 from dataclasses import dataclass
 import importlib
 import re
 import typing as t
 import warnings
 
-import pkg_resources
 from flask import current_app, g
 from flask_login import AnonymousUserMixin, LoginManager
 from flask_login import UserMixin as BaseUserMixin
 from flask_login import current_user
 from flask_principal import Identity, Principal, RoleNeed, UserNeed, identity_loaded
 from itsdangerous import URLSafeTimedSerializer
 from passlib.context import CryptContext
@@ -126,15 +125,15 @@
     "URL_PREFIX": None,
     "STATIC_FOLDER": "static",
     "STATIC_FOLDER_URL": "/fs-static",
     "SUBDOMAIN": None,
     "FLASH_MESSAGES": True,
     "RETURN_GENERIC_RESPONSES": False,
     "I18N_DOMAIN": "flask_security",
-    "I18N_DIRNAME": pkg_resources.resource_filename("flask_security", "translations"),
+    "I18N_DIRNAME": "builtin",
     "EMAIL_VALIDATOR_ARGS": None,
     "PASSWORD_HASH": "bcrypt",
     "PASSWORD_SALT": None,
     "PASSWORD_SINGLE_HASH": {
         "django_argon2",
         "django_bcrypt_sha256",
         "django_pbkdf2_sha256",
@@ -645,27 +644,15 @@
 def _request_loader(request):
     # Short-circuit if we have already been called and verified.
     # This can happen since Flask-Login will call us (if no session) and our own
     # decorator @auth_token_required can call us.
     # N.B. we don't call current_user here since that in fact might try and LOAD
     # a user - which would call us again.
     if get_request_attr("fs_authn_via") == "token":
-        # Flask-Login 0.6.2 and post Flask 2.2
-        if hasattr(g, "_login_user"):
-            return g._login_user
-        else:  # pragma: no cover
-            # pre flask_login 0.6.2 and handle that flask 2.3 is deprecating
-            # _request_ctx_stack
-            try:
-                from flask import _request_ctx_stack
-
-                if hasattr(_request_ctx_stack.top, "user"):
-                    return _request_ctx_stack.top.user
-            except ImportError:
-                pass
+        return g._login_user
 
     header_key = _security.token_authentication_header
     args_key = _security.token_authentication_key
     header_token = request.headers.get(header_key, None)
     token = request.args.get(args_key, header_token)
     if request.is_json:
         data = request.get_json(silent=True) or {}
@@ -1400,16 +1387,15 @@
         ]
         for attr in attr_names:
             if kwargs.get(attr, None):
                 setattr(self, attr, kwargs.get(attr))
 
         # set all (SECURITY) config items as attributes (minus the SECURITY_ prefix)
         for key, value in get_config(app).items():
-            # need to start getting rid of this - especially things like *_URL which
-            # should never be referenced
+            # need to start getting rid of this - very confusing.
             if not key.endswith("_URL"):
                 setattr(self, key.lower(), value)
 
         identity_loaded.connect_via(app)(_on_identity_loaded)
 
         if hasattr(self.datastore, "user_model") and not hasattr(
             self.datastore.user_model, "fs_uniquifier"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/datastore.py` & `Flask-Security-Too-5.2.0/flask_security/datastore.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/decorators.py` & `Flask-Security-Too-5.2.0/flask_security/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,25 +137,15 @@
             redirect_to = request.referrer
 
         return redirect(view or redirect_to)
     abort(403)
 
 
 def _check_token():
-    # N.B. this isn't great Flask-Login 0.5.0 made this protected
-    # Issue https://github.com/maxcountryman/flask-login/issues/471
-    # was filed to restore public access. We want to call this via
-    # login_manager in case someone has overridden the login_manager which we
-    # allow.
-    if hasattr(_security.login_manager, "request_callback"):
-        # Pre 0.5.0
-        user = _security.login_manager.request_callback(request)
-    else:
-        user = _security.login_manager._request_callback(request)
-
+    user = _security.login_manager.request_callback(request)
     if user and user.is_authenticated:
         app = current_app._get_current_object()
         identity_changed.send(app, identity=Identity(user.fs_uniquifier))
         return True
 
     return False
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/forms.py` & `Flask-Security-Too-5.2.0/flask_security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/json.py` & `Flask-Security-Too-5.2.0/flask_security/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,14 @@
     Flask-Security JSON extensions.
 
     :copyright: (c) 2022-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
     Pieces of this code liberally copied from flask-mongoengine.
 """
-from flask import __version__ as flask_version
-from pkg_resources import parse_version
-
-
-def use_json_provider() -> bool:
-    """Split Flask before 2.2.0 and after, to use/not use JSON provider approach."""
-    return parse_version(flask_version) >= parse_version("2.2.0")
 
 
 def _use_encoder(superclass):  # pragma: no cover
     """Flask < 2.2"""
 
     class FsJsonEncoder(superclass):
         """Flask-Security JSON encoder.
@@ -47,23 +40,23 @@
             return super(FSJsonProvider, FSJsonProvider).default(obj)
 
     return FSJsonProvider
 
 
 def setup_json(app, bp=None):
     # Called at init_app time.
-    if use_json_provider():
+    if hasattr(app, "json_provider_class"):
+        # Flask >= 2.2
         app.json_provider_class = _use_provider(app.json_provider_class)
         app.json = app.json_provider_class(app)
         # a bit if a hack - if a package (e.g. flask-mongoengine) hasn't
         # converted yet - they might use json_encoder. This ONLY applies
         # to this specific version of Flask that happens to use _json_encoder to
         # signal if any app/extension has registered an old style encoder.
         # (app.json_encoder is always set)
         # (If they do, then Flask 2.2.x won't use json_provider at all)
         # Of course if they do this AFTER we're initialized all bets are off.
-        if parse_version(flask_version) >= parse_version("2.2.0"):
-            if getattr(app, "_json_encoder", None):
-                app.json_encoder = _use_encoder(app.json_encoder)
+        if getattr(app, "_json_encoder", None):
+            app.json_encoder = _use_encoder(app.json_encoder)
 
     elif bp:  # pragma: no cover
         bp.json_encoder = _use_encoder(app.json_encoder)
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/mail_util.py` & `Flask-Security-Too-5.2.0/flask_security/mail_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/models/fsqla.py` & `Flask-Security-Too-5.2.0/flask_security/models/fsqla.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/models/fsqla_v2.py` & `Flask-Security-Too-5.2.0/flask_security/models/fsqla_v2.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/models/fsqla_v3.py` & `Flask-Security-Too-5.2.0/flask_security/models/fsqla_v3.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/oauth_glue.py` & `Flask-Security-Too-5.2.0/flask_security/oauth_glue.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/password_util.py` & `Flask-Security-Too-5.2.0/flask_security/password_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/passwordless.py` & `Flask-Security-Too-5.2.0/flask_security/passwordless.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/phone_util.py` & `Flask-Security-Too-5.2.0/flask_security/phone_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/proxies.py` & `Flask-Security-Too-5.2.0/flask_security/proxies.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/quart_compat.py` & `Flask-Security-Too-5.2.0/flask_security/quart_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/recoverable.py` & `Flask-Security-Too-5.2.0/flask_security/recoverable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/recovery_codes.py` & `Flask-Security-Too-5.2.0/flask_security/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/registerable.py` & `Flask-Security-Too-5.2.0/flask_security/registerable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/signals.py` & `Flask-Security-Too-5.2.0/flask_security/signals.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/static/js/base64.js` & `Flask-Security-Too-5.2.0/flask_security/static/js/base64.js`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/static/js/webauthn.js` & `Flask-Security-Too-5.2.0/flask_security/static/js/webauthn.js`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/_macros.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/_macros.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/_menu.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/base.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/base.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/change_password.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/change_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/us_instructions.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/us_instructions.txt` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/us_instructions.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome.txt` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing.txt` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing_username.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/email/welcome_existing_username.txt` & `Flask-Security-Too-5.2.0/flask_security/templates/security/email/welcome_existing_username.txt`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/forgot_password.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/forgot_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/login_user.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/login_user.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/mf_recovery_codes.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/mf_recovery_codes.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/register_user.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/register_user.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/reset_password.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/reset_password.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/send_confirmation.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/send_login.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/send_login.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_select.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_select.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_setup.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_setup.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/two_factor_verify_code.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/two_factor_verify_code.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/us_setup.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/us_setup.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/us_signin.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/us_signin.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/us_verify.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/us_verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/verify.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/wan_register.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_register.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/wan_signin.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_signin.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/templates/security/wan_verify.html` & `Flask-Security-Too-5.2.0/flask_security/templates/security/wan_verify.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/tf_plugin.py` & `Flask-Security-Too-5.2.0/flask_security/tf_plugin.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/totp.py` & `Flask-Security-Too-5.2.0/flask_security/totp.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security-Too 4.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Michael Bosch <michael@lonelyviking.com>\n"
 "Language: af_ZA\n"
 "Language-Team: af_ZA <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/af_ZA/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,435 +4,435 @@
 # project.
 # Michael Bosch <michael@lonelyviking.com>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security-Too 4.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Michael Bosch <michael@lonelyviking.com>\n"
 "Language: af_ZA\n"
 "Language-Team: af_ZA <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Intekening Benodig"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Welkom"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Bevestig asseblief jou e-pos adres"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Intekening instruksies"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Jou wagwoord is teruggestel"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Jou wagwoord is verander"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Wagwoord terugstel instruksies"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Twee-faktoor Intekening"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Twee-faktoor Redding"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Verifikasie Kode"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Insette nie geskik vir die versoekte API nie"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Jy het nie toestemming om hierdie hulpbron te bekyk nie."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Jy is nie geverifieer nie. Verskaf asseblief die korrekte getuigskrifte"
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Jy moet herverifieer om toegang te kry tot hierdie eindpunt"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Dankie. Bevestigings instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Dankie. Jou e-pos adres is bevestig."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Jou e-pos adres is reeds bevestig."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr ""
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s is reeds geassosieer met 'n rekening."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Identiteits kenmerk '%(attr)s' met waarde '%(value)s' is reeds "
 "geassosieer met 'n rekening."
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Wagwoord stem nie ooreen nie"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Wagwoorde stem nie ooreen nie"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Herleiding buite die domein is verbied"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instruksies om jou wagwoord terug te stel is gestuur na %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Jy het nie jou wagwoord terug gestel binne %(within)s nie. Nuwe "
 "instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Ongeldige wagwoord terugstellings token."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "E-pos adres benodig bevestiging"
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bevestigings instruksies is gestuur na %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Jy het nie jou e-pos adres bevestig binne %(within)s nie. Nuwe "
 "instruksies om jou e-pos adres te bevestig is gestuur na %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Jy het nie ingeteken binne %(within)s nie. Nuwe instruksies om in te "
 "teken is gestuur na %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruksies om in te teken is gestuur na %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Ongeldige intekenings token."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Rekening is gestremd."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "E-pos is nie voorsien nie"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Ongeldige e-pos adres"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Ongeldige kode"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Wagwoord is nie voorsien nie"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Wagwoord moet ten minste %(length)s karakters bevat"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Wagwoord is te eenvoudig"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefoon nommer is ongeldig, bv. afwesige lands kode"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Gespesifieerde verbruiker bestaan nie"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Ongeldige wagwoord"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Voorsiende wagwoord of kode is ongeldig"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Jy het met sukses in geteken"
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Wagwoord vergeet?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Jy het met sukses jou wagwoord teruggestel en jy het automaties in "
 "geteken."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Jou nuwe wagwoord moet verskil van jou vorige wagwoord."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Jy het met sukses jou wagwoord verander."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Teken asseblief in om toegang te kry tot hierdie blad."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Herverifieer asseblief om toegang te kry tot hierdie blad."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Herverifikasie suksesvol"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Jy kan slegs hierdie eindpunt bereik wanneer jy nie in geteken is nie."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Mislukking met stuur van kode. Probeer asseblief later weer"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Jy het met sukses jou twee-faktoor metode verander."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Jy het tans nie toestemming om hierdie blad te besoek nie"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Gemerkde metode is nie geldig nie"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Jy het met sukses twee-faktoor verifikasie afgeskakel"
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Versoekte metode is nie geldig nie"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Opstel moet voltooi wees binne %(within)s. Begin asseblief oor."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Jy moet 'n valiede identiteit spesifiseer om in te teken"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Gebruik hierdie kode om in te teken: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-pos adres"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2019-06-16 00:12+0200\n"
 "Last-Translator: Orestes Sanchez <miceno.atreides@gmail.com>\n"
 "Language: ca_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/ca_ES/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,437 +4,437 @@
 # project.
 # Orestes Sanchez <miceno.atreides@gmail.com>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2019-06-16 00:12+0200\n"
 "Last-Translator: Orestes Sanchez <miceno.atreides@gmail.com>\n"
 "Language: ca_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Per poder veure la pàgina sol·licitada és necessari iniciar la sessió"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Benvingut"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Si us plau, confirmeu el vostre correu electrònic"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instruccions d'inici de la sessió"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "S'ha restablit la teva contrasenya"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "S'ha canviat la teva contrasenya"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instruccions de recuperació de la contrasenya"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "No tens permís d'accés per a consultar aquest recurs."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Moltes gràcies. S'ha enviat un correu electrònic a %(email)s amb "
 "instruccions per confirmar el teu compte."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Moltes gràcies. S'ha confirmat el teu correu electrònic."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "El teu correu electrònic ja s'havia confirmat."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Token de confirmació no vàlid."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ja es associat amb un compte."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "La contrasenya no coincideix"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Les contrasenyes no coincideixen"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Les redireccions a llocs web externes s'han prohibit"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Les instruccions per restablir la teva contrasenya s'han enviat a "
 "%(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "No vas restablir la teva contrasenya abans de %(within)s. S'han enviat "
 "noves instruccions a %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "El token per restablir la contrasenya no és vàlid."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "El correu electrònic requereix d'una confirmació."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Les instruccions de confirmació s'han enviat a %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "No vas confirmar el teu correu electrònic abans de %(within)s. S'han "
 "enviat noves instruccions a %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No vas iniciar la sessió abans de %(within)s. S'han enviat noves "
 "instruccions a %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "S'han enviat instruccions per l'inici de sessió a %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Token de d'inici de sessió no vàlid."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "el compte està desactivat."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "No s'ha inclòs el correu electrònic"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Adreça de correu electrònic no vàlida"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "No s'ha inclòs la contrasenya"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "La contrasenya ha de tenir al menys %(length)s caràcters"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "L'usuari no existeix"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Contrasenya no vàlida"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "La sessió s'ha iniciat amb èxit."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Has oblidat la teva contrasenya?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Has restablert la teva contrasenya amb èxit i s'ha iniciat la sessió "
 "automàticament."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "La nova contrasenya ha de ser diferent de l'anterior."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "La teva contrasenya s'ha modificat amb èxit."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Has d'iniciar sessió per tal d'accedir a aquesta pàgina."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Has d'iniciar una nova sessió per tal d'accedir a aquesta pàgina."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Correu electrònic"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-03-23 14:04+0100\n"
 "Last-Translator: Leonhard Printz <leonhardprintz@protonmail.ch>\n"
 "Language: da_DK\n"
 "Language-Team: da_DK <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/da_DK/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,435 +4,435 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-03-23 14:04+0100\n"
 "Last-Translator: Leonhard Printz <leonhardprintz@protonmail.ch>\n"
 "Language: da_DK\n"
 "Language-Team: da_DK <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Login påkræveet"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Velkommen"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Bekræft venligst din email"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Logininstruktioner"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Din adgangskode er blevet nulstillet"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Din adgangskode er blevet ændret"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instruktioner til nulstilling af adganskode"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Du har ikke adgang til denne resource."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Mange tak. Bekræftelsesinstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Mange Tak. Din email er blevet bekræftet."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Din email er allerede blevet bekræftet."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Ugyldig bekræftigelsestoken."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s er allerede brugt af en anden konto."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Adgangskode passer ikke"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Adgangskoderne passer ikke"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Omdirigering udenfor domænet er forbudt"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Instruktioner til nulstilling af din adgangskode er blevet sendt til "
 "%(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Du har ikke nulstillet din adgangskode indenfor %(within)s. Nye "
 "instruktioner er sendt til %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Ugyldig nulstillingstoken."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Email kræver bekræftigelse."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bekræftigelsesinstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Du har ikke bekræftet din email indenfor %(within)s. Nye instruktioner er"
 " blevet sendt til %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Du har ikke logget in indenfor %(within)s. Nye logininstruktioner er "
 "blevet sendt til %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Logininstruktioner er blevet sendt til %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Ugyldig logintoken."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Kontoen er deaktiveret."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Email ikke angivet"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Ugyldig email adresse"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Adgangskode ikke angivet"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Adgangskoden skal indeholde mindst %(length)s tegn"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Denne bruger findes ikke"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Ugyldig adgangskode"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Du er hermed blevet logget ind."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Glemt adgangskode?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Du har hermed nulstillet din adgangskode og er blevet automatisk logget "
 "ind."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Din nye adgangskode skal være anderledes end din tidligere adgangskode."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Du har hermed ændret din adgangskode."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Log in for at få adgang til denne side."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Bekræft identitet for at få adgang til denne side."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Email adresse"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2022-04-05 13:50+0200\n"
 "Last-Translator: Pascua Theus <pascua@identeco.de>\n"
 "Language: de_DE\n"
 "Language-Team: de_DE <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/de_DE/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,450 +6,450 @@
 # Erich Seifert <dev@erichseifert.de>, 2017.
 # Pascua Theus <pascua@identeco.de>, 2021-2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.1.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2022-04-05 13:50+0200\n"
 "Last-Translator: Pascua Theus <pascua@identeco.de>\n"
 "Language: de_DE\n"
 "Language-Team: de_DE <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Anmeldung erforderlich"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Willkommen"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Bitte E-Mail-Adresse bestätigen"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Anmeldeanleitung"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Das Passwort wurde zurückgesetzt"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Das Passwort wurde geändert"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Anleitung zur Passwortwiederherstellung"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Zwei-Faktor-Anmeldung"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Zwei-Faktor-Wiederherstellung"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Verifizierungscode"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Ungültige Eingabe für die angeforderte Ressource"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 "Authentifizierung fehlgeschlagen – Identität oder Passwort/Passcode "
 "ungültig"
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Wenn diese E-Mail-Adresse bei uns existiert, erhalten Sie eine E-Mail, in"
 " der beschrieben wird, wie Sie Ihr Passwort zurücksetzen können."
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Wenn diese Identität bei uns existiert, wird Ihnen ein Code zugesandt."
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Sie haben keine Berechtigung, um diese Ressource zu sehen."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Sie sind nicht angemeldet. Bitte geben Sie die korrekten Zugangsdaten ein."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Bitte neu authentisieren, um auf diese Seite zuzugreifen."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Vielen Dank. Bestätigungsanleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Vielen Dank. Die E-Mail-Adresse wurde bestätigt."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Die E-Mail-Adresse wurde bereits bestätigt."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Ungültiger Bestätigungscode."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ist bereits mit einem Konto verknüpft."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Benutzermerkmal '%(attr)s' mit Wert '%(value)s' ist bereits mit einem "
 "anderen Benutzerkonto verknüpft"
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Das Passwort stimmt nicht überein"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Die Passwörter stimmen nicht überein"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Weiterleitungen außerhalb der Domain sind verboten"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr "Wiederherstellungscode ungültig"
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Eine Anleitung, um das Passwort wiederherzustellen wurde an %(email)s "
 "gesendet."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Das Passwort wurde nicht innerhalb von %(within)s zurückgesetzt. Eine "
 "neue Anleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Ungültiger Passwortwiederherstellungscode."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Die E-Mail-Adresse muss bestätigt werden."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Bestätigungsanleitung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Die E-Mail-Adresse wurden nicht innerhalb von %(within)s bestätigt. Neue "
 "Instruktionen wurden an %(email)s gesendet."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Die Anmeldung erfolgte nicht in %(within)s. Eine neue Anleitung wurde an "
 "%(email)s gesendet."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Eine Anleitung zur Anmeldung wurde an %(email)s gesendet."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Ungültiger Anmeldecode."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Konto ist deaktiviert."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Keine E-Mail-Adresse angegeben"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Ungültige E-Mail-Adresse"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Ungültiger Code"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Kein Passwort angegeben"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Das Passwort muss mindestens %(length)s Zeichen lang sein"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Passwort ist nicht komplex genug"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Passwort ist öffentlich bekannt"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "Konnte keine Verbindung zum Dienst aufbauen, um Passwörter zu überprüfen."
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefonnumer ist ungültig, eventuell fehlt die Landesvorwahl"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Der angegebene Benutzer existiert nicht"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Ungültiges Passwort"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Übermitteltes Passwort oder Code ist ungültig"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Sie wurden angemeldet."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Passwort vergessen?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Das Passwort wurde erfolgreich wiederhergestellt und die Anmeldung "
 "erfolgte automatisch."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Das neue Passwort muss sich vom vorherigen unterscheiden."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Das Passwort wurde erfolgreich geändert."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Bitte melden Sie sich an, um diese Seite zu sehen."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Bitte neu anmelden, um auf diese Seite zuzugreifen."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Neuanmeldung erfolgreich"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Dieser Endpunkt ist nur für angemeldete Nutzer erlaubt."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr "Code wurde gesendet."
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 "Zusendung des Codes fehlgeschlagen. Bitte versuchen Sie es später noch "
 "einmal."
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr "Ihr Code wurde bestätigt."
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Sie haben Ihre Zwei-Faktor-Methode erfolgreich geändert."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Sie haben aktuell nicht die nötigen Rechte, um die Seite anzusehen"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Ausgewählte Methode ist nicht gültig"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Zwei-Faktor-Authentisierung wurde deaktiviert"
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Angefragte Methode ist ungültig"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Einrichtung muss innerhalb %(within)s abgeschlossen werden. Bitte neu "
 "beginnen."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Single-User-Login erfolgreich eingerichtet"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Sie müssen eine gültige Identität auswählen, um sich anzumelden"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Code zur Anmeldung: %(code)s"
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Der Benutzername muss mindestens %(min)d und darf nicht länger als "
 "%(max)d Zeichen sein."
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "Der Benutzername enthält ungültige Zeichen."
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "Der Benutzername darf nur aus Buchstaben und Ziffern bestehen"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "Benutzername nicht angegeben"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s ist bereits mit einem Benutzerkonto verknüpft."
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 "Der WebAuthn-Vorgang muss innerhalb von %(within)s beendet werden. Bitte "
 "erneut versuchen."
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr "Zum Setzen eines neuen Webauthn-Tokens ist ein Nickname erforderlich."
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s ist bereits mit einem Webauthn-Token verknüpft."
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s ist für den aktuellen Benutzer nicht eingetragen."
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr "Der Token '%(name)s' wurde entfernt."
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr "Der WebAuthn-Token '%(name)s' wurde hinzugefügt."
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr "WebAuthn-Token-ID wurde bereits eingetragen."
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr "Nicht eingetragene WebAuthn-Token-ID."
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "WebAuthn-Token gehört zu keinem Benutzer."
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Konnte WebAuthn-Token nicht verifizieren: %(cause)s."
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr "WebAuthn-Token ist für diese Verwendung nicht eingetragen."
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr "Benutzerhandle des WebAuthn-Token stimmt nicht überein."
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-Mail-Adresse"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-08-25 17:21+0200\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: es_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/es_ES/LC_MESSAGES/flask_security.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,442 +4,442 @@
 # project.
 # Mauko Quiroga <mauko.quiroga@data.gouv.fr>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-08-25 17:21+0200\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: es_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Inicio de sesión necesario"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bienvenido"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Por favor, confirma tu correo electrónico"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instrucciones para iniciar sesión"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Tu contraseña ha sido restablecida"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Tu contraseña ha sido cambiada"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instrucciones de recuperación de contraseña"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Inicio de sesión de dos factores"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Recuperación de sesión de dos factores"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Código de verificación"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Entrada no apropiada para la API solicitada"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "No tienes permiso para consultar este recurso."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "No estás autenticado. Por favor, proporciona las credenciales correctas."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Debes volver a autenticarte para acceder a este recurso"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Gracias. Un correo con instrucciones sobre cómo confirmar tu cuenta ha "
 "sido enviado a %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Gracias. Tu correo electrónico ha sido confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Tu correo electrónico ya ha sido confirmado."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Autentificador de confirmación inválido."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s ya está asociado a una cuenta."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "El atributo de identidad '%(attr)s' con el valor '%(value)s' ya está "
 "asociado con una cuenta."
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "La contraseña no coincide"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Las contraseñas no coinciden"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Las redirecciones a sitios web externos están prohibidas"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Las instrucciones para restablecer tu contraseña han sido enviadas a "
 "%(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "No restableciste tu contraseña antes de %(within)s. Nuevas instrucciones "
 "han sido enviadas a %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Autentificador de restablecimiento de contraseña inválido."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "El correo electrónico requiere confirmación."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Las instrucciones de confirmación se han enviado a %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "No confirmaste tu correo electrónico antes de %(within)s. Nuevas "
 "instrucciones para confirmar tu correo electrónico han sido enviadas a "
 "%(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "No iniciaste sesión antes de %(within)s. Nuevas instrucciones para "
 "iniciar sesión han sido enviadas a %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instrucciones para iniciar sesión han sido enviadas a %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Autenticador de inicio de sesión inválido."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Cuenta deshabilitada."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Correo electrónico no indicado"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Dirección de correo electrónico inválida"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Código no válido"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Contraseña no indicada"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "La contraseña debe tener al menos %(length)s caracteres"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "La contraseña no es lo suficientemente compleja"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Contraseña en lista infringida"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "No se pudo contactar con el sitio de contraseñas infringidas"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "El número de teléfono no es válido, p. ej. falta el código de país"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Usuario·a especificado·a no existe"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Contraseña inválida"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "La contraseña o el código facilitado no es válido"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Has iniciado sesión con éxito."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "¿Has olvidado tu contraseña?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Has restablecido tu contraseña con éxito y has iniciado sesión "
 "automáticamente."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Tu nueva contraseña debe ser diferente de la antigua."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Has cambiado tu contraseña con éxito."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Debes iniciar sesión para poder acceder a esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Deber iniciar sesión nuevamente para poder acceder a esta página."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Reautenticación exitosa"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Solo puedes acceder a este recurso si no estás conectado."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "No se pudo enviar el código. Por favor, inténtelo de nuevo más tarde"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Cambiaste con éxito tu método de dos factores."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Actualmente no tienes permisos para acceder a esta página"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "El método marcado no es válido"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Has deshabilitado con éxito la autorización de dos factores."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "El método solicitado no es válido"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "La configuración debe completarse en %(within)s. Empiece de nuevo."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "El inicio de sesión unificado se configuró correctamente"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Debes especificar una identidad válida para iniciar sesión"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Utiliza este código para iniciar sesión: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "El nombre de usuario debe tener al menos %(min)d caracteres y menos de "
 "%(max)d caracteres"
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "El nombre de usuario contiene caracteres no válidos"
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "El nombre de usuario solo puede contener letras y números"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "Nombre de usuario no proporcionado"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s ya está asociado a una cuenta."
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Correo electrónico"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-11-28 13:41+0100\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: eu_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/eu_ES/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,435 +4,435 @@
 # project.
 # Martin Mozos <martinmozos@gmail.com>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-11-28 13:41+0100\n"
 "Last-Translator: Martin Mozos <martinmozos@gmail.com>\n"
 "Language: eu_ES\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Saioa hasi behar da"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Ongi etorri"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Mesedez berretsi zure posta elektronikoa"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Saioa hasteko argibideak"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Zure pasahitza berrezarri da"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Zure pasahitza aldatu da"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Pasahitza berreskuratzeko argibideak"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Bi faktoreko saioa hastea"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Bi faktoreko saioa berreskuratzea"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Egiaztapen kodea"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Sarrera ez da egokia eskatutako APIarentzat"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Ez duzu baliabide hau kontsultatzeko baimenik."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Ez zaude autentifikatuta. Mesedez, eman egiaztagiri zuzenak."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Baliabide honetara sartzeko berriro autentifikatu behar duzu"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Eskerrik asko. Baieztapen argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Eskerrik asko. Zure posta elektronikoa berretsi da."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Zure posta elektronikoa dagoeneko baieztatuta dago."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Berrespen token baliogabea."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s dagoeneko kontu batekin lotuta dago."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "'%(attr)s' identitate atributua '%(value)s' balioarekin dagoeneko kontu "
 "batekin lotuta dago"
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Pasahitza ez dator bat"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Pasahitzak ez datoz bat"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Domeinutik kanpoko birbideratzeak debekatuta daude"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Pasahitza berrezartzeko argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Ez duzu zure pasahitza berrezarri %(within)s barruan. Argibide berriak "
 "bidali dira %(email)s-era."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Pasahitza berrezartzeko token baliogabea."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Mezu elektronikoak berrespena behar du."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Baieztapen argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Ez duzu zure posta elektronikoa berretsi %(within)s barruan. Zure posta "
 "elektronikoa berresteko argibide berriak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Ez duzu saioa hasi %(within)s barruan. Saioa hasteko argibide berriak "
 "%(email)s helbidera bidali dira."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Saioa hasteko argibideak %(email)s helbidera bidali dira."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Saioa hasteko token baliogabea."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Kontua desgaituta dago."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Helbide elektronikoa beharrezkoa da"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Helbide elektroniko baliogabea"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Kode baliogabea"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Pasahitza beharrezkoa da"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Pasahitzak gutxienez %(length)s karaktere izan behar ditu"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Pasahitza ez da nahikoa konplexua"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Pasahitza urratutako zerrendan"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "Ezin izan da urratutako pasahitzen iturburuarekin harremanetan jarri"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Telefono zenbakiak ez du balio, baliteke herrialde kodea faltatzea"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Zehaztutako erabiltzea ez da existitzen"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Pasahitz okerra"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Zehaztutako pasahitzak edo kodeak ez du balio"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Behar bezala hasi duzu saioa."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Pasahitza ahaztua?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Pasahitza berrezarri duzunez automatikoki hasi duzu saioa."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Zure pasahitz berriak zure aurreko pasahitzaren ezberdin behar du izan."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Pasahitza behar bezala aldatu duzu."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Hasi saioa orri honetara sartzeko."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Mesedez, berriro autentifikatu orri honetara sartzeko."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Berautentifikatzea osatu da"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Saioa amaitzen ez duzunean soilik sar zaitezke baliabide honetara"
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Ezin izan da kodea bidali. Saiatu berriro geroago"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Bi faktoretako metodoa ondo aldatu duzu."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Une honetan ez duzu baimenik orrialde honetara sartzeko"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Markatutako metodoak ez du balio"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Bi faktoreren baimena behar bezala desgaitu duzu."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Eskatutako metodoak ez du balio"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Konfigurazioa %(within)s barruan osatu behar da. Mesedez, berriro hasi."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Bateratutako saio hasierarako konfigurazioa ongi egin da"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Saioa hasteko identitate baliagarria zehaztu behar duzu"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Erabili kode hau saioa hasteko: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Erabiltzaile izenak gutxienez %(min)d karaktere eta %(max)d karaktere "
 "baino gutxiago izan behar ditu"
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "Erabiltzaile izenak legez kanpoko karaktereak ditu"
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "Erabiltzaile izenak letrak eta zenbakiak soilik izan ditzake"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "Erabiltzaile izena ez da eman"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s dagoeneko kontu batekin lotuta dago."
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Posta elektronikoa"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/flask_security.pot` & `Flask-Security-Too-5.2.0/flask_security/translations/flask_security.pot`

 * *Files 1% similar despite different names*

```diff
@@ -3,425 +3,425 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: Flask-Security 5.1.0\n"
+"Project-Id-Version: Flask-Security 5.2.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr ""
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr ""
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr ""
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr ""
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr ""
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr ""
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr ""
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr ""
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr ""
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr ""
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr ""
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr ""
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr ""
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr ""
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr ""
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr ""
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr ""
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr ""
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr ""
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr ""
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr ""
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr ""
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr ""
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr ""
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr ""
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr ""
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr ""
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr ""
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr ""
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-06-08 10:13+0200\n"
 "Last-Translator: Alexandre Bulté <alexandre@bulte.net>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/fr_FR/LC_MESSAGES/flask_security.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,435 +4,435 @@
 # project.
 # Alexandre Bulté <alexandre@bulte.net>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-06-08 10:13+0200\n"
 "Last-Translator: Alexandre Bulté <alexandre@bulte.net>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Connexion requise"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bienvenue"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Merci de confirmer votre adresse email"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instructions de connexion"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Votre mot de passe a été réinitialisé"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Votre mot de passe a été changé"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instructions de réinitialisation de votre mot de passe"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Vous n'avez pas l'autorisation d'accéder à cette ressource."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Merci de vous reconnecter pour accéder à cette page."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Merci. Les instructions de confirmation ont été envoyées à %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Merci. Votre adresse email a été confirmée."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Votre adresse email a déjà été confirmée."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Token de confirmation non valide."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "L'adresse %(email)s est déjà utilisée."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Le mot de passe ne correspond pas"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Les mots de passe ne correspondent pas"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Les redirections en dehors du domaine sont interdites"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Les instructions de réinitialisation de votre mot de passe ont été "
 "envoyées à %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Vous n'avez pas réinitialisé votre mot de passe dans l'intervalle requis "
 "(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Token de réinitialisation non valide."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Une confirmation de l'adresse email est requise."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Les instructions de confirmation ont été envoyées à %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Vous n'avez pas confirmé votre adresse email dans l'intervalle requis "
 "(%(within)s)De nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Vous ne vous êtes pas connecté dans l'intervalle requis (%(within)s)De "
 "nouvelles instructions ont été envoyées à %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Les instructions de connexion ont été envoyées à %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Token de connexion non valide."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Le compte est désactivé."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Merci d'indiquer une adresse email"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Adresse email non valide"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Code invalide"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Merci d'indiquer un mot de passe"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Le mot de passe doit comporter au moins %(length)s caractères"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Numéro de téléphone non valide, par ex. code pays manquant"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Cet utilisateur n'existe pas"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Mot de passe non valide"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Le mot de passe ou le code soumis n'est pas valide"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Vous êtes bien connecté."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Mot de passe oublié&thinsp;?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Vous avez bien réinitialisé votre mot de passe et avez été "
 "automatiquement connecté."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Votre nouveau mot de passe doit être différent du précédent."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Vous avez bien changé votre mot de passe."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Merci de vous connecter pour accéder à cette page."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Merci de vous reconnecter pour accéder à cette page."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Réauthentification réussie"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Vous avez réussi à modifier votre méthode à deux facteurs."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Configuration de la connexion unifiée réussie"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Vous devez spécifier une identité valide pour vous connecter"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr "Le surnom du nouvel identifiant est requis."
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr "Identifiant non enregistré pour cet usage (premier ou secondaire)"
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Adresse email"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu_HU\n"
 "Language-Team: hu_HU <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/hu_HU/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,449 +4,449 @@
 # project.
 # FIRST AUTHOR ritt.alex@gmail.com, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu_HU\n"
 "Language-Team: hu_HU <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Bejelentkezés szükséges"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Üdvözöljük"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Kérjük, erősítse meg e-mail címét"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Bejelentkezési utasítások"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "A jelszava visszaállításra került"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "A jelszava megváltozott"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Jelszó visszaállítási utasítások"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Kétfaktoros Bejelentkezés"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Kétfaktoros Visszaállítás"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Ellenőrző kód"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "A bemenet nem megfelelő a kért API-hoz"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr "Sikertelen hitelesítés - azonosító vagy jelszó/kód érvénytelen"
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Ha ez az e-mail cím szerepel a rendszerünkben, akkor kapni fog egy "
 "e-mailt a jelszó visszaállítási menetéről."
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Ha ez az azonosító szerepel a rendszerünkben, akkor kódot küldtünk."
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Nincs jogosultsága ennek az erőforrásnak a megtekintéséhez."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Ön nincs hitelesítve. Kérjük, adja meg a megfelelő hitelesítő adatokat."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "A végpont eléréséhez újra hitelesíteni kell"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Köszönjük. A megerősítő utasításokat elküldtük a következő címre: "
 "%(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Köszönjük. E-mail címét megerősítettük."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Az e-mail címét már megerősítették."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Érvénytelen megerősítő token."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s már társítva van egy fiókhoz."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "A \"%(attr)s\" azonosító attribútum \"%(value)s\" értékkel már társítva "
 "van egy fiókhoz."
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "A jelszó nem egyezik"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "A jelszavak nem egyeznek"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "A tartományon kívüli átirányítások tilosak"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr "A helyreállítási kód érvénytelen"
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "A jelszó visszaállítására vonatkozó utasításokat elküldtük a következő "
 "címre: %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Nem állította vissza jelszavát %(within)s időn belül. Új utasításokat "
 "küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Érvénytelen jelszó-visszaállítási token."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Az e-mail megerősítést igényel."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "A megerősítő utasításokat elküldtük a következő címre: %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Nem erősítette meg e-mail-címét %(within)s-en belül. Az e-mail "
 "megerősítéséhez új utasításokat küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nem jelentkezett be %(within)s-en belül. Új bejelentkezési utasításokat "
 "küldtünk a következő címre: %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 "A bejelentkezéshez szükséges utasításokat elküldtük a következő címre: "
 "%(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Érvénytelen bejelentkezési token."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "A fiók le van tiltva."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "E-mail nincs megadva"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Érvénytelen e-mail cím"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Érvénytelen kód"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Nincs megadva a jelszó"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A jelszónak legalább %(length)s karakterből kell állnia"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "A jelszó nem elég összetett"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "A telefonszám nem érvényes, pl. hiányzik az országkód"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "A megadott felhasználó nem létezik"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Érvénytelen jelszó"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "A beküldött jelszó vagy kód érvénytelen"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Sikeresen bejelentkezett."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Elfelejtette jelszavát?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Sikeresen visszaállította jelszavát, és automatikusan be is jelentkezett."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Az új jelszavának különböznie kell a korábbi jelszavától."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Sikeresen megváltoztatta a jelszavát."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Kérjük, jelentkezzen be az oldal eléréséhez."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Kérjük, hitelesítse újra az oldal eléréséhez."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Az újrahitelesítés sikeres"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "\"Csak akkor érheti el ezt a végpontot, ha nincs bejelentkezve."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr "A kód elküldve."
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Nem sikerült elküldeni a kódot. Kérjük, próbálja újra később."
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr "A kódod megerősítésre került"
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Sikeresen megváltoztatta a kétfaktoros hitelesítést."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Jelenleg nincs jogosultsága az oldal eléréséhez"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "A megjelölt metódus nem érvényes"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Sikeresen letiltotta a kétfaktoros hitelesítést."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "A kért metódus nem érvényes"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "A telepítést %(within)s időn belül be kell fejezni. Kezdje újra."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Az egységes bejelentkezés beállítása sikeres"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "A bejelentkezéshez érvényes azonositót kell megadnia"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Használja ezt a kódot a bejelentkezéshez: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "A felhasználónévnek legalább %(min)d karakterből és kevesebb mint %(max)d"
 " karakterből kell állnia"
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "A felhasználónév illegális karaktereket tartalmaz"
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "A felhasználónév csak betűket és számokat tartalmazhat"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "A felhasználónév nincs megadva"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "%(username)s már hozzá van rendelve egy fiókhoz."
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr "A WebAuthn műveletet %(within)s időn belül be kell fejezni. Kezdje újra."
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr "Az új hitelesítő adatokhoz becenév szükséges."
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s már hozzá van rendelve egy hitelesítő adathoz."
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s nincs regisztrálva az aktuális felhasználónál."
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 "A WebAuthn hitelesítő adatok sikeresen törölve a következő névvel: "
 "%(name)s"
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 "Sikeresen hozzáadva a WebAuthn hitelesítő adatot a következő névvel: "
 "%(name)s"
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr "A WebAuthn hitelesítő adatazonosítója már regisztrálva."
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr "Nem regisztrált WebAuthn hitelesítő adat azonosítója."
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "A WebAuthn hitelesítő adatok nem tartoznak egyetlen felhasználóhoz sem."
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Nem sikerült ellenőrizni a WebAuthn hitelesítő adatait: %(cause)s."
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 "A hitelesítő adat nincs regisztrálva ehhez a felhasználáshoz (első vagy "
 "másodlagos)"
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-mail"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-12-01 11:47+0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hy_AM\n"
 "Language-Team: hy_AM <ramirjanyan@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/hy_AM/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,434 +4,434 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-12-01 11:47+0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hy_AM\n"
 "Language-Team: hy_AM <ramirjanyan@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Անհրաժեշտ է մուտք գործել"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Բարի գալուստ"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Հաստատեք Ձեր էլ․փոստի հասցեն"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Մուտքի հրահանգներ"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Ձեր գաղտնաբառը վերականգնվել է"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Ձեր գաղտնաբառը փոխվեց"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Գաղտնաբառի վերականգնման հրահանգներ"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Երկու գործոնով մուտք"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Երկու գործոնով վերականգնում"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Վերահաստատման ծածկագիր"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Մուտքը չի համապատասխանում հայցվող API֊ին"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Դուք այս ռեսուրսը դիտելու թույլտվություն չունեք"
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Դուք նույնականացված չեք: Խնդրում ենք մուտքագրել ճիշտ տվյալներ։"
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Դուք պետք է կրկին նույնականցվեք որպեսզի այստեղ մուտք գործեք"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Շնորհակալություն. Հաստատման հրահանգներն ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Շնորհակալություն. Ձեր էլ․փոստի հասցեն հաստատվել է։"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Ձեր էլ․փոստի հասցեն արդեն հաստատված է։"
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Հաստատման տոկենը անվավեր է։"
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s արդեն կապված է այլ օգտահաշվի հետ։"
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Գաղտնաբառը չի համապատասխանում"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Գաղտնաբառերը չեն համապատասխանում"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Դոմենից դուրս վերահղումներն արգելափակված են"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Գաղտնաբառի վերականգնման հրահանգներն ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Դուք ձեր գաղտնաբառը չեք վերականգնել %(within)s֊ի ընթացքում։ Նոր "
 "հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Գաղտնաբառի վերականգնման տոկենը անվավեր է։"
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Էլ․փոստի հասցեն պետք է հաստատել։"
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Հաստատման հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Դուք չեք հաստատել Ձեր էլ․փոստի հասցեն %(within)s ընթացքում։ Նոր "
 "հրահանգները էլ․փոստի հասցեի հաստատման համար ուղարկվել են %(email)s "
 "հասցեին։"
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Դուք մուտք չեք գործել %(within)s֊ի ընթացքում. Մուտքի նոր հրահանգները "
 "ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Մուտքի հրահանգները ուղարկվել են %(email)s հասցեին։"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Մուտքի անվավեր տոկեն։"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Օգտահաշիվն արգելափակված է։"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Էլ․փոստի հասցեն տրամադրված չէ"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Անվավեր էլ․փոստի հասցե"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Անվավեր ծածկագիր"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Գաղտնաբառը տրամադրված չէ"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Գաղտնաբառը պետք է պարունակի առնվազն %(length)s նիշ"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Գաղտնաբառը բավարար բարդ չէ"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Գաղտնաբառը բացված գաղտնաբառերի ցուցակում է"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "Չհաջողվեց կապվել բացված գաղտնաբառերի կայքի հետ"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Հեռախոսահամարը անվավեր է, օրինակ՝ բացակայում է երկրի կոդը"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Նշված օգտատերը գոյություն չունի"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Անվավեր գաղտնաբառ"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Ներկայացված գաղտնաբառը կամ ծածկագիրը վավեր չէ"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Դուք բարեհաջող մուտք էք գործել։"
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Մոռացել ե՞ք գաղտնաբառը"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Դուք հաջողությամբ վերականգնել եք ձեր գաղտնաբառը եւ մուտք էք գործել "
 "համակարգ ինքնաբերաբար։"
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Ձեր նոր գաղտնաբառը պետք է տարբերվի նախկինից"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Դուք հաջողությամբ փոխեցիք ձեր գաղտնաբառը։"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Մուտք գործեք այս էջից օգտվելու համար։"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Այս էջ մուտք գործելու համար անհրաժեշտ է նորից նույնականացվել:"
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Նույնականացումը հաջողված է"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Դուք կարող եք մտնել այս վերջնակետ միայն այն ժամանակ, երբ մուտք չեք գործել"
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Չհաջողվեց ուղարկել ծածկագիրը: Խնդրում ենք փորձել ավելի ուշ"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Դուք հաջողությամբ փոխեցիք ձեր երկու֊գործոն տարբերակը"
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Ներկայումս դուք չունեք այս էջ մուտք գործելու թույլտվություն"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Նշված տարբերակը վավեր չէ"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Դուք հաջողությամբ անջատել եք երկու գործոնի թույլտվությունը"
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Հայցվող մեթոդը վավեր չէ"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "Կարգավորումը պետք է ավարտվի %(within)s ընթացքում։ Խնդրում ենք նորից սկսել։"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Միասնական մուտքի տեղադրումը հաջող է"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Մուտք գործելու համար պետք է նշեք վավեր ինքնություն"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Մուտքի համար օգտագործեք այս ծածկագիրը․ %(code)s։"
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Էլեկտրոնային փոստի հասցե"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2022-04-23 17:04+0000\n"
 "Last-Translator: \n"
 "Language: is_IS\n"
 "Language-Team: is_IS <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n%10==1 && n%100!=11 ? 0 : 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/is_IS/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,433 +4,433 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 4.0.0\n"
 "Report-Msgid-Bugs-To: jwag956@github.com\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2022-04-23 17:04+0000\n"
 "Last-Translator: \n"
 "Language: is_IS\n"
 "Language-Team: is_IS <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n%10==1 && n%100!=11 ? 0 : 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Innskráningar er þörf"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Velkomin(n)"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Vinsamlegast staðfestu netfangið þitt"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Leiðbeiningar fyrir innskráningu"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Lykilorðið þitt hefur verið endurstillt"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Lykilorðinu þínu hefur verið breytt"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Leiðbeiningar um endurstillingu lykilorðs"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Tveggja þátta innskráning"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Staðfestingarkóði"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Þú hefur ekki heimild til að skoða þessa auðlind."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr ""
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Þakka þér fyrir. Leiðbeiningar fyrir staðfestingu hafa verið sendar á "
 "%(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Þakka þér fyrir. Netfangið þitt hefur verið staðfest."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Netfangið þitt hefur þegar verið staðfest."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Ógildur staðfestingarkóði."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s er þegar í notkun á öðrum reikningi."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Lykilorðið er ekki eins"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Lykilorðin eru ekki eins"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr ""
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "Leiðbeiningar um hvernig þú getur endurstillt lykilorðið þitt hafa verið "
 "sendar á %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr ""
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Netfangið þarfnast staðfestingar."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr ""
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr ""
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Aðgangurinn er óvirkur."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Netfang var ekki gefið upp"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Ógilt netfang"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Ógildur kóði"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Lykilorð var ekki gefið upp"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Lykilorð verða að vera að minnsta kosti %(length)s stafir"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Lykilorðið er ekki nógu flókið"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Lykilorðið er á lista yfir brotin lykilorð"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "Gat ekki haft samband við síðu yfir brotin lykilorð"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Símanúmerið er ekki gilt, t.d. vegna þess að landakóða vantar"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr ""
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Ógilt lykilorð"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Þér tókst að skrá þig inn."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Gleymt lykilorð?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Þér tókst að endurstilla lykilorðið þitt og þú hefur verið skráð(ur) inn "
 "sjálfkrafa."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Nýja lykilorðið þitt verður að vera öðruvísi en gamla lykilorðið."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Þér tókst að breyta lykilorðinu þínu."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Vinsamlegast skráðu þig inn til að opna þessa síðu."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr ""
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Notendanafnið verður að vera að minnsta kosti %(min)d stafir að lengd og "
 "styttra en %(max)d stafir"
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "Notendanafnið inniheldur óleyfileg tákn"
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "Notendanafnið má eingöngu innihalda bókstafi og tölustafi"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "Notendanafn var ekki gefið upp"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Netfang"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-01-25 14:12+0900\n"
 "Last-Translator: \n"
 "Language: ja\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/ja_JP/LC_MESSAGES/flask_security.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,426 +4,426 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-01-25 14:12+0900\n"
 "Last-Translator: \n"
 "Language: ja\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "ログインが必要です"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "ようこそ"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "メール アドレスの検証"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "ログイン手順"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "パスワード変更"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "パスワードが変更されました。"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "パスワード再設定手順"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "アクセス権がありません"
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "再度ログインしてください"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "ご登録ありがとうございます。%(email)sにメール アドレス検証手順が送信されました。"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "ありがとうございます。メール アドレスが検証されました。"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "メール アドレスは検証済みです"
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s のアカウントは既に作成されています"
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "パスワードが一致しません"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "入力したパスワードが一致していません"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "ドメイン外へのリダイレクトは禁止されています"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "パスワードの再設定手順が %(email)s に送信されました"
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr "%(within)s以内にパスワードを設定しませんでした。パスワード再設定手順を %(email)s に再度送信しました。"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "メール アドレスの検証が必要です"
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "%(email)sにメール アドレス検証手順が再送信されました"
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr "%(within)s以内にメール アドレスが検証されませんでした。新しい検証手順を %(email)s に送信しました。"
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr "%(within)s以内にログインしませんでした。ログイン手順を %(email)s に再度送信しました。"
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "%(email)sにログイン手順が送信されました"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "リンクが無効です"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "アカウントが無効になっています"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "メール アドレスを入力してください"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "正しいメール アドレスを入力してください"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "パスワードを入力してください"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr ""
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "入力を確認してください"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "入力を確認してください"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "ログインしました"
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "パスワードを忘れた場合"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "パスワードの再設定が完了しました。"
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "新旧パスワードが同じです"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "パスワードが変更されました"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "ログインしてください"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "再度ログインしてください"
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "メール アドレス"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-05-01 17:52+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl_NL\n"
 "Language-Team: nl_NL <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/nl_NL/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,438 +4,438 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-05-01 17:52+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl_NL\n"
 "Language-Team: nl_NL <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Inloggen Verplicht"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Welkom"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Gelieve uw e-mailadres te bevestigen"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Aanmeld instructies"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Uw wachtwoord werd gereset"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Uw wachtwoord werd gewijzigd"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Wachtwoord reset instructies"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Dubbele Authenticatie Aanmelding"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Dubbele Authenticatie Herstellen"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 #, fuzzy
 msgid "Verification Code"
 msgstr "Authenticatie Code"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "U heeft niet de nodige rechten om deze pagina te zien."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "U bent niet aangemeld. Voer alstublieft de juiste gegevens in."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Gelieve opnieuw in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Bedankt. Instructies voor bevestiging zijn verzonden naar %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Bedankt. Uw e-mailadres werd bevestigd."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Uw e-mailadres werd reeds bevestigd."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Ongeldige bevestiging token."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s is al gelinkt aan een ander account."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Wachtwoord komt niet overeen"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Wachtwoorden komen niet overeen"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Omleidingen buiten het domein zijn niet toegelaten"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instructies om uw wachtwoord te resetten werden verzonden naar %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "U heeft uw wachtwoord niet gereset gedurende %(within)s. Nieuwe "
 "instructies werden verzonden naar %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Ongeldig wachtwoord reset token."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "E-mailadres moet bevestigd worden."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Instructies ter bevestiging van uw e-mailadres werden verzonden naar "
 "%(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "U heeft uw e-mailadres niet bevestigd in de voorziene %(within)s. Nieuwe "
 "instructies ter bevestiging van uw e-mailadres werden verzonden naar "
 "%(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Je bent niet ingelogd geweest gedurende %(within)s. Nieuwe instructies om"
 " in te loggen werden verzonden naar%(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instructies om in te loggen werden verzonden naar %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Ongeldige aanmelding."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Account is geblokkeerd."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Email niet ingevuld"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Ongeldig e-mailadres"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 #, fuzzy
 msgid "Invalid code"
 msgstr "Niet valide token"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Wachtwoord niet ingevuld"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Uw wachtwoord moet minstens %(length)s karakters bevatten"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Deze gebruiker bestaat niet"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Ongeldig wachtwoord"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "U bent succesvol ingelogd."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Wachtwoord vergeten?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "U heeft uw wachtwoord succesvol gereset en bent nu automatisch ingelogd."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Uw nieuw wachtwoord moet verschillend zijn van het voorgaande wachtwoord."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Uw wachtwoord werd met succes gewijzigd."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Gelieve in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Gelieve opnieuw in te loggen om deze pagina te zien."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "U heeft succesvol uw Dubbele Authenticatie methode veranderd."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "U heeft niet de juiste permissies om deze pagina te laden"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "De gemarkeerde methode is niet valide"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "U heeft succesvol Dubbele Authenticatie uitgeschakeld."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 #, fuzzy
 msgid "Requested method is not valid"
 msgstr "De gemarkeerde methode is niet valide"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-mailadres"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-11-28 10:19+0100\n"
 "Last-Translator: Kamil Daniewski <kamil.daniewski@gmail.com>\n"
 "Language: pl_PL\n"
 "Language-Team: pl_PL <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/pl_PL/LC_MESSAGES/flask_security.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,442 +3,442 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2020-11-28 10:19+0100\n"
 "Last-Translator: Kamil Daniewski <kamil.daniewski@gmail.com>\n"
 "Language: pl_PL\n"
 "Language-Team: pl_PL <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Logowanie jest wymagane"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Witamy"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Prosimy o potwierdzenie Twojego adresu e-mail"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instrukcje logowania"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Twoje hasło zostało zresetowane"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Twoje hasło zostało zmienione"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instrukcje zmiany hasła"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Logowanie dwuskładnikowe"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Pomoc w logowaniu dwuskładnikowym"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Kod weryfikacyjny"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Nieprawidłowe dane dla żądanego API"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Nie posiadasz uprawnień, aby wyświetlić tę stronę."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 "Nie jesteś zalogowany. Prosimy o przesłanie prawidłowych danych "
 "uwierzytelniania."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Musisz zalogować się ponownie, aby wyświetlić tę stronę"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr ""
 "Dziękujemy. Instrukcje potwierdzenia rejestracji zostały wysłane na adres"
 " %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Dziękujemy. Twój adres e-mail został potwierdzony."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Twój adres e-mail już został potwierdzony."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Nieprawidłowy token potwierdzania adresu e-mail."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s jest już powiązany z kontem."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Atrybut identyfikujący '%(attr)s' z wartością '%(value)s' jest już "
 "powiązany z kontem."
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Hasło nie pasuje"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Hasła nie pasują do siebie"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Przekierowania poza domenę są zabronione"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Instrukcje resetowania hasła zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Nie ustawiłeś hasła w ciągu %(within)s. Nowe instrukcje zostały wysłane "
 "na adres %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Nieprawidłowy token resetowania hasła."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Wymagane jest potwierdzenie adresu e-mail."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Instrukcje potwierdzenia adresu e-mail zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Nie potwierdziłeś adresu e-mail w ciągu %(within)s. Nowe instrukcje "
 "zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Nie zalogowałeś się w ciągu %(within)s. Nowe instrukcje logowania zostały"
 " wysłane na adres %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instrukcje logowania zostały wysłane na adres %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Nieprawidłowy token logowania."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Konto jest wyłączone."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Adres e-mail nie został wprowadzony"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Nieprawidłowy adres e-mail"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Nieprawidłowy kod"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Hasło nie zostało wprowadzone"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Hasło musi zawierać co najmniej %(length)s znaków"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Hasło nie jest wystarczająco złożone"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Hasło znajduje się na liście haseł wykradzionych"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 "Nie udało się dotrzeć do podmiotu sprawdzającego hasło w bazie "
 "wykradzionych haseł"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Nieprawidłowiy numer telefonu (upewnij się, że zawiera kod kraju)"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Ten użytkownik nie istnieje"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Nieprawidłowe hasło"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Hasło lub wprowadzony kod są nieprawidłowe"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Zostałeś zalogowany pomyślnie."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Zapomniałeś hasło?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Ustawiono nowe hasło i zostałeś zalogowany pomyślnie."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Twoje nowe hasło musi być inne, niż obecne hasło."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Pomyślnie zmieniłeś hasło."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Prosimy o zalogowanie się, aby móc odwiedzić tę stronę."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Prosimy o ponowne zalogowanie się, aby móc odwiedzić tę stronę."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Ponownie zalogowano"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Możesz odwiedzić tę stronę tylko będąc niezalogowanym."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Nie udało się wysłać kodu. Prosimy spróbować później"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Metoda logowania dwuskładnikowego została zmieniona pomyślnie."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "Nie posiadasz uprawnień, aby odwiedzić tę stronę"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Wybrana metoda jest niewłaściwa"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Pomyślnie wyłączyłeś logowanie dwuskładnikowe."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Żądana metoda jest niewłaściwa"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Ustawienie musi zostać ukończone w ciągu %(within)s. Prosimy zacząć "
 "ponownie."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Ujednolicone logowanie przebiegło pomyślnie"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Musisz ustawić prawidłowy identyfikator, aby się zalogować"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Użyj tego kodu, aby się zalogować: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Adres e-mail"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-09-27 23:39-0300\n"
 "Last-Translator: José Neto <josenetodino@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/pt_BR/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,433 +4,433 @@
 # project.
 # José Neto <josenetodino@gmail.com>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2017-09-27 23:39-0300\n"
 "Last-Translator: José Neto <josenetodino@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Login obrigatório"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bem-vindo"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Por favor, confirme seu email"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instruções de login"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Sua senha foi redefinida"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Sua senha foi alterada"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instruções para redfinir a senha"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Você não tem permissão para ver este recurso"
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Por favor, reautentique-se para acessar esta página."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Obrigado. As instruções para a confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Obrigado. Seu email foi confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Seu email já foi confirmado."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Token de confirmação inválido."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s já está associado a uma conta."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Senha não confere"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Senhas não conferem"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Redirecionamentos para fora do domínio são proibidos"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "As instruções para redefinir sua senha foram enviadas para %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Você não redefiniu sua senha dentro de %(within)s. Novas instruções foram"
 " enviadas para %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Token de redefinição de senha inválido."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "O email requer confirmação."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "As instruções de confirmaç foram enviadas para %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Você não confirmou seu email dentro de %(within)s. Novas instruções foram"
 " enviadas para %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Você não logou dentro de %(within)s. Novas instruções para logar foram "
 "enviadas para %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruções para logar foram enviadas para %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Token de login inválido."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Conta desabilitada."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Email não informado"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Endereço de email inválido"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 #, fuzzy
 msgid "Invalid code"
 msgstr "Senha inválida"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Senha não informada"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A senha deve ter pelo menos 6 caracteres"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Usuário não existe"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Senha inválida"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Você logou com sucesso."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Esqueceu a senha?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Você redefiniu sua senha com sucesso e foi logado automaticamente."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Sua nova senha deve ser diferente da sua senha anterior."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Você alterou sua senha com sucesso."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Por favor, logue para acessar esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Por favor, reautentique-se para acessar esta página."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Endereço de email"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-04-27 14:00+0100\n"
 "Last-Translator: Micael Grilo <micael.grilo@outlook.com>\n"
 "Language: pt_PT\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/pt_PT/LC_MESSAGES/flask_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,436 +4,436 @@
 # project.
 # Micael Grilo <micael.grilo@outlook.com>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-04-27 14:00+0100\n"
 "Last-Translator: Micael Grilo <micael.grilo@outlook.com>\n"
 "Language: pt_PT\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Login obrigatório"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Bem-vindo"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Por favor, confirme o seu email"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Instruções de login"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "A sua palavra-passe foi redefinida"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "A sua palavra-passe foi alterada"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Instruções para redefinir a palavra-passe"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Não tem permissões para ver este recurso"
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Por favor, reautentique-se para aceder esta página."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Obrigado. As instruções para a confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Obrigado. O seu email foi confirmado."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "O seu email já foi confirmado."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Token de confirmação inválido."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s já está associado a uma conta."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Palavra-passe não coincide"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Palavras-passe não coincidem"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Redirecionamentos para fora do domínio são proibidos"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr ""
 "As instruções para redefinir a sua palavra-passe foram enviadas para "
 "%(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Não redefiniu a sua palavra-passe dentro de %(within)s. Novas instruções "
 "foram enviadas para %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Token de redefinição de senha inválido."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "O email requer confirmação."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "As instruções de confirmação foram enviadas para %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Não confirmou o seu email dentro de %(within)s. Novas instruções foram "
 "enviadas para %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Não iniciou sessão dentro de %(within)s. Novas instruções de inicio de "
 "sessão foram enviadas para %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Instruções para o inicio de sessão foram enviadas para %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Token de login inválido."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Conta desactivada."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Email em falta"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Endereço de email inválido"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Palavra-passe em falta"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "A palavra-passe deve ter pelo menos %(length)s caracteres"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Utilizador não existe"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Palavra-passe inválida"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Sessão iniciada com sucesso."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Esqueceu a palavra-passe?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr ""
 "Redefiniu a sua palavra-passe com sucesso e iniciou sessão "
 "automaticamente."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "A sua nova palavra-passe deve ser diferente da anterior."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Alterou a sua palavra-passe com sucesso."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Por favor, inicie sessão para aceder a esta página."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Por favor, reautentique-se para aceder esta página."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Endereço de email"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2023-01-25 04:14+0530\n"
 "Last-Translator: Ivan Fedorov <inbox@titaniumhocker.ru>\n"
 "Language: ru_RU\n"
 "Language-Team: Leonid R. <leovp@users.noreply.github.com>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/ru_RU/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,448 +4,448 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2023-01-25 04:14+0530\n"
 "Last-Translator: Ivan Fedorov <inbox@titaniumhocker.ru>\n"
 "Language: ru_RU\n"
 "Language-Team: Leonid R. <leovp@users.noreply.github.com>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Требуется авторизация"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Добро пожаловать"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Пожалуйста, подтвердите свой адрес электронной почты"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Инструкция для входа"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Ваш пароль был сброшен"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Ваш пароль был изменён"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Инструкции для восстановления пароля"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "Двухфакторный вход"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr "Двухфакторное восстановление"
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "Код подтверждения"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "Ввод некорректен для запрошенного API"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 "Аутентификация не удалась — идентификатор или пароль/код доступа "
 "недействительны"
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 "Если этот адрес электронной почты есть в нашей системе, вы получите "
 "письмо с описанием того, как сбросить пароль."
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr "Если этот идентификатор есть в нашей системе, вам был выслан код."
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "У вас нет прав доступа к этому ресурсу."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "Вы не аутентифицированы. Пожалуйста, укажите корректные учётные данные."
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Пожалуйста, войдите повторно чтобы получить доступ к этой странице"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Спасибо. Инструкции по подтверждению были отправлены на %(email)s."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Спасибо. Ваш почтовый адрес был подтверждён."
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "Ваш почтовый адрес уже подтверждён."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Неверный токен для подтверждения аккаунта."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s уже привязан к другому аккаунту."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 "Идентификационный атрибут '%(attr)s' со значением '%(value)s' уже "
 "ассоциирован с учетной записью."
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr "Идентификация %(id)s не зарегистрирована"
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 "Произошла ошибка при взаимодействии с провайдером Oauth. Пожалуйста, "
 "попробуйте ещё раз."
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Пароль не подходит"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Пароли не совпадают"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Перенаправления вне текущего домена запрещены"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr "Код восстановления недействителен"
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr "Коды восстановления еще не сгенерированы"
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Инструкции по восстановлению пароля были отправлены на %(email)s."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Вы не восстановили пароль в течение %(within)s. Новые инструкции были "
 "отправлены на %(email)s."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Неверный токен для восстановления пароля."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "Почтовый адрес требует подтверждения."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Инструкции по подтверждению были отправлены на %(email)s."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "Вы не подтвердили свой почтовый адрес в течение %(within)s. Новые "
 "инструкции по подтверждению отправлены на %(email)s."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "Вы не вошли в течение %(within)s. Новые инструкции по входу отправлены на"
 " %(email)s."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Инструкции по входу отправлены на %(email)s."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Неверный токен для входа."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Аккаунт отключён."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "Почтовый адрес не введён"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Неверный почтовый адрес"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr "Код недействителен"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Пароль не введён"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Пароль должен содержать не менее %(length)s символов"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "Пароль недостаточно сложный"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "Пароль в списке скомпрометированных"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "Не удалось соединиться с сайтом скомпрометированных паролей"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "Номер телефона некорректен, например, отсутствует код страны"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Указанный пользователь не существует"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Неверный пароль"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "Предоставленный пароль или код недействительны"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Вы успешно вошли в систему."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Забыли пароль?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Вы успешно сбросили пароль и автоматически вошли в систему."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Ваш новый пароль должен отличаться от предыдущего."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Вы успешно изменили свой пароль."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Пожалуйста, войдите чтобы получить доступ к этой странице."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Пожалуйста, войдите заново, чтобы получить доступ к этой странице."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "Повторный вход выполнен успешно"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "Вы можете получить доступ к данной странице, только если не авторизованы."
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr "Код отправлен."
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "Не удалось отправить код. Пожалуйста, попробуйте позже"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr "Ваш код был подтвержден"
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "Вы успешно изменили метод двухфакторной авторизации."
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "В настоящее время у вас нет доступа к данной странице"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "Отмеченный метод недействителен"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "Вы успешно отключили двухфакторную авторизацию."
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "Запрошенный метод недействителен"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 "Настройка должна быть завершена в течение %(within)s. Пожалуйста, начните"
 " заново."
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "Настройка единого способа входа прошла успешно"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "Вы должны указать действительный идентификатор для входа"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "Используйте данный код для входа: %(code)s."
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 "Имя пользователя должно содержать не менее %(min)d и не более %(max)d "
 "символов"
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr "Имя пользователя содержит недопустимые символы"
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr "Имя пользователя может содержать только буквы и цифры"
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr "Имя пользователя не указано"
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr "Имя пользователя %(username)s уже связано с учётной записью."
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 "Операция WebAuthn должна быть завершена в течение %(within)s. Пожалуйста,"
 " начните сначала."
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr "Требуется псевдоним для новых учётных данных."
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr "%(name)s уже связан с учётными данными."
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr "%(name)s не зарегистрирован с текущим пользователем."
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr "Учётные данные WebAuthn с именем %(name)s успешно удалены"
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr "Учётные данные WebAuthn с именем %(name)s успешно добавлены"
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr "Учётные данные WebAuthn уже зарегистрированы."
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr "Незарегистрированный идентификатор учетных данных WebAuthn."
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr "Учётные данные WebAuthn не принадлежат ни одному пользователю."
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr "Не удалось проверить учётные данные WebAuthn: %(cause)s."
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 "Учётные данные не зарегистрированы для этого использования (первичное или"
 " вторичное)"
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr "Несовпадение учётных данных пользователя"
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "Адрес электронной почты"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-12-20 18:48+0300\n"
 "Last-Translator: Ecmel B. Canlıer <me@ecmelberk.com>\n"
 "Language: tr_TR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/tr_TR/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,432 +3,432 @@
 # This file is distributed under the same license as the Flask-Security
 # project.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-12-20 18:48+0300\n"
 "Last-Translator: Ecmel B. Canlıer <me@ecmelberk.com>\n"
 "Language: tr_TR\n"
 "Language-Team: \n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "Giriş yapmanız gerekmektedir"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "Hoş Geldiniz"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "Lütfen e-posta adresinizi onaylayın"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "Giriş talimatları"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "Şifreniz yenilenmiştir"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "Şifreniz değiştirilmiştir"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "Şifre yenileme talimatları"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr ""
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr ""
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr ""
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "Bu maddeyi görmeye yetkiniz yoktur."
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr ""
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "Bu sayfaya erişebilmek için lütfen tekrardan giriş yapın."
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "Teşekkür ederiz. Onaylama talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "Teşekkür ederiz. E-posta adresiniz onaylanmıştır"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "E-posta adresiniz zaten onaylanmış."
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "Yanlış onaylama kodu."
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s başka bir hesaba bağlı."
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "Şifre yanlış"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "Şifreler uymuyor"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "Adres dışına yönlendirmeler yasaktır"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "Şifrenizi yenileme talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr ""
 "Şifrenizi %(within)s içinde yenilemediniz. Yeni talimatlar %(email)s "
 "adresine gönderilmiştir."
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "Yanlış şifre yenileme kodu."
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "E-posta onayı gerekmektedir."
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "Onaylama talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr ""
 "E-posta adresinizi %(within)s içinde onaylamadınız. Yeni onaylama "
 "talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr ""
 "%(within)s içinde giriş yapmadınız. Yeni giriş yapma talimatları "
 "%(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "Giriş yapma talimatları %(email)s adresine gönderilmiştir."
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "Yanlış giriş kodu."
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "Hesap kapalıdır."
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "E-posta verilmemiş"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "Yanlış e-posta adresi"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 msgid "Invalid code"
 msgstr ""
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "Şifre verilmemiş"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, fuzzy, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "Şifreniz en az %(length)s karakter olmalıdır"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr ""
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr ""
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr ""
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr ""
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "Böyle bir kullanıcı yok"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "Şifre yanlış"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr ""
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "Başarıyla giriş yaptınız."
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "Şifrenizi mi unuttunuz?"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "Şifreniz yenilenmiştir ve otomatik olarak giriş yapmış bulunmaktasınız."
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "Yeni şifreniz eski şifrenizden farklı olmalıdır."
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "Şifrenizi başarıyla değiştirdiniz."
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "Bu sayfaya erişebilmek için lütfen giriş yapın."
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "Bu sayfaya erişebilmek için lütfen tekrardan giriş yapın."
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr ""
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr ""
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr ""
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr ""
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr ""
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr ""
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr ""
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr ""
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr ""
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr ""
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr ""
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "E-posta Adresi"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo` & `Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-08-02 19:55+0800\n"
 "Last-Translator: SteinKuo <guoming054@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese Simplified <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po` & `Flask-Security-Too-5.2.0/flask_security/translations/zh_Hans_CN/LC_MESSAGES/flask_security.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,427 +4,427 @@
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Flask-Security 2.0.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2023-03-07 08:27-0800\n"
+"POT-Creation-Date: 2023-05-04 06:35-0700\n"
 "PO-Revision-Date: 2018-08-02 19:55+0800\n"
 "Last-Translator: SteinKuo <guoming054@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese Simplified <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: flask_security/core.py:266
+#: flask_security/core.py:265
 msgid "Login Required"
 msgstr "需要登录"
 
-#: flask_security/core.py:267
+#: flask_security/core.py:266
 #: flask_security/templates/security/email/two_factor_instructions.html:1
 #: flask_security/templates/security/email/two_factor_instructions.txt:1
 #: flask_security/templates/security/email/us_instructions.html:9
 #: flask_security/templates/security/email/us_instructions.txt:9
 msgid "Welcome"
 msgstr "欢迎"
 
-#: flask_security/core.py:268
+#: flask_security/core.py:267
 msgid "Please confirm your email"
 msgstr "请激活你的电子邮箱"
 
-#: flask_security/core.py:269
+#: flask_security/core.py:268
 msgid "Login instructions"
 msgstr "登录邮件"
 
-#: flask_security/core.py:270
+#: flask_security/core.py:269
 #: flask_security/templates/security/email/reset_notice.html:1
 #: flask_security/templates/security/email/reset_notice.txt:1
 msgid "Your password has been reset"
 msgstr "你的密码已重置"
 
-#: flask_security/core.py:271
+#: flask_security/core.py:270
 msgid "Your password has been changed"
 msgstr "你的密码已更改"
 
-#: flask_security/core.py:272
+#: flask_security/core.py:271
 msgid "Password reset instructions"
 msgstr "密码重置"
 
-#: flask_security/core.py:275
+#: flask_security/core.py:274
 msgid "Two-factor Login"
 msgstr "双因素认证登录"
 
-#: flask_security/core.py:276
+#: flask_security/core.py:275
 msgid "Two-factor Rescue"
 msgstr ""
 
-#: flask_security/core.py:324
+#: flask_security/core.py:323
 msgid "Verification Code"
 msgstr "验证码"
 
-#: flask_security/core.py:370
+#: flask_security/core.py:369
 msgid "Input not appropriate for requested API"
 msgstr "输入信息不适合所请求的API"
 
-#: flask_security/core.py:372
+#: flask_security/core.py:371
 msgid "Authentication failed - identity or password/passcode invalid"
 msgstr ""
 
-#: flask_security/core.py:376
+#: flask_security/core.py:375
 msgid ""
 "If that email address is in our system, you will receive an email "
 "describing how to reset your password."
 msgstr ""
 
-#: flask_security/core.py:383
+#: flask_security/core.py:382
 msgid "If that identity is in our system, you were sent a code."
 msgstr ""
 
-#: flask_security/core.py:386
+#: flask_security/core.py:385
 msgid "You do not have permission to view this resource."
 msgstr "你无权查看此资源！"
 
-#: flask_security/core.py:388
+#: flask_security/core.py:387
 msgid "You are not authenticated. Please supply the correct credentials."
 msgstr "你还没有通过认证。请提供正确的凭证。"
 
-#: flask_security/core.py:392
+#: flask_security/core.py:391
 #, fuzzy
 msgid "You must re-authenticate to access this endpoint"
 msgstr "请重新进行身份验证，以访问此页面。"
 
-#: flask_security/core.py:396
+#: flask_security/core.py:395
 #, python-format
 msgid "Thank you. Confirmation instructions have been sent to %(email)s."
 msgstr "谢谢你。已发送激活邮件到 %(email)s。"
 
-#: flask_security/core.py:399
+#: flask_security/core.py:398
 msgid "Thank you. Your email has been confirmed."
 msgstr "谢谢。你的邮箱已激活！"
 
-#: flask_security/core.py:400
+#: flask_security/core.py:399
 msgid "Your email has already been confirmed."
 msgstr "你的邮箱已激活！"
 
-#: flask_security/core.py:401
+#: flask_security/core.py:400
 msgid "Invalid confirmation token."
 msgstr "无效验证码！"
 
-#: flask_security/core.py:403
+#: flask_security/core.py:402
 #, python-format
 msgid "%(email)s is already associated with an account."
 msgstr "%(email)s 已关联账户。"
 
-#: flask_security/core.py:407
+#: flask_security/core.py:406
 #, python-format
 msgid ""
 "Identity attribute '%(attr)s' with value '%(value)s' is already "
 "associated with an account."
 msgstr ""
 
-#: flask_security/core.py:414
+#: flask_security/core.py:413
 #, python-format
 msgid "Identity %(id)s not registered"
 msgstr ""
 
-#: flask_security/core.py:418
+#: flask_security/core.py:417
 msgid ""
 "An error occurred while communicating with the Oauth provider. Please try"
 " again."
 msgstr ""
 
-#: flask_security/core.py:424
+#: flask_security/core.py:423
 msgid "Password does not match"
 msgstr "密码不匹配"
 
-#: flask_security/core.py:425
+#: flask_security/core.py:424
 msgid "Passwords do not match"
 msgstr "密码不匹配"
 
-#: flask_security/core.py:426
+#: flask_security/core.py:425
 msgid "Redirections outside the domain are forbidden"
 msgstr "禁止域名外重定向"
 
-#: flask_security/core.py:427
+#: flask_security/core.py:426
 msgid "Recovery code invalid"
 msgstr ""
 
-#: flask_security/core.py:428
+#: flask_security/core.py:427
 msgid "No recovery codes generated yet"
 msgstr ""
 
-#: flask_security/core.py:430
+#: flask_security/core.py:429
 #, python-format
 msgid "Instructions to reset your password have been sent to %(email)s."
 msgstr "重置密码邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:434
+#: flask_security/core.py:433
 #, python-format
 msgid ""
 "You did not reset your password within %(within)s. New instructions have "
 "been sent to %(email)s."
 msgstr "你未在 %(within)s 重置密码。新重置密码邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:440
+#: flask_security/core.py:439
 msgid "Invalid reset password token."
 msgstr "密码重置验证码无效！"
 
-#: flask_security/core.py:441
+#: flask_security/core.py:440
 msgid "Email requires confirmation."
 msgstr "请先激活邮箱。"
 
-#: flask_security/core.py:443
+#: flask_security/core.py:442
 #, python-format
 msgid "Confirmation instructions have been sent to %(email)s."
 msgstr "激活邮件已发送到  %(email)s。"
 
-#: flask_security/core.py:447
+#: flask_security/core.py:446
 #, python-format
 msgid ""
 "You did not confirm your email within %(within)s. New instructions to "
 "confirm your email have been sent to %(email)s."
 msgstr "你未在 %(within)s 激活邮箱。新激活邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:455
+#: flask_security/core.py:454
 #, python-format
 msgid ""
 "You did not login within %(within)s. New instructions to login have been "
 "sent to %(email)s."
 msgstr "你未在 %(within)s 登录账户。新登录邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:462
+#: flask_security/core.py:461
 #, python-format
 msgid "Instructions to login have been sent to %(email)s."
 msgstr "登录邮件已发送到 %(email)s。"
 
-#: flask_security/core.py:465
+#: flask_security/core.py:464
 msgid "Invalid login token."
 msgstr "无效登录验证码！"
 
-#: flask_security/core.py:466
+#: flask_security/core.py:465
 msgid "Account is disabled."
 msgstr "账户已被禁用！"
 
-#: flask_security/core.py:467
+#: flask_security/core.py:466
 msgid "Email not provided"
 msgstr "未填写电子邮箱"
 
-#: flask_security/core.py:468
+#: flask_security/core.py:467
 msgid "Invalid email address"
 msgstr "无效邮箱地址"
 
-#: flask_security/core.py:469 flask_security/core.py:508
+#: flask_security/core.py:468 flask_security/core.py:507
 #, fuzzy
 msgid "Invalid code"
 msgstr "密码不正确"
 
-#: flask_security/core.py:470
+#: flask_security/core.py:469
 msgid "Password not provided"
 msgstr "未填写密码"
 
-#: flask_security/core.py:472
+#: flask_security/core.py:471
 #, python-format
 msgid "Password must be at least %(length)s characters"
 msgstr "密码至少包含%(length)s个字符"
 
-#: flask_security/core.py:475
+#: flask_security/core.py:474
 msgid "Password not complex enough"
 msgstr "密码不够复杂"
 
-#: flask_security/core.py:476
+#: flask_security/core.py:475
 msgid "Password on breached list"
 msgstr "密码在易被泄露名单上"
 
-#: flask_security/core.py:478
+#: flask_security/core.py:477
 msgid "Failed to contact breached passwords site"
 msgstr "未能连通检测易泄露密码的网站"
 
-#: flask_security/core.py:481
+#: flask_security/core.py:480
 msgid "Phone number not valid e.g. missing country code"
 msgstr "手机号码非法。例如: 缺少国家代码"
 
-#: flask_security/core.py:482
+#: flask_security/core.py:481
 msgid "Specified user does not exist"
 msgstr "此用户不存在"
 
-#: flask_security/core.py:483
+#: flask_security/core.py:482
 msgid "Invalid password"
 msgstr "密码不正确"
 
-#: flask_security/core.py:484
+#: flask_security/core.py:483
 msgid "Password or code submitted is not valid"
 msgstr "提交的密码或代码无效"
 
-#: flask_security/core.py:485
+#: flask_security/core.py:484
 msgid "You have successfully logged in."
 msgstr "你已成功登录！"
 
-#: flask_security/core.py:486
+#: flask_security/core.py:485
 msgid "Forgot password?"
 msgstr "忘记密码？"
 
-#: flask_security/core.py:488
+#: flask_security/core.py:487
 msgid ""
 "You successfully reset your password and you have been logged in "
 "automatically."
 msgstr "你的密码已成功重置，并已自动登录。"
 
-#: flask_security/core.py:495
+#: flask_security/core.py:494
 msgid "Your new password must be different than your previous password."
 msgstr "你的新密码不能与当前密码相同。"
 
-#: flask_security/core.py:498
+#: flask_security/core.py:497
 msgid "You successfully changed your password."
 msgstr "你已成功更改密码！"
 
-#: flask_security/core.py:499
+#: flask_security/core.py:498
 msgid "Please log in to access this page."
 msgstr "请登录访问此页面。"
 
-#: flask_security/core.py:500
+#: flask_security/core.py:499
 msgid "Please reauthenticate to access this page."
 msgstr "请重新进行身份验证，以访问此页面。"
 
-#: flask_security/core.py:501
+#: flask_security/core.py:500
 msgid "Reauthentication successful"
 msgstr "成功进行重新认证"
 
-#: flask_security/core.py:503
+#: flask_security/core.py:502
 msgid "You can only access this endpoint when not logged in."
 msgstr "您只能在未登录时访问此端点。"
 
-#: flask_security/core.py:506
+#: flask_security/core.py:505
 msgid "Code has been sent."
 msgstr ""
 
-#: flask_security/core.py:507
+#: flask_security/core.py:506
 msgid "Failed to send code. Please try again later"
 msgstr "发送代码失败。请稍后再试"
 
-#: flask_security/core.py:509
+#: flask_security/core.py:508
 msgid "Your code has been confirmed"
 msgstr ""
 
-#: flask_security/core.py:511
+#: flask_security/core.py:510
 msgid "You successfully changed your two-factor method."
 msgstr "你成功改变了你的双因素验证方法。"
 
-#: flask_security/core.py:515
+#: flask_security/core.py:514
 msgid "You currently do not have permissions to access this page"
 msgstr "你现在还没有权限访问这个页面"
 
-#: flask_security/core.py:518
+#: flask_security/core.py:517
 msgid "Marked method is not valid"
 msgstr "选择的方法无效"
 
-#: flask_security/core.py:520
+#: flask_security/core.py:519
 msgid "You successfully disabled two factor authorization."
 msgstr "你成功地禁用了双因素授权。"
 
-#: flask_security/core.py:523
+#: flask_security/core.py:522
 msgid "Requested method is not valid"
 msgstr "非法的请求方法"
 
-#: flask_security/core.py:525
+#: flask_security/core.py:524
 #, python-format
 msgid "Setup must be completed within %(within)s. Please start over."
 msgstr "必须在%(within)s内完成设置。请重新开始。"
 
-#: flask_security/core.py:528
+#: flask_security/core.py:527
 msgid "Unified sign in setup successful"
 msgstr "统一登录设置成功"
 
-#: flask_security/core.py:529
+#: flask_security/core.py:528
 msgid "You must specify a valid identity to sign in"
 msgstr "您必须指定一个有效的身份才能登录"
 
-#: flask_security/core.py:530
+#: flask_security/core.py:529
 #, python-format
 msgid "Use this code to sign in: %(code)s."
 msgstr "使用此代码登录：%(code)s"
 
-#: flask_security/core.py:532
+#: flask_security/core.py:531
 #, python-format
 msgid ""
 "Username must be at least %(min)d characters and less than %(max)d "
 "characters"
 msgstr ""
 
-#: flask_security/core.py:539
+#: flask_security/core.py:538
 msgid "Username contains illegal characters"
 msgstr ""
 
-#: flask_security/core.py:543
+#: flask_security/core.py:542
 msgid "Username can contain only letters and numbers"
 msgstr ""
 
-#: flask_security/core.py:546
+#: flask_security/core.py:545
 msgid "Username not provided"
 msgstr ""
 
-#: flask_security/core.py:548
+#: flask_security/core.py:547
 #, python-format
 msgid "%(username)s is already associated with an account."
 msgstr ""
 
-#: flask_security/core.py:552
+#: flask_security/core.py:551
 #, python-format
 msgid "WebAuthn operation must be completed within %(within)s. Please start over."
 msgstr ""
 
-#: flask_security/core.py:556
+#: flask_security/core.py:555
 msgid "Nickname for new credential is required."
 msgstr ""
 
-#: flask_security/core.py:560
+#: flask_security/core.py:559
 #, python-format
 msgid "%(name)s is already associated with a credential."
 msgstr ""
 
-#: flask_security/core.py:564
+#: flask_security/core.py:563
 #, python-format
 msgid "%(name)s not registered with current user."
 msgstr ""
 
-#: flask_security/core.py:568
+#: flask_security/core.py:567
 #, python-format
 msgid "Successfully deleted WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:572
+#: flask_security/core.py:571
 #, python-format
 msgid "Successfully added WebAuthn credential with name: %(name)s"
 msgstr ""
 
-#: flask_security/core.py:576
+#: flask_security/core.py:575
 msgid "WebAuthn credential id already registered."
 msgstr ""
 
-#: flask_security/core.py:580
+#: flask_security/core.py:579
 msgid "Unregistered WebAuthn credential id."
 msgstr ""
 
-#: flask_security/core.py:584
+#: flask_security/core.py:583
 msgid "WebAuthn credential doesn't belong to any user."
 msgstr ""
 
-#: flask_security/core.py:588
+#: flask_security/core.py:587
 #, python-format
 msgid "Could not verify WebAuthn credential: %(cause)s."
 msgstr ""
 
-#: flask_security/core.py:592
+#: flask_security/core.py:591
 msgid "Credential not registered for this use (first or secondary)"
 msgstr ""
 
-#: flask_security/core.py:596
+#: flask_security/core.py:595
 msgid "Credential user handle didn't match"
 msgstr ""
 
 #: flask_security/forms.py:58
 msgid "Email Address"
 msgstr "邮箱地址"
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/twofactor.py` & `Flask-Security-Too-5.2.0/flask_security/twofactor.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/unified_signin.py` & `Flask-Security-Too-5.2.0/flask_security/unified_signin.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/username_util.py` & `Flask-Security-Too-5.2.0/flask_security/username_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/utils.py` & `Flask-Security-Too-5.2.0/flask_security/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
     flask_security.utils
     ~~~~~~~~~~~~~~~~~~~~
 
     Flask-Security utils module
 
     :copyright: (c) 2012-2019 by Matt Wright.
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 import abc
 import base64
 import datetime
 from functools import partial
 import hashlib
 import hmac
-from pkg_resources import parse_version
 import time
 import typing as t
 from urllib.parse import parse_qsl, parse_qs, urlsplit, urlunsplit, urlencode
 import urllib.request
 import urllib.error
 import warnings
 
@@ -36,15 +35,14 @@
 from flask_login import logout_user as _logout_user
 from flask_login import current_user
 from flask_login import COOKIE_NAME as REMEMBER_COOKIE_NAME
 from flask_principal import AnonymousIdentity, Identity, identity_changed, Need
 from flask_wtf import csrf
 from wtforms import ValidationError
 from itsdangerous import BadSignature, SignatureExpired
-from werkzeug import __version__ as werkzeug_version
 from werkzeug.local import LocalProxy
 
 from .quart_compat import best, get_quart_status
 from .proxies import _security, _datastore, _pwd_context, _hashing_context
 from .signals import user_authenticated
 
 if t.TYPE_CHECKING:  # pragma: no cover
@@ -922,18 +920,15 @@
         if has_remember_cookie and current_user.is_authenticated:
             op = "set"
         else:
             return response
 
     if op == "clear":
         # Alas delete_cookie only accepts some of the keywords set_cookie does
-        # and Werkzeug didn't accept samesite, secure, httponly until 2.0
         allowed = ["path", "domain", "secure", "httponly", "samesite"]
-        if parse_version(werkzeug_version) < parse_version("2.0.0"):  # pragma: no cover
-            allowed = ["path", "domain"]
         args = {k: csrf_cookie.get(k) for k in allowed if k in csrf_cookie}
         response.delete_cookie(csrf_cookie_name, **args)
         session.pop("fs_cc")
         return response
 
     # Send a cookie if any of:
     # 1) CSRF_COOKIE_REFRESH_EACH_REQUEST is true
```

### Comparing `Flask-Security-Too-5.1.2/flask_security/views.py` & `Flask-Security-Too-5.2.0/flask_security/views.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/webauthn.py` & `Flask-Security-Too-5.2.0/flask_security/webauthn.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/flask_security/webauthn_util.py` & `Flask-Security-Too-5.2.0/flask_security/webauthn_util.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/pytest.ini` & `Flask-Security-Too-5.2.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     passwordless
     trackable
     unified_signin
     webauthn
 
 filterwarnings =
     error
-    ignore:.*'app.json_encoder' is deprecated.*:DeprecationWarning:flask:0
-    ignore:.*Setting 'json_encoder'.*:DeprecationWarning:flask:0
-    ignore:.*'JSONEncoder'.*:DeprecationWarning:flask:0
+    ignore:.*'locked_cached_property'.*:DeprecationWarning:flask:0
+    ignore:.*'flask.Markup'.*:DeprecationWarning:flask:0
     ignore::DeprecationWarning:mongoengine:
+    ignore::DeprecationWarning:flask_login:0
     ignore:.*passwordless feature.*:DeprecationWarning:flask_security:0
     ignore:.*passing settings to bcrypt.*:DeprecationWarning:passlib:0
     ignore:.*'crypt' is deprecated.*:DeprecationWarning:passlib:0
+    ignore:.*pkg_resources is deprecated.*:DeprecationWarning:pkg_resources:0
     ignore:.*'sms' was enabled in SECURITY_US_ENABLED_METHODS;.*:UserWarning:flask_security:0
     ignore:.*'get_token_status' is deprecated.*:DeprecationWarning:flask_security:0
```

### Comparing `Flask-Security-Too-5.1.2/setup.cfg` & `Flask-Security-Too-5.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,38 @@
 [options.extras_require]
 babel = 
-	babel>=2.10.0
-	flask_babel>=2.0.0
+	babel>=2.12.1
+	flask_babel>=3.1.0
 fsqla = 
 	flask_sqlalchemy>=3.0.2
 	sqlalchemy>=1.4.35
 	sqlalchemy-utils>=0.38.3
 common = 
 	bcrypt>=4.0.1
 	flask_mailman>=0.3.0
-	bleach>=5.0.0
+	bleach>=6.0.0
 mfa = 
-	cryptography>=37.0.4
-	qrcode>=7.3.1
-	phonenumberslite>=8.12.18
-	webauthn>=1.6.0
+	cryptography>=40.0.2
+	qrcode>=7.4.2
+	phonenumberslite>=8.13.11
+	webauthn>=1.8.0
 
 [aliases]
 test = pytest
 
 [bdist_wheel]
 universal = 1
 
-[build_sphinx]
-source-dir = docs/
-build-dir = docs/_build
-warning-is-error = 1
-
-[upload_sphinx]
-upload-dir = docs/_build/html
-
 [compile_catalog]
 directory = flask_security/translations/
 domain = flask_security
 
 [extract_messages]
 project = Flask-Security
-version = 5.1.0
+version = 5.2.0
 msgid_bugs_address = jwag956@github.com
 mapping-file = babel.ini
 output-file = flask_security/translations/flask_security.pot
 add-comments = NOTE
 keywords = _fsdomain
 
 [init_catalog]
```

### Comparing `Flask-Security-Too-5.1.2/setup.py` & `Flask-Security-Too-5.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 with open("README.rst", encoding="utf8") as f:
     readme = f.read()
 
 with open("flask_security/__init__.py", encoding="utf8") as f:
     version = re.search(r'__version__ = "(.*?)"', f.read()).group(1)
 
 install_requires = [
-    "Flask>=2.1.0,<2.3",
-    "Flask-Login>=0.6.0",
+    # flask dependencies include werkzeug, jinja2, itsdangerous, click, blinker
+    "Flask>=2.3.0",
+    "Flask-Login>=0.6.2",
     "Flask-Principal>=0.4.0",
-    "Flask-WTF>=1.0.0",
+    "Flask-WTF>=1.1.1",
     "email-validator>=1.1.1",
-    "itsdangerous>=2.1.0",
     "passlib>=1.7.4",
-    "blinker>=1.4",
     "wtforms>=3.0.0",  # for form-level errors
-    "setuptools",  # for pkg_resources
+    "importlib_resources>=5.10.0",
 ]
 
 packages = find_packages(exclude=["tests"])
 
 setup(
     name="Flask-Security-Too",
     version=version,
@@ -40,27 +39,26 @@
         "Code": "https://github.com/Flask-Middleware/flask-security",
         "Issue tracker": "https://github.com/Flask-Middleware/flask-security/issues",
     },
     packages=packages,
     zip_safe=False,
     include_package_data=True,
     platforms="any",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Flask",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Development Status :: 5 - Production/Stable",
```

### Comparing `Flask-Security-Too-5.1.2/tests/conftest.py` & `Flask-Security-Too-5.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/templates/_nav.html` & `Flask-Security-Too-5.2.0/tests/templates/_nav.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/templates/register.html` & `Flask-Security-Too-5.2.0/tests/templates/register.html`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_changeable.py` & `Flask-Security-Too-5.2.0/tests/test_changeable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     test_changeable
     ~~~~~~~~~~~~~~~
 
     Changeable tests
 
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 
 import base64
 
 import pytest
 from flask import Flask
@@ -220,16 +220,16 @@
         follow_redirects=True,
     )
 
     # Should have received a new session cookie - so should still be logged in
     response = client.get("/profile", follow_redirects=True)
     assert b"Profile Page" in response.data
 
-    assert "remember_token" in [c.name for c in client.cookie_jar]
-    client.cookie_jar.clear_session_cookies()
+    assert client.get_cookie("remember_token")
+    client.delete_cookie("session")
     response = client.get("/profile", follow_redirects=True)
     assert b"Profile Page" in response.data
 
 
 def test_change_invalidates_auth_token(app, client):
     # if change password, by default that should invalidate auth tokens
     response = json_authenticate(client)
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_cli.py` & `Flask-Security-Too-5.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_common.py` & `Flask-Security-Too-5.2.0/tests/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
     test_common
     ~~~~~~~~~~~
 
     Test common functionality
 
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 
 import base64
 import json
 import re
-from http.cookiejar import Cookie
 import pytest
 
 from flask import Blueprint
 
 from flask_security import uia_email_mapper
 
 from tests.test_utils import (
@@ -74,15 +73,15 @@
     response = client.post("/login?next=http:///google.com", data=data)
     assert get_message("INVALID_REDIRECT") in response.data
 
 
 def test_login_template_next(client):
     # Test that our login template propagates next.
     response = client.get("/profile", follow_redirects=True)
-    assert "?next=%2Fprofile" in response.request.url
+    assert "?next=/profile" in response.request.url
     login_url = get_form_action(response)
     response = client.post(
         login_url,
         data=dict(email="matt@lp.com", password="password"),
         follow_redirects=True,
     )
     assert b"Profile Page" in response.data
@@ -740,41 +739,21 @@
 
     response = client.get("/")
     assert b"Hello matt@lp.com" not in response.data
 
 
 def test_remember_token(client):
     response = authenticate(client, follow_redirects=False)
-    client.cookie_jar.clear_session_cookies()
+    client.delete_cookie("session")
     response = client.get("/profile")
     assert b"profile" in response.data
 
 
 def test_request_loader_does_not_fail_with_invalid_token(client):
-    c = Cookie(
-        version=0,
-        name="remember_token",
-        value="None",
-        port=None,
-        port_specified=False,
-        domain="www.example.com",
-        domain_specified=False,
-        domain_initial_dot=False,
-        path="/",
-        path_specified=True,
-        secure=False,
-        expires=None,
-        discard=True,
-        comment=None,
-        comment_url=None,
-        rest={"HttpOnly": None},
-        rfc2109=False,
-    )
-
-    client.cookie_jar.set_cookie(c)
+    client.set_cookie("remember_token")
     response = client.get("/")
     assert b"BadSignature" not in response.data
 
 
 def test_sending_auth_token_with_json(client):
     response = json_authenticate(client)
     token = response.json["response"]["user"]["authentication_token"]
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_configuration.py` & `Flask-Security-Too-5.2.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_confirmable.py` & `Flask-Security-Too-5.2.0/tests/test_confirmable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_context_processors.py` & `Flask-Security-Too-5.2.0/tests/test_context_processors.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_csrf.py` & `Flask-Security-Too-5.2.0/tests/test_csrf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     test_csrf
     ~~~~~~~~~~~~~~~~~
 
     CSRF tests
 
-    :copyright: (c) 2019-2020 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 """
 from contextlib import contextmanager
 import time
 
 import flask_wtf.csrf
 
@@ -430,27 +430,20 @@
     app.config["WTF_CSRF_CHECK_DEFAULT"] = False
     CSRFProtect(app)
     app.security = Security(app=app, datastore=sqlalchemy_datastore)
     create_user(app)
 
     client = app.test_client()
     json_login(client)
-    found = False
-    for cookie in client.cookie_jar:
-        if cookie.name == "XSRF-Token":
-            found = True
-            assert cookie.path == "/"
-            # Alas http.cookiejar doesn't support samesite...
-            # assert cookie.samesite == "Strict"
-    assert found
+    assert client.get_cookie("XSRF-Token")
 
     # Make sure cleared on logout
     response = client.post("/logout", content_type="application/json")
     assert response.status_code == 200
-    assert "XSRF-Token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("XSRF-Token")
 
 
 @pytest.mark.settings(CSRF_COOKIE={"key": "XSRF-Token"})
 @pytest.mark.changeable()
 def test_cp_with_token_cookie(app, sqlalchemy_datastore):
     # Make sure can use returned CSRF-Token cookie in Header when changing password.
     app.config["WTF_CSRF_ENABLED"] = True
@@ -464,26 +457,26 @@
 
     # make sure returned csrf_token works in header.
     data = dict(
         password="password",
         new_password="battery staple",
         new_password_confirm="battery staple",
     )
-    csrf_token = [c.value for c in client.cookie_jar if c.name == "XSRF-Token"][0]
+    csrf_token = client.get_cookie("XSRF-Token")
     with mp_validate_csrf() as mp:
         response = client.post(
             "/change",
             content_type="application/json",
             json=data,
-            headers={"X-XSRF-Token": csrf_token},
+            headers={"X-XSRF-Token": csrf_token.value},
         )
         assert response.status_code == 200
     assert mp.success == 1 and mp.failure == 0
     json_logout(client)
-    assert "XSRF-Token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("XSRF-Token")
 
 
 @pytest.mark.settings(CSRF_COOKIE_NAME="XSRF-Token", csrf_ignore_unauth_endpoints=True)
 @pytest.mark.changeable()
 def test_cp_with_token_cookie_expire(app, sqlalchemy_datastore):
     # Make sure that we get a new Csrf-Token cookie if expired.
     app.config["WTF_CSRF_ENABLED"] = True
@@ -500,34 +493,32 @@
     # sleep so make csrf_token expires
     time.sleep(2)
     data = dict(
         password="password",
         new_password="battery staple",
         new_password_confirm="battery staple",
     )
-    csrf_token = [c.value for c in client.cookie_jar if c.name == "XSRF-Token"][0]
+    csrf_token = client.get_cookie("XSRF-Token")
     with mp_validate_csrf() as mp:
         response = client.post(
             "/change",
             content_type="application/json",
             json=data,
-            headers={"X-XSRF-Token": csrf_token},
+            headers={"X-XSRF-Token": csrf_token.value},
         )
         assert response.status_code == 400
         assert b"expired" in response.data
 
         # Should have gotten a new CSRF cookie value
-        new_csrf_token = [c.value for c in client.cookie_jar if c.name == "XSRF-Token"][
-            0
-        ]
-        assert csrf_token != new_csrf_token
+        new_csrf_token = client.get_cookie("XSRF-Token")
+        assert csrf_token.value != new_csrf_token.value
     # 2 failures since the utils:csrf_cookie_handler will check
     assert mp.success == 0 and mp.failure == 2
     json_logout(client)
-    assert "XSRF-Token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("XSRF-Token")
 
 
 @pytest.mark.settings(
     CSRF_COOKIE_NAME="XSRF-Token", CSRF_COOKIE_REFRESH_EACH_REQUEST=True
 )
 @pytest.mark.changeable()
 def test_cp_with_token_cookie_refresh(app, sqlalchemy_datastore):
@@ -544,39 +535,37 @@
     # make sure returned csrf_token works in header.
     data = dict(
         password="password",
         new_password="battery staple",
         new_password_confirm="battery staple",
     )
 
-    csrf_cookie = [c for c in client.cookie_jar if c.name == "XSRF-Token"][0]
+    csrf_cookie = client.get_cookie("XSRF-Token")
     with mp_validate_csrf() as mp:
         # Delete cookie - we should always get a new one
-        client.delete_cookie(csrf_cookie.domain, csrf_cookie.name)
+        client.delete_cookie("XSRF-Token")
         response = client.post(
             "/change",
             content_type="application/json",
             json=data,
             headers={"X-XSRF-Token": csrf_cookie.value},
         )
         assert response.status_code == 200
-        csrf_cookie = [c for c in client.cookie_jar if c.name == "XSRF-Token"][0]
-        assert csrf_cookie
+        assert client.get_cookie("XSRF-Token")
     assert mp.success == 1 and mp.failure == 0
 
     # delete cookie again, do a 'GET' - the REFRESH_COOKIE_ON_EACH_REQUEST should
     # send us a new one
-    client.delete_cookie(csrf_cookie.domain, csrf_cookie.name)
+    client.delete_cookie("XSRF-Token")
     response = client.get("/change")
     assert response.status_code == 200
-    csrf_cookie = [c for c in client.cookie_jar if c.name == "XSRF-Token"][0]
-    assert csrf_cookie
+    assert client.get_cookie("XSRF-Token")
 
     json_logout(client)
-    assert "XSRF-Token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("XSRF-Token")
 
 
 @pytest.mark.settings(CSRF_COOKIE_NAME="XSRF-Token")
 @pytest.mark.changeable()
 def test_remember_login_csrf_cookie(app, sqlalchemy_datastore):
     # Test csrf cookie upon resuming a remember session
     app.config["WTF_CSRF_ENABLED"] = True
@@ -585,24 +574,26 @@
     create_user(app)
 
     client = app.test_client()
 
     # Login with remember_token generation
     json_login(client, use_header=True, remember=True)
 
-    csrf_cookie = [c for c in client.cookie_jar if c.name == "XSRF-Token"][0]
-    session_cookie = [c for c in client.cookie_jar if c.name == "session"][0]
+    # csrf_cookie = [c for c in client.cookie_jar if c.name == "XSRF-Token"][0]
+    # session_cookie = [c for c in client.cookie_jar if c.name == "session"][0]
     # Delete session and csrf cookie - we should always get new ones
-    client.delete_cookie(csrf_cookie.domain, csrf_cookie.name)
-    client.delete_cookie(session_cookie.domain, session_cookie.name)
+    # client.delete_cookie(csrf_cookie.domain, csrf_cookie.name)
+    # client.delete_cookie(session_cookie.domain, session_cookie.name)
+    client.delete_cookie("XSRF-Token")
+    client.delete_cookie("session")
 
     # Do a simple get request with the remember_token cookie present
-    assert "remember_token" in [c.name for c in client.cookie_jar]
+    assert client.get_cookie("remember_token")
     response = client.get("/profile")
     assert response.status_code == 200
-    assert "session" in [c.name for c in client.cookie_jar]
-    assert "XSRF-Token" in [c.name for c in client.cookie_jar]
+    assert client.get_cookie("session")
+    assert client.get_cookie("XSRF-Token")
     # Logout and check that everything cleans up nicely
     json_logout(client)
-    assert "remember_token" not in [c.name for c in client.cookie_jar]
-    assert "session" not in [c.name for c in client.cookie_jar]
-    assert "XSRF-Token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("remember_token")
+    assert not client.get_cookie("session")
+    assert not client.get_cookie("XSRF-Token")
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_datastore.py` & `Flask-Security-Too-5.2.0/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_entities.py` & `Flask-Security-Too-5.2.0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_hashing.py` & `Flask-Security-Too-5.2.0/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_misc.py` & `Flask-Security-Too-5.2.0/tests/test_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 
 from datetime import timedelta
 import hashlib
 from unittest import mock
 import re
 import os.path
-import pkg_resources
 import sys
 import time
 import typing as t
 
 import pytest
 
 from wtforms.validators import DataRequired, Length
@@ -631,23 +630,39 @@
 
 
 @pytest.mark.babel()
 @pytest.mark.app_settings(babel_default_locale="fr_FR")
 def test_myxlation(app, sqlalchemy_datastore, pytestconfig):
     # Test changing a single MSG and having an additional translation dir
     # Flask-BabelEx doesn't support lists of directories..
-    try:
-        import flask_babelex  # noqa: F401
+    pytest.importorskip("flask_babel")
 
-        pytest.skip("Flask-BabelEx doesn't support lists of translations")
-    except ImportError:
-        pass
+    i18n_dirname = [
+        "builtin",
+        os.path.join(pytestconfig.rootdir, "tests/translations"),
+    ]
+    init_app_with_options(
+        app, sqlalchemy_datastore, **{"SECURITY_I18N_DIRNAME": i18n_dirname}
+    )
 
+    assert check_xlation(app, "fr_FR"), "You must run python setup.py compile_catalog"
+
+    app.config["SECURITY_MSG_INVALID_PASSWORD"] = ("Password no-worky", "error")
+
+    client = app.test_client()
+    response = client.post("/login", data=dict(email="matt@lp.com", password="forgot"))
+    assert b"Passe - no-worky" in response.data
+
+
+@pytest.mark.babel()
+@pytest.mark.app_settings(babel_default_locale="fr_FR")
+def test_myxlation_complete(app, sqlalchemy_datastore, pytestconfig):
+    # Test having own translations and not using builtin.
+    pytest.importorskip("flask_babel")
     i18n_dirname = [
-        pkg_resources.resource_filename("flask_security", "translations"),
         os.path.join(pytestconfig.rootdir, "tests/translations"),
     ]
     init_app_with_options(
         app, sqlalchemy_datastore, **{"SECURITY_I18N_DIRNAME": i18n_dirname}
     )
 
     assert check_xlation(app, "fr_FR"), "You must run python setup.py compile_catalog"
@@ -965,17 +980,15 @@
     assert response.status_code == 200
 
     # This should require additional authn and redirect to verify
     time.sleep(0.1)
     with capture_flashes() as flashes:
         response = client.get("/myspecialview", follow_redirects=False)
         assert response.status_code == 302
-        assert (
-            "/verify?next=http%3A%2F%2Flocalhost%2Fmyspecialview" in response.location
-        )
+        assert "/verify?next=http://localhost/myspecialview" in response.location
     assert flashes[0]["category"] == "error"
     assert flashes[0]["message"].encode("utf-8") == get_message(
         "REAUTHENTICATION_REQUIRED"
     )
 
     # Test json error response
     response = client.get("/myspecialview", headers={"accept": "application/json"})
@@ -1047,15 +1060,15 @@
     app.add_url_rule("/myview", view_func=myview, methods=["GET"])
     authenticate(client, endpoint="/myprefix/login")
 
     # This should require additional authn and redirect to verify
     reset_fresh(client, within=timedelta(minutes=1))
     response = client.get("/myview", follow_redirects=False)
     assert response.status_code == 302
-    assert "/myprefix/verify?next=http%3A%2F%2Flocalhost%2Fmyview" in response.location
+    assert "/myprefix/verify?next=http://localhost/myview" in response.location
 
 
 def test_authn_freshness_grace(app, client, get_message):
     # Test that grace override within.
     @auth_required(within=lambda: timedelta(minutes=30), grace=10)
     def myview():
         return Response(status=200)
@@ -1089,15 +1102,15 @@
     response = json_authenticate(client_nc)
     token = response.json["response"]["user"]["authentication_token"]
     h = {"Authentication-Token": token}
 
     # This should fail - should be a redirect
     response = client_nc.get("/myview", headers=h, follow_redirects=False)
     assert response.status_code == 302
-    assert "/verify?next=http%3A%2F%2Flocalhost%2Fmyview" in response.location
+    assert "/verify?next=http://localhost/myview" in response.location
 
 
 def test_verify_fresh(app, client, get_message):
     # Hit a fresh-required endpoint and walk through verify
     authenticate(client)
     reset_fresh(client, app.config["SECURITY_FRESHNESS"])
 
@@ -1198,22 +1211,14 @@
     response = client.post(
         "/auth/?next=http://localhost/mynext",
         data=dict(password="password"),
         follow_redirects=False,
     )
     assert response.location == "http://localhost/mynext"
 
-    response = client.post(
-        "/auth/?next=http%3A%2F%2F127.0.0.1%3A5000%2Fdashboard%2Fsettings%2F",
-        data=dict(password="password"),
-        follow_redirects=False,
-        base_url="http://127.0.0.1:5000",
-    )
-    assert response.location == "http://127.0.0.1:5000/dashboard/settings/"
-
 
 @pytest.mark.webauthn()
 @pytest.mark.settings(webauthn_util_cls=HackWebauthnUtil)
 def test_verify_wan(app, client, get_message):
     # test get correct options when requiring a reauthentication and have wan keys
     # setup.
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_oauthglue.py` & `Flask-Security-Too-5.2.0/tests/test_oauthglue.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_passwordless.py` & `Flask-Security-Too-5.2.0/tests/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_recoverable.py` & `Flask-Security-Too-5.2.0/tests/test_recoverable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_recovery_codes.py` & `Flask-Security-Too-5.2.0/tests/test_recovery_codes.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_registerable.py` & `Flask-Security-Too-5.2.0/tests/test_registerable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_response.py` & `Flask-Security-Too-5.2.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_tf_plugin.py` & `Flask-Security-Too-5.2.0/tests/test_tf_plugin.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_trackable.py` & `Flask-Security-Too-5.2.0/tests/test_trackable.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tests/test_two_factor.py` & `Flask-Security-Too-5.2.0/tests/test_two_factor.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,33 +84,30 @@
         ]
     )
 
 
 @pytest.mark.settings(two_factor_always_validate=False)
 def test_always_validate(app, client):
     tf_authenticate(app, client, remember=True)
-    cookie = next(
-        (cookie for cookie in client.cookie_jar if cookie.name == "tf_validity"), None
-    )
-    assert cookie is not None
+    assert client.get_cookie("tf_validity")
 
     logout(client)
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
     assert b"Welcome gal@lp.com" in response.data
     assert response.status_code == 200
 
     logout(client)
     data = dict(email="gal2@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
     assert b"Please enter your authentication code" in response.data
 
     # make sure the cookie doesn't affect the JSON request
-    client.cookie_jar.clear("localhost.local", "/", "tf_validity")
+    client.delete_cookie("tf_validity")
     # Test JSON
     token = tf_authenticate(app, client, json=True, remember=True)
     logout(client)
     data = dict(email="gal@lp.com", password="password", tf_validity_token=token)
     response = client.post(
         "/login",
         json=data,
@@ -203,15 +200,15 @@
         app.security.datastore.commit()
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
 
     assert b"Please enter your authentication code" in response.data
 
-    client.cookie_jar.clear("localhost.local", "/", "tf_validity")
+    client.delete_cookie("tf_validity")
     # Test JSON
     token = tf_authenticate(app, client, json=True, remember=True)
     logout(client)
     with app.app_context():
         user = app.security.datastore.find_user(email="gal@lp.com")
         app.security.datastore.set_uniquifier(user)
         app.security.datastore.commit()
@@ -238,15 +235,15 @@
         app.security.datastore.commit()
 
     data = dict(email="gal@lp.com", password="password")
     response = client.post("/login", data=data, follow_redirects=True)
 
     assert b"Two-factor authentication adds an extra layer of security" in response.data
 
-    client.cookie_jar.clear("localhost.local", "/", "tf_validity")
+    client.delete_cookie("tf_validity")
     # Test JSON
     token = tf_authenticate(app, client, json=True, remember=True, validate=False)
     logout(client)
     with app.app_context():
         user = app.security.datastore.find_user(email="gal@lp.com")
         app.security.datastore.reset_user_access(user)
         app.security.datastore.commit()
@@ -436,35 +433,30 @@
     code = totp.generate().token
     response = client.post("/tf-validate", data=dict(code=code), follow_redirects=True)
     assert b"You successfully changed your two-factor method" in response.data
 
     logout(client)
 
     # Test login with remember_token
-    assert "remember_token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("remember_token")
     data = dict(email="gal@lp.com", password="password", remember=True)
     response = client.post(
         "/login",
         json=data,
         headers={"Content-Type": "application/json"},
         follow_redirects=True,
     )
 
     # Generate token from passed totp_secret
     code = totp.generate().token
     response = client.post("/tf-validate", data=dict(code=code), follow_redirects=True)
     assert get_message("TWO_FACTOR_LOGIN_SUCCESSFUL") in response.data
 
     # Verify that the remember token is properly set
-    found = False
-    for cookie in client.cookie_jar:
-        if cookie.name == "remember_token":
-            found = True
-            assert cookie.path == "/"
-    assert found
+    assert client.get_cookie("remember_token")
 
     response = logout(client)
     # Verify that logout clears session info
     assert not tf_in_session(get_session(response))
 
     # Test two-factor authentication first login
     data = dict(email="matt@lp.com", password="password")
@@ -1247,29 +1239,29 @@
 
 
 def test_propagate_next(app, client):
     # verify we propagate the ?next param all the way through a two-factor login
     with capture_send_code_requests() as codes:
         data = dict(email="gal@lp.com", password="password")
         response = client.post("/login?next=/im-in", data=data, follow_redirects=True)
-        assert "?next=%2Fim-in" in response.request.url
+        assert "?next=/im-in" in response.request.url
         # grab URL from form to show that our template propagates ?next
         verify_url = get_form_action(response)
         response = client.post(
             verify_url, data=dict(code=codes[0]["login_token"]), follow_redirects=False
         )
         assert "/im-in" in response.location
 
 
 @pytest.mark.settings(freshness=timedelta(minutes=0))
 def test_verify(app, client, get_message):
     # Test setup when re-authenticate required
     authenticate(client)
     response = client.get("tf-setup", follow_redirects=False)
-    assert "/verify?next=http%3A%2F%2Flocalhost%2Ftf-setup" in response.location
+    assert "/verify?next=http://localhost/tf-setup" in response.location
     logout(client)
 
     # Now try again - follow redirects to get to verify form
     # This call should require re-verify
     authenticate(client)
     response = client.get("tf-setup", follow_redirects=True)
     assert get_message("REAUTHENTICATION_REQUIRED") in response.data
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_unified_signin.py` & `Flask-Security-Too-5.2.0/tests/test_unified_signin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     test_unified_signin
     ~~~~~~~~~~~~~~~~~~~
 
     Unified signin tests
 
-    :copyright: (c) 2019-2022 by J. Christopher Wagner (jwag).
+    :copyright: (c) 2019-2023 by J. Christopher Wagner (jwag).
     :license: MIT, see LICENSE for more details.
 
 """
 
 import base64
 from contextlib import contextmanager
 from datetime import timedelta
@@ -189,22 +189,22 @@
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode="blahblah"),
         follow_redirects=True,
     )
     assert get_message("INVALID_PASSWORD_CODE") in response.data
 
     # Correct code
-    assert "remember_token" not in [c.name for c in clients.cookie_jar]
-    assert "session" not in [c.name for c in clients.cookie_jar]
+    assert not clients.get_cookie("remember_token")
+    assert not clients.get_cookie("session")
     response = clients.post(
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode=requests[0]["token"]),
         follow_redirects=False,
     )
-    assert "remember_token" not in [c.name for c in clients.cookie_jar]
+    assert not clients.get_cookie("remember_token")
     assert "email" in auths[0][1]
 
     response = clients.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
     logout(clients)
     response = clients.get("/profile", follow_redirects=False)
@@ -224,22 +224,22 @@
     code = sms_sender.messages[0].split()[-1].strip(".")
     response = clients.post(
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode=code, remember=True),
         follow_redirects=True,
     )
     assert response.status_code == 200
-    assert "remember_token" in [c.name for c in clients.cookie_jar]
+    assert clients.get_cookie("remember_token")
     assert "sms" in auths[1][1]
 
     response = clients.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
     logout(clients)
-    assert "remember_token" not in [c.name for c in clients.cookie_jar]
+    assert not clients.get_cookie("remember_token")
 
 
 def test_simple_signin_json(app, client_nc, get_message):
     set_email(app)
     auths = []
 
     @user_authenticated.connect_via(app)
@@ -986,15 +986,15 @@
     # Test setup when re-authenticate required
     # With  freshness set to 0 - the first call should require reauth (by
     # redirecting); but the second should work due to grace period.
     set_email(app)
     us_authenticate(client)
     response = client.get("us-setup", follow_redirects=False)
     verify_url = response.location
-    assert "/us-verify?next=http%3A%2F%2Flocalhost%2Fus-setup" in verify_url
+    assert "/us-verify?next=http://localhost/us-setup" in verify_url
     logout(client)
     us_authenticate(client)
 
     response = client.get("us-setup", follow_redirects=True)
     form_response = response.data.decode("utf-8")
     assert "Please Reauthenticate" in form_response
     send_code_url = get_form_action(response, 1)
@@ -1437,15 +1437,15 @@
 
     response = client.post(
         "/us-signin",
         data=dict(identity="matt@lp.com", passcode="password", remember=True),
         follow_redirects=True,
     )
     assert response.status_code == 200
-    assert "remember_token" in [c.name for c in client.cookie_jar]
+    assert client.get_cookie("remember_token")
     assert "password" in auths[0][1]
 
     response = client.get("/profile", follow_redirects=False)
     assert response.status_code == 200
 
 
 @pytest.mark.settings(
@@ -1815,27 +1815,23 @@
     us_tf_authenticate(app, client, remember=True)
     logout(client)
     data = dict(identity="gal@lp.com", passcode="password")
     response = client.post(
         "/us-signin", json=data, headers={"Content-Type": "application/json"}
     )
     assert b'"code": 200' in response.data
-    cookie = next(
-        (cookie for cookie in client.cookie_jar if cookie.name == "tf_validity"), None
-    )
-    assert cookie is not None
-
+    assert client.get_cookie("tf_validity")
     logout(client)
 
     data = dict(identity="gal2@lp.com", passcode="password")
     response = client.post("/us-signin", data=data, follow_redirects=True)
     assert b"Please enter your authentication code" in response.data
 
     # clear the cookie to make sure it's not picking it up with json.
-    client.cookie_jar.clear("localhost.local", "/", "tf_validity")
+    client.delete("tf_validity")
 
     token = us_tf_authenticate(app, client, remember=True, json=True)
     logout(client)
     data = dict(identity="gal@lp.com", passcode="password", tf_validity_token=token)
     response = client.post(
         "/us-signin",
         json=data,
@@ -2100,15 +2096,15 @@
 @pytest.mark.settings(url_prefix="/auth", us_signin_replaces_login=True)
 def test_propagate_next(app, client):
     # verify we propagate the ?next param all the way through a unified signin
     # Also test blueprint prefix since we rarely actually test that.
     set_phone(app)
     with capture_send_code_requests() as codes:
         response = client.get("profile", follow_redirects=True)
-        assert "?next=%2Fprofile" in response.request.url
+        assert "?next=/profile" in response.request.url
         signin_url = get_form_action(response, 0)
         sendcode_url = get_form_action(response, 1)
         response = client.post(
             sendcode_url, data=dict(identity="matt@lp.com", chosen_method="sms")
         )
         data = dict(identity="matt@lp.com", passcode=codes[0]["login_token"])
         response = client.post(signin_url, data=data, follow_redirects=False)
@@ -2122,15 +2118,15 @@
     response = client.post(
         "/auth/login", json=dict(identity="matt@lp.com", passcode="password")
     )
     sms_sender = setup_tf_sms(client, url_prefix=app.config["SECURITY_URL_PREFIX"])
     logout(client, endpoint="/auth/logout")
 
     response = client.get("/profile", follow_redirects=True)
-    assert "?next=%2Fprofile" in response.request.url
+    assert "?next=/profile" in response.request.url
     signin_url = get_form_action(response, 0)
     response = client.post(
         signin_url,
         data=dict(identity="matt@lp.com", passcode="password"),
         follow_redirects=True,
     )
     sendcode_url = get_form_action(response, 0)
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_utils.py` & `Flask-Security-Too-5.2.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,15 @@
         "/".join(filter(None, (url_prefix, "tf-validate"))), json=dict(code=code)
     )
     assert response.status_code == 200
     return sms_sender
 
 
 def get_existing_session(client):
-    cookie = next(
-        (cookie for cookie in client.cookie_jar if cookie.name == "session"), None
-    )
+    cookie = client.get_cookie("session")
     if cookie:
         serializer = URLSafeTimedSerializer("secret", serializer=TaggedJSONSerializer())
         val = serializer.loads_unsafe(cookie.value)
         return val[1]
 
 
 def reset_fresh(client, within):
```

### Comparing `Flask-Security-Too-5.1.2/tests/test_webauthn.py` & `Flask-Security-Too-5.2.0/tests/test_webauthn.py`

 * *Files 2% similar despite different names*

```diff
@@ -835,15 +835,15 @@
 @pytest.mark.two_factor()
 @pytest.mark.settings(
     webauthn_util_cls=HackWebauthnUtil, two_factor_always_validate=False
 )
 def test_tf_validity_window(app, client, get_message):
     # Test with a two-factor validity setting - we don't get re-prompted.
     authenticate(client)
-    assert "tf_validity" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("tf_validity")
     register_options, response_url = _register_start_json(client)
     client.post(response_url, json=dict(credential=json.dumps(REG_DATA1)))
     logout(client)
 
     # login - should require second factor
     response = client.post(
         "/login",
@@ -871,15 +871,15 @@
         follow_redirects=True,
     )
     assert b"Use Your WebAuthn Security Key as a Second Factor" in response.data
 
     signin_options, response_url = _signin_start(client, "matt@lp.com")
     response = client.post(response_url, json=dict(credential=json.dumps(SIGNIN_DATA1)))
     assert response.status_code == 200
-    assert "tf_validity" in [c.name for c in client.cookie_jar]
+    assert client.get_cookie("tf_validity")
     logout(client)
 
     # since we did specify 'remember' previously - should not require 2FA
     response = client.post(
         "/login",
         data=dict(email="matt@lp.com", password="password"),
         follow_redirects=True,
@@ -912,15 +912,15 @@
     signin_options, response_url = _signin_start(client, "matt@lp.com")
     response = client.post(response_url, json=dict(credential=json.dumps(SIGNIN_DATA1)))
     assert response.status_code == 200
     tf_token = response.json["response"]["tf_validity_token"]
     logout(client)
 
     # make sure the cookie doesn't affect the JSON request
-    client.cookie_jar.clear("localhost.local", "/", "tf_validity")
+    client.delete_cookie("tf_validity")
 
     # Sign in again - shouldn't require 2FA
     response = client.post(
         "/login",
         json=dict(
             email="matt@lp.com",
             password="password",
@@ -1289,15 +1289,15 @@
         response_url, data=dict(credential=json.dumps(REG_DATA1)), follow_redirects=True
     )
     assert response.status_code == 200
     assert b"testr1" in response.data
 
     old_paa = reset_fresh(client, app.config["SECURITY_FRESHNESS"])
     response = client.get("fresh")
-    assert "/verify?next=http%3A%2F%2Flocalhost%2Ffresh" in response.location
+    assert "/verify?next=http://localhost/fresh" in response.location
     signin_options, response_url = _signin_start(
         client, endpoint="wan-verify?next=/fresh"
     )
 
     response = client.post(
         response_url,
         data=dict(credential=json.dumps(SIGNIN_DATA1)),
@@ -1459,30 +1459,30 @@
     register_options, response_url = _register_start_json(
         client, name="testr3", usage="first"
     )
     response = client.post(response_url, json=dict(credential=json.dumps(REG_DATA1)))
     assert response.status_code == 200
     logout(client)
 
-    assert "remember_token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("remember_token")
 
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
 
     response = client.post(
         "wan-signin", headers=headers, json=dict(identity="matt@lp.com", remember=True)
     )
     response_url = f'wan-signin/{response.json["response"]["wan_state"]}'
     assert response.json["response"]["remember"]
 
     response = client.post(
         response_url,
         json=dict(credential=json.dumps(SIGNIN_DATA1), remember=True),
     )
-    assert "remember_token" in [c.name for c in client.cookie_jar]
-    client.cookie_jar.clear_session_cookies()
+    assert client.get_cookie("remember_token")
+    client.delete_cookie("session")
     response = client.get("/profile")
     assert b"profile" in response.data
 
 
 @pytest.mark.two_factor()
 @pytest.mark.unified_signin()
 @pytest.mark.settings(webauthn_util_cls=HackWebauthnUtil)
@@ -1490,15 +1490,15 @@
     # test that remember token properly set after secondary authn with webauthn
     authenticate(client)
     register_options, response_url = _register_start_json(client, name="testr3")
     response = client.post(response_url, json=dict(credential=json.dumps(REG_DATA1)))
     assert response.status_code == 200
     logout(client)
 
-    assert "remember_token" not in [c.name for c in client.cookie_jar]
+    assert not client.get_cookie("remember_token")
 
     # login again - should require MFA
     response = client.post(
         "/us-signin",
         json=dict(identity="matt@lp.com", passcode="password", remember=True),
     )
     assert response.status_code == 200
@@ -1508,16 +1508,16 @@
         assert session["tf_remember_login"]
 
     signin_options, response_url, _ = _signin_start_json(client, "matt@lp.com")
     response = client.post(
         response_url,
         json=dict(credential=json.dumps(SIGNIN_DATA1), remember=True),
     )
-    assert "remember_token" in [c.name for c in client.cookie_jar]
-    client.cookie_jar.clear_session_cookies()
+    assert client.get_cookie("remember_token")
+    client.delete_cookie("session")
     response = client.get("/profile")
     assert b"profile" in response.data
 
 
 @pytest.mark.settings(
     webauthn_util_cls=HackWebauthnUtil,
     wan_post_register_view="/post_register",
@@ -1638,15 +1638,15 @@
         response_url, data=dict(credential=json.dumps(REG_DATA1)), follow_redirects=True
     )
     assert response.status_code == 200
     assert get_message("WEBAUTHN_REGISTER_SUCCESSFUL", name="testr3") in response.data
     logout(client, endpoint="/auth/logout")
 
     response = client.get("profile", follow_redirects=True)
-    assert "?next=%2Fprofile" in response.request.url
+    assert "?next=/profile" in response.request.url
     # pull webauthn form action out of login_form - should have ?next=...
     webauthn_url = get_form_action(response, 1)
 
     signin_options, response_url = _signin_start(
         client, "matt@lp.com", endpoint=webauthn_url
     )
     response = client.post(
```

### Comparing `Flask-Security-Too-5.1.2/tests/view_scaffold.py` & `Flask-Security-Too-5.2.0/tests/view_scaffold.py`

 * *Files identical despite different names*

### Comparing `Flask-Security-Too-5.1.2/tox.ini` & `Flask-Security-Too-5.2.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{37,38,39,310,311,py39}-{low,release}
+    py{38,39,310,311,py39}-{low,release}
     mypy
     nowebauthn
     nobabel
     noauthlib
     style
     docs
     coverage
@@ -14,22 +14,22 @@
 [testenv:pypy39-release]
 deps =
     -r requirements/tests.txt
 commands =
     python setup.py compile_catalog
     pytest -W ignore --basetemp={envtmpdir} {posargs:tests}
 
-[testenv:py{37,38,39,310,311}-release]
+[testenv:py{38,39,310,311}-release]
 deps =
     -r requirements/tests.txt
 commands =
     python setup.py compile_catalog
     pytest --basetemp={envtmpdir} {posargs:tests}
 
-[testenv:py{37,38,39,310,311,py39}-low]
+[testenv:py{38,39,310,311,py39}-low]
 deps =
     pytest
     -r requirements_low/tests.txt
 commands =
     python setup.py compile_catalog
     pytest -W ignore --basetemp={envtmpdir} {posargs:tests}
```

