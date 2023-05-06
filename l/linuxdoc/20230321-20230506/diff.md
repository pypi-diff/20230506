# Comparing `tmp/linuxdoc-20230321.tar.gz` & `tmp/linuxdoc-20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxdoc-20230321.tar", last modified: Tue Mar 21 16:23:57 2023, max compression
+gzip compressed data, was "linuxdoc-20230506.tar", last modified: Sat May  6 08:55:08 2023, max compression
```

## Comparing `linuxdoc-20230321.tar` & `linuxdoc-20230506.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-03-21 16:23:57.771566 linuxdoc-20230321/
--rw-rw-r--   0 markus   (10001) markus   (10001)    34520 2023-02-18 16:34:18.000000 linuxdoc-20230321/LICENSE
--rw-rw-r--   0 markus   (10001) markus   (10001)     1931 2023-03-21 16:23:57.771566 linuxdoc-20230321/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)      997 2023-03-21 16:22:52.000000 linuxdoc-20230321/README.rst
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-03-21 16:23:57.771566 linuxdoc-20230321/linuxdoc/
--rw-rw-r--   0 markus   (10001) markus   (10001)      789 2023-03-21 15:59:23.000000 linuxdoc-20230321/linuxdoc/__init__.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     5420 2023-03-21 16:22:52.000000 linuxdoc-20230321/linuxdoc/__pkginfo__.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     7290 2023-03-21 15:59:30.000000 linuxdoc-20230321/linuxdoc/autodoc.py
--rw-rw-r--   0 markus   (10001) markus   (10001)      560 2023-03-21 15:59:34.000000 linuxdoc-20230321/linuxdoc/cdomain.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     5085 2023-03-21 15:59:38.000000 linuxdoc-20230321/linuxdoc/cdomainv2.py
--rw-rw-r--   0 markus   (10001) markus   (10001)      766 2023-03-21 15:59:43.000000 linuxdoc-20230321/linuxdoc/cdomainv3.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     1734 2023-03-21 15:59:49.000000 linuxdoc-20230321/linuxdoc/compat.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     2785 2023-03-21 15:59:54.000000 linuxdoc-20230321/linuxdoc/grep_doc.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)   117246 2023-03-21 16:00:05.000000 linuxdoc-20230321/linuxdoc/kernel_doc.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     7961 2023-03-21 16:00:47.000000 linuxdoc-20230321/linuxdoc/kernel_include.py
--rw-rw-r--   0 markus   (10001) markus   (10001)    17224 2023-03-21 16:01:00.000000 linuxdoc-20230321/linuxdoc/kfigure.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     3722 2023-03-21 16:01:07.000000 linuxdoc-20230321/linuxdoc/lint.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    13347 2023-03-21 16:01:21.000000 linuxdoc-20230321/linuxdoc/manKernelDoc.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    12757 2023-03-21 16:01:38.000000 linuxdoc-20230321/linuxdoc/rstFlatTable.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    18769 2023-03-21 16:01:49.000000 linuxdoc-20230321/linuxdoc/rstKernelDoc.py
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-03-21 16:23:57.771566 linuxdoc-20230321/linuxdoc.egg-info/
--rw-rw-r--   0 markus   (10001) markus   (10001)     1931 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)      580 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        1 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)      171 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/entry_points.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       34 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/requires.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       15 2023-03-21 16:23:57.000000 linuxdoc-20230321/linuxdoc.egg-info/top_level.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       61 2023-03-21 16:23:57.771566 linuxdoc-20230321/setup.cfg
--rwxrwxr-x   0 markus   (10001) markus   (10001)     1149 2021-07-08 14:17:32.000000 linuxdoc-20230321/setup.py
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-03-21 16:23:57.771566 linuxdoc-20230321/tests/
--rwxrwxr-x   0 markus   (10001) markus   (10001)      404 2021-07-08 14:17:32.000000 linuxdoc-20230321/tests/__init__.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/
+-rw-rw-r--   0 markus    (1001) markus    (1001)    34520 2023-03-25 08:10:56.000000 linuxdoc-20230506/LICENSE
+-rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-05-06 08:55:08.801174 linuxdoc-20230506/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1002 2023-05-06 08:50:39.000000 linuxdoc-20230506/README.rst
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/linuxdoc/
+-rw-rw-r--   0 markus    (1001) markus    (1001)      777 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/__init__.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5829 2023-05-06 08:39:00.000000 linuxdoc-20230506/linuxdoc/__pkginfo__.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7200 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/autodoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      560 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomain.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5085 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomainv2.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      754 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/cdomainv3.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1734 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/compat.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1701 2023-05-06 08:23:40.000000 linuxdoc-20230506/linuxdoc/deprecated.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     2016 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/grepdoc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)   110357 2023-05-06 07:53:06.000000 linuxdoc-20230506/linuxdoc/kernel_doc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7949 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/kernel_include.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)    17224 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/kfigure.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     3321 2023-03-26 12:51:46.000000 linuxdoc-20230506/linuxdoc/lint.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    13347 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/manKernelDoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     6418 2023-05-06 07:47:06.000000 linuxdoc-20230506/linuxdoc/rest.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    12757 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/rstFlatTable.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    18769 2023-03-25 08:10:56.000000 linuxdoc-20230506/linuxdoc/rstKernelDoc.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/linuxdoc.egg-info/
+-rw-rw-r--   0 markus    (1001) markus    (1001)     2211 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)      619 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)        1 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)      389 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       34 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       15 2023-05-06 08:55:08.000000 linuxdoc-20230506/linuxdoc.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       61 2023-05-06 08:55:08.805174 linuxdoc-20230506/setup.cfg
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     1191 2023-05-06 08:15:34.000000 linuxdoc-20230506/setup.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2023-05-06 08:55:08.801174 linuxdoc-20230506/tests/
+-rwxrwxr-x   0 markus    (1001) markus    (1001)      392 2023-03-25 08:10:56.000000 linuxdoc-20230506/tests/__init__.py
```

### Comparing `linuxdoc-20230321/LICENSE` & `linuxdoc-20230506/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/README.rst` & `linuxdoc-20230506/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 extensions in common Sphinx-doc projects.
 
 
 Install
 =======
 
 `Install LinuxDoc <https://return42.github.io/linuxdoc/install.html>`__ using `pip
-<https://pip.pypa.io/en/stable/quickstart/>`__:
+<https://pip.pypa.io/en/stable/getting-started/>`__:
 
 .. code-block:: text
 
    pip install --user -U linuxdoc
 
 
 Links
@@ -25,13 +25,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20230321)
-copyright:   2024 Markus Heiser
+package:     linuxdoc (20230506)
+copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20230321/linuxdoc/__init__.py` & `linuxdoc-20230506/linuxdoc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The LinuxDoc library contains Sphinx-doc extensions and command line tools
 related to the build process of the Linux-Kernel documentation.  Even if this
 project started in context of the Linux-Kernel documentation, you can use these
 extensions in common Sphinx-doc projects.
 
 :copyright:  Copyright (C) 2018 Markus Heiser
 :e-mail:     markus.heiser@darmarIT.de
-:license:    GPL Version 2, June 1991 see Linux/COPYING for details.
+:license:    AGPL-3.0-or-later; see LICENSE for details.
 :docs:       http://return42.github.io/linuxdoc
 :repository: `github return42/linuxdoc <https://github.com/return42/linuxdoc>`_
 """
 
 from . import __pkginfo__
 
 __version__   = __pkginfo__.version
```

### Comparing `linuxdoc-20230321/linuxdoc/__pkginfo__.py` & `linuxdoc-20230506/linuxdoc/__pkginfo__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # pylint: disable=line-too-long, invalid-name, consider-using-f-string
 """Python package meta informations used by setup.py and other project files.
 """
 
 from setuptools import find_packages
 
 package = 'linuxdoc'
-version = '20230321'
+version = '20230506'
 
-copyright = '2024 Markus Heiser'  # pylint: disable=redefined-builtin
+copyright = '2023 Markus Heiser'  # pylint: disable=redefined-builtin
 description = (
     'Sphinx-doc extensions & tools to extract documentation'
     ' from C/C++ source file comments.'
 )
 license   = 'AGPLv3+'  # pylint: disable=redefined-builtin
 keywords = 'sphinx extension doc source code comments kernel-doc linux'
 
@@ -30,14 +30,15 @@
 docs = 'https://return42.github.io/linuxdoc'
 issues = url + '/issues'
 
 project_urls = {
     'Documentation'    : docs,
     'Code'             : url,
     'Issue tracker'    : issues,
+    'Changelog'        : url + '/blob/master/CHANGELOG',
 }
 
 packages = find_packages(exclude=['docs', 'tests'])
 
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files
 package_data = {
 #     'xxxx' : [
@@ -97,14 +98,15 @@
 test_requires = [
     'pylint'
     ]
 test_requires.sort()
 test_requires_txt = "\n".join(test_requires)
 
 develop_requires = [
+    'argparse-manpage',
     'pallets-sphinx-themes',
     'sphinx-autobuild',
     'sphinx-issues',
     'sphinx-jinja',
     'sphinx-tabs',
     'sphinxcontrib-programoutput',
     'tox',
@@ -112,18 +114,27 @@
     ]
 develop_requires_txt = "\n".join(develop_requires)
 
 def get_entry_points():
     """get entry points of the python package"""
     return {
         'console_scripts': [
-            'kernel-doc = linuxdoc.kernel_doc:main',
-            'kernel-autodoc = linuxdoc.autodoc:main',
-            'kernel-lintdoc = linuxdoc.lint:main',
-            'kernel-grepdoc = linuxdoc.grep_doc:main',
+
+            'linuxdoc.rest = linuxdoc.rest:main',
+            'linuxdoc.autodoc = linuxdoc.autodoc:main',
+            'linuxdoc.lintdoc = linuxdoc.lint:main',
+            'linuxdoc.grepdoc = linuxdoc.grepdoc:main',
+
+            # compatibility / deprecated
+
+            'kernel-doc = linuxdoc.deprecated:cmd_kernel_doc',
+            'kernel-autodoc = linuxdoc.deprecated:cmd_kernel_autodoc',
+            'kernel-lintdoc = linuxdoc.deprecated:cmd_kernel_lintdoc',
+            'kernel-grepdoc = linuxdoc.deprecated:cmd_kernel_grepdoc',
+
         ]
     }
 
 requirements_txt = """\
 %(install_requires_txt)s
 """ % globals()
 
@@ -146,15 +157,15 @@
 
 %(docstring)s
 
 Install
 =======
 
 `Install LinuxDoc <%(docs)s/install.html>`__ using `pip
-<https://pip.pypa.io/en/stable/quickstart/>`__:
+<https://pip.pypa.io/en/stable/getting-started/>`__:
 
 .. code-block:: text
 
    pip install --user -U linuxdoc
 
 
 Links
```

### Comparing `linuxdoc-20230321/linuxdoc/autodoc.py` & `linuxdoc-20230506/linuxdoc/autodoc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: AGPL-3.0-or-later
-u"""
-    autodoc
-    ~~~~~~~
+"""
+autodoc
+~~~~~~~
 
-    Implementation of the ``kernel-autodoc`` command.
+Implementation of the ``linuxdoc.autodoc`` command.
 
-    :copyright:  Copyright (C) 2018 Markus Heiser
-    :license:    GPL Version 2, June 1991 see Linux/COPYING for details.
+:copyright:  Copyright (C) 2023 Markus Heiser
+:license:    AGPL-3.0-or-later; see LICENSE for details.
 
-    The ``kernel-autodoc`` command extracts documentation from Linux kernel's
-    source code comments, see ``--help``::
+The command ``linuxdoc.autodoc`` extracts the kernel-doc comments from the
+source code and uses them to create documentation of the source code in the reST
+markup::
 
-        $ kernel-autodoc --help
+    $ linuxdoc.autodoc --help
 
 """
 
-# ------------------------------------------------------------------------------
-# imports
-# ------------------------------------------------------------------------------
-
 import sys
 import argparse
 import multiprocessing
 
 import six
 
 from fspath import FSPath
 from . import kernel_doc as kerneldoc
 from .kernel_doc import Container
 
+CMD = None
 
-# ------------------------------------------------------------------------------
-# config
-# ------------------------------------------------------------------------------
-
-MARKUP = "kernel-doc" # "reST"
 MSG    = lambda msg: sys.__stderr__.write("INFO : %s\n" % msg)
 ERR    = lambda msg: sys.__stderr__.write("ERROR: %s\n" % msg)
 FATAL  = lambda msg: sys.__stderr__.write("FATAL: %s\n" % msg)
 
 TEMPLATE_INDEX="""\
 .. -*- coding: utf-8; mode: rst -*-
 
@@ -48,74 +40,30 @@
 ================================================================================
 
 .. toctree::
     :maxdepth: 1
 
 """
 
-EPILOG = u"""This implementation of autodoc uses the kernel-doc parser from the linuxdoc
+EPILOG = """This command uses the kernel-doc parser from the linuxdoc Sphinx
 extension, for details see: https://return42.github.io/linuxdoc/cmd-line.html"""
 
-CMD = None
+DESCRIPTION = """The linuxdoc.autodoc tool can be used to generate documentation
+in the reST markup from the kernel-doc markup comments in the source files.
+This tool can be used to create an analogous document structure in reST markup
+from the folder structure of the source code.  """
 
 # ------------------------------------------------------------------------------
 def main():
 # ------------------------------------------------------------------------------
 
-    "Parse *kernel-doc* comments from source code (main)"
-
     global CMD  # pylint: disable=global-statement
 
-    CLI = argparse.ArgumentParser(  # pylint: disable=invalid-name
-        description = ("Parse *kernel-doc* comments from source code")
-        , epilog = EPILOG
-        , formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-
-    CLI.add_argument(
-        "srctree"
-        , help    = "Folder of source code."
-        , type    = lambda x: FSPath(x).ABSPATH)
-
-    CLI.add_argument(
-        "doctree"
-        , help    = "Folder to place reST documentation."
-        , type    = lambda x: FSPath(x).ABSPATH)
-
-    CLI.add_argument(
-        "--sloppy"
-        , action  = "store_true"
-        , help    = "Sloppy comment check, reports only severe errors.")
-
-    CLI.add_argument(
-        "--force"
-        , action  = "store_true"
-        , help    = "Don't stop if doctree exists.")
-
-    CLI.add_argument(
-        "--threads"
-        , type    =  int
-        , default = multiprocessing.cpu_count()
-        , help    = "Use up to n threads.")
-
-    CLI.add_argument(
-        "--markup"
-        , choices = ["reST", "kernel-doc"]
-        , default = "reST"
-        , help    = (
-            "Markup of the comments. Change this option only if you know"
-            " what you do. New comments must be marked up with reST!"))
-
-    CLI.add_argument(
-        "--rst-files"
-        , type    = lambda x: FSPath(x).ABSPATH
-        , help    = (
-            "File that list source files, which has comments in reST markup."
-            " Use kernel-grepdoc command to generate those file."))
-
-    CMD = CLI.parse_args()
+    cli = get_cli()
+    CMD = cli.parse_args()
 
     if not CMD.srctree.EXISTS:
         ERR("%s does not exists." % CMD.srctree)
         sys.exit(42)
 
     if not CMD.srctree.ISDIR:
         ERR("%s is not a folder." % CMD.srctree)
@@ -138,23 +86,77 @@
         pool.join()
     else:
         for fname in gather_filenames(CMD):
             autodoc_file(fname)
 
     insert_index_files(CMD.doctree)
 
+def get_cli():
+
+    cli = argparse.ArgumentParser(
+        description = DESCRIPTION
+        , epilog = EPILOG
+        , formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+    cli.add_argument(
+        "srctree"
+        , help    = "Folder of source code."
+        , type    = lambda x: FSPath(x).ABSPATH
+    )
+    cli.add_argument(
+        "doctree"
+        , help    = "Folder to place reST documentation."
+        , type    = lambda x: FSPath(x).ABSPATH
+    )
+    cli.add_argument(
+        "--sloppy"
+        , action  = "store_true"
+        , help    = "Sloppy comment check, reports only severe errors."
+    )
+    cli.add_argument(
+        "--force"
+        , action  = "store_true"
+        , help    = "Don't stop if doctree exists."
+    )
+    cli.add_argument(
+        "--threads"
+        , type    =  int
+        , default = multiprocessing.cpu_count()
+        , help    = "Use up to n threads."
+    )
+    cli.add_argument(
+        "--markup"
+        , choices = ["reST", "kernel-doc"]
+        , default = "reST"
+        , help    = (
+            "Markup of the comments.  Change this option only if you know what"
+            " you do and make use of --rst-files if you also have some files in"
+            " your source tree with reST markup.  The markup of new comments must"
+            " be reST!"
+        )
+    )
+    cli.add_argument(
+        "--rst-files"
+        , type    = lambda x: FSPath(x).ABSPATH
+        , help    = (
+            "File that list source files, which has comments in reST markup."
+            " Use linuxdoc.grepdoc command to generate those file."
+        )
+    )
+
+    return cli
+
+
 # ------------------------------------------------------------------------------
 def gather_filenames(cmd):
 # ------------------------------------------------------------------------------
 
     "yield .c & .h filenames"
 
     for fname in cmd.srctree.reMatchFind(r"^.*\.[ch]$"):
-        if fname.startswith(CMD.srctree/"Documentation"):
-            continue
         yield fname
 
 # ------------------------------------------------------------------------------
 def autodoc_file(fname):
 # ------------------------------------------------------------------------------
 
     "generate documentation from fname"
@@ -162,15 +164,15 @@
     fname  = fname.relpath(CMD.srctree)
     markup = CMD.markup
 
     if CMD.markup == "kernel-doc" and fname in CMD.rst_files:
         markup = "reST"
 
     opts = kerneldoc.ParseOptions(
-        rel_fname       = fname
+        fname           = fname
         , src_tree      = CMD.srctree
         , verbose_warn  = not (CMD.sloppy)
         , use_all_docs  = True
         , markup        = markup )
 
     parser = kerneldoc.Parser(opts, kerneldoc.NullTranslator())
     try:
```

### Comparing `linuxdoc-20230321/linuxdoc/cdomain.py` & `linuxdoc-20230506/linuxdoc/cdomain.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/cdomainv2.py` & `linuxdoc-20230506/linuxdoc/cdomainv2.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/cdomainv3.py` & `linuxdoc-20230506/linuxdoc/cdomainv3.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 u"""
     cdomainv3 (Sphinx v>=3.0)
     ~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Replacement for the sphinx c-domain.
 
     :copyright:  Copyright (C) 2020 Markus Heiser
-    :license:    GPL Version 2, June 1991 see Linux/COPYING for details.
+    :license:    AGPL-3.0-or-later; see LICENSE for details.
 
     For user documentation see :ref:`customized-c-domain`.
 """
 
 from sphinx.domains.c import CObject as Base_CObject
 from sphinx.domains.c import CDomain as Base_CDomain
```

### Comparing `linuxdoc-20230321/linuxdoc/compat.py` & `linuxdoc-20230506/linuxdoc/compat.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/kernel_doc.py` & `linuxdoc-20230506/linuxdoc/kernel_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,65 +3,54 @@
 #
 # pylint: disable=missing-docstring, arguments-differ, invalid-name
 # pylint: disable=too-many-arguments, too-many-locals, too-many-branches
 # pylint: disable=too-many-nested-blocks, too-many-lines
 # pylint: disable=too-many-statements, useless-object-inheritance
 
 """
-    kernel_doc
-    ~~~~~~~~~~
+kernel_doc
+~~~~~~~~~~
 
-    Implementation of the ``kernel-doc`` parser.
+Implementation of the ``kernel-doc`` parser.  The kernel-doc parser extracts
+:ref:`kernel-doc markup <kernel-doc-intro>` from source code comments.
 
-    The kernel-doc parser extracts documentation from Linux kernel's source code
-    comments. This implements the :ref:`kernel-doc markup <kernel-doc-intro>`.
+This module provides an API which could be used by a sphinx-doc generator
+extension and a command-line interface
 
-    This module provides an API -- which could be used by a sphinx-doc generator
-    extension -- and a command-line interface, see ``--help``::
+Compared with the Perl kernel-doc script used in the Linux kernel, this
+implementation has additional features like *parse options* for a smooth
+integration of reStructuredText (reST) markup in the source code comments.  In
+combination with the (separate) *kernel-doc* reST directive (which uses this
+module), the documentation generation becomes more clear and flexible.
 
-        $ kernel-doc --help
+The architecture of the parser is simple and consists of three types of
+objects (three classes).
 
-    But, the command-line is only for test, normally you don't need it.
+* :py:obj:`Parser`: The parser parses the source-file and dumps extracted
+  kernel-doc data.
 
-    Compared with the Perl kernel-doc script, this implementation has additional
-    features like *parse options* for a smooth integration of reStructuredText
-    (reST) markup in the kernel's source code comments.  In combination with the
-    (separate) *kernel-doc* reST directive (which uses this module), the
-    documentation generation becomes more clear and flexible.
+* subclasses of class :py:obj:`TranslatorAPI`: to translate the dumped
+  kernel-doc data into output formats. There exists two implementations:
 
-    The architecture of the parser is simple and consists of three types of
-    objects (three classes).
+  - :py:obj:`NullTranslator`: translates nothing, just parse
 
-    * class Parser: The parser parses the source-file and dumps extracted
-      kernel-doc data.
+  - :py:obj:`ReSTTranslator`: translates dumped kernel-doc data to reST markup
 
-    * subclasses of class TranslatorAPI: to translate the dumped kernel-doc data
-      into output formats. There exists two implementations:
+* :py:obj:`ParseOptions`: a container full with options to control *parsing* and
+  *translation*.
 
-      - class NullTranslator: translates nothing, just parse
-
-      - class ReSTTranslator(TranslatorAPI): translates dumped kernel-doc data
-        to reST markup.
-
-    * class ParseOptions: a container full with options to control parsing an
-      translation.
-
-    With the NullTranslator a source file is parsed only once while different
-    output could be generated (multiple times) just by changing the Translator
-    (e.g. with the ReSTTranslator) and the option container.
-
-    With parsing the source files only once, the building time is reduced n-times.
+With the :py:obj:`NullTranslator` a source file is parsed only once while
+different output could be generated (multiple times) just by changing the
+Translator (e.g. with the :py:obj:`ReSTTranslator`) and the option
+container. With parsing the source files only once, the building time is reduced
+n-times.
 
 """
 
-# ==============================================================================
-# imports
-# ==============================================================================
 
-import argparse
 import codecs
 import collections
 import copy
 import os
 import re
 import sys
 import textwrap
@@ -334,18 +323,15 @@
 
 class DevNull(object): # pylint: disable=too-few-public-methods
     """A dev/null file descriptor."""
     def write(self, *args, **kwargs):
         pass
 DevNull = DevNull()
 
-SRCTREE        = OS_ENV.get("srctree", os.getcwd())
-GIT_REF        = ("Linux kernel source tree:"
-                  " `%(rel_fname)s <https://git.kernel.org/cgit/linux/kernel/git/torvalds/linux.git/tree/"
-                  "%(rel_fname)s>`__")
+SRCTREE = OS_ENV.get("srctree", os.getcwd())
 DEFAULT_EXP_METHOD = "macro"
 """Default value of ``:exp-method:``"""
 
 DEFAULT_EXP_IDS    = ['EXPORT_SYMBOL', 'EXPORT_SYMBOL_GPL', 'EXPORT_SYMBOL_GPL_FUTURE']
 """Default value of ``:exp-ids:``"""
 
 # ==============================================================================
@@ -388,194 +374,14 @@
             return
         message = message % replace
         replace.update(dict(message = message, logclass = "DEBUG"))
         STREAM.log_out.write(self.LOG_FORMAT % replace)
 
 LOG = SimpleLog()
 
-# ==============================================================================
-def main():
-    # pylint: disable=global-statement
-# ==============================================================================
-
-    global VERBOSE, DEBUG
-
-    epilog = (u"This implementation uses the kernel-doc parser"
-              " from the linuxdoc extension, for detail informations read"
-              " https://return42.github.io/linuxdoc/cmd-line.html#kernel-doc")
-
-    CLI = argparse.ArgumentParser(
-        description = (
-            "Parse *kernel-doc* comments from source code"
-            " and print them (with reST markup) to stdout." )
-        , epilog = epilog
-        , formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-
-    CLI.add_argument(
-        "files"
-        , nargs   = "+"
-        , help    = "source file(s) to parse.")
-
-    CLI.add_argument(
-        "--id-prefix"
-        , default = ""
-        , help    = (
-            "A prefix for automatic generated IDs. The IDs are automaticly"
-            " gernerated based on the declaration and / or section names. The"
-            " prefix is also used as namespace in Sphinx's C-domain"))
-
-    CLI.add_argument(
-        "--verbose", "-v"
-        , action  = "store_true"
-        , help    = "verbose output with log messages to stderr" )
-
-    CLI.add_argument(
-        "--sloppy"
-        , action  = "store_true"
-        , help    = "Sloppy linting, reports only severe errors.")
-
-    CLI.add_argument(
-        "--debug"
-        , action  = "store_true"
-        , help    = "debug messages to stderr" )
-
-    CLI.add_argument(
-        "--quiet", "-q"
-        , action  = "store_true"
-        , help    = "no messages to stderr" )
-
-    CLI.add_argument(
-        "--skip-preamble"
-        , action  = "store_true"
-        , help    = "skip preamble in the output" )
-
-    CLI.add_argument(
-        "--skip-epilog"
-        , action  = "store_true"
-        , help    = "skip epilog in the output" )
-
-    CLI.add_argument(
-        "--list-internals"
-        , choices = Parser.DOC_TYPES + ["all"]
-        , nargs   = "+"
-        , help    = "list symbols, titles or whatever is documented, but *not* exported" )
-
-    CLI.add_argument(
-        "--list-exports"
-        , action  = "store_true"
-        , help    = "list all exported symbols" )
-
-    CLI.add_argument(
-        "--use-names"
-        , nargs   = "+"
-        , help    = "print documentation of functions, structs or whatever title/object")
-
-    CLI.add_argument(
-        "--exported"
-        , action  = "store_true"
-        , help    = "print documentation of all exported symbols")
-
-    CLI.add_argument(
-        "--internal"
-        , action  = "store_true"
-        , help    = ("print documentation of all symbols that are documented,"
-                     " but not exported" ))
-
-    CLI.add_argument(
-        "--markup"
-        , choices = ["reST", "kernel-doc"]
-        , default = "reST"
-        , help    = (
-            "Markup of the comments. Change this option only if you know"
-            " what you do. New comments must be marked up with reST!"))
-
-    CLI.add_argument(
-        "--symbols-exported-method"
-        , default = DEFAULT_EXP_METHOD
-        , help    = (
-            "Indicate the way by which an exported symbol an exported symbol"
-            " is exported. Must be either 'macro' or 'attribute'."))
-
-    CLI.add_argument(
-        "--symbols-exported-identifiers"
-        , nargs   = "+"
-        , default = DEFAULT_EXP_IDS
-        , help    = "identifiers list that specifies an exported symbol")
-
-    CLI.add_argument(
-        "--known-attrs"
-        , default = []
-        , nargs   = "+"
-        , help    = ("provides a list of known attributes that has to be"
-                     " hidden when displaying function prototypes"))
-
-    CMD     = CLI.parse_args()
-    VERBOSE = CMD.verbose
-    DEBUG   = CMD.debug
-
-    if CMD.quiet:
-        STREAM.log_out = DevNull  # pylint: disable=attribute-defined-outside-init
-
-    LOG.debug(u"CMD: %(CMD)s", CMD=CMD)
-
-    retVal     = 0
-
-    for fname in CMD.files:
-        translator = ReSTTranslator()
-        opts = ParseOptions(
-            fname           = fname
-            , id_prefix     = CMD.id_prefix
-            , skip_preamble = CMD.skip_preamble
-            , skip_epilog   = CMD.skip_epilog
-            , out           = STREAM.appl_out
-            , markup        = CMD.markup
-            , verbose_warn  = not (CMD.sloppy)
-            , exp_method    = CMD.symbols_exported_method
-            , exp_ids       = CMD.symbols_exported_identifiers
-            , known_attrs   = CMD.known_attrs
-            ,)
-        opts.set_defaults()
-
-        if CMD.list_exports or CMD.list_internals:
-            translator = ListTranslator(CMD.list_exports, CMD.list_internals)
-            opts.gather_context = True
-
-        elif CMD.use_names:
-            opts.use_names  = CMD.use_names
-
-        elif CMD.exported or CMD.internal:
-            # gather exported symbols ...
-            src   = readFile(opts.fname)
-            ctx   = ParserContext()
-            Parser.gather_context(src, ctx, opts)
-
-            opts.error_missing = False
-            opts.use_names     = ctx.exported_symbols
-            opts.skip_names    = []
-
-            if CMD.internal:
-                opts.use_names  = []
-                opts.skip_names = ctx.exported_symbols
-        else:
-            # if non section is choosen by use-name, internal or exclude, then
-            # use all DOC: sections
-            opts.use_all_docs = True
-
-        parser = Parser(opts, translator)
-        parser.parse()
-        parser.close()
-        if parser.errors:
-            retVal = 1
-
-    return retVal
-
-# ==============================================================================
-# API
-# ==============================================================================
-
 # ------------------------------------------------------------------------------
 class TranslatorAPI(object):
 # ------------------------------------------------------------------------------
     u"""
     Abstract kernel-doc translator.
 
     :cvar list cls.HIGHLIGHT_MAP:  highlight mapping
@@ -1421,15 +1227,15 @@
 
         self.rel_fname = self.fname
         if self.fname[0] == '/':
             if not self.src_tree:
                 LOG.error("missing SRCTREE")
             self.rel_fname = self.fname[1:]
 
-        self.fname = os.path.abspath(self.src_tree + "/" + self.rel_fname)
+        self.fname = os.path.abspath(str(self.src_tree) + "/" + str(self.rel_fname))
 
     def set_defaults(self):
 
         # default way to identify exported symbol
 
         if not self.exp_method:
             self.exp_method = DEFAULT_EXP_METHOD
@@ -1440,19 +1246,14 @@
         # default top title and top link
 
         if self.fname and self.top_title == "":
             self.top_title = os.path.basename(self.fname)
         if self.top_title:
             self.top_title = self.top_title % self
 
-        if self.top_link == "":
-            if self.rel_fname:
-                self.top_link  = GIT_REF % self
-            else:
-                LOG.warn("missing SRCTREE, can't set *top_link* option")
         if self.top_link:
             self.top_link = self.top_link % self
 
     def add_filters(self, parse_options):
 
         def setINSPECT(name, val): # pylint: disable=unused-argument
             global INSPECT
@@ -3069,14 +2870,7 @@
 
         if self.options.verbose_warn and not self.ctx.sections.get(self.section_return, None):
             self.warn("no description found for return-value of function '%(func)s()'"
                       , func = decl_name, line_no = self.ctx.decl_offset)
         else:
             self.debug("check_return_section(): return-value of %(func)s() OK"
                        , func = decl_name)
-
-# ==============================================================================
-# run ...
-# ==============================================================================
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `linuxdoc-20230321/linuxdoc/kernel_include.py` & `linuxdoc-20230506/linuxdoc/kernel_include.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 u"""
     kernel-include
     ~~~~~~~~~~~~~~
 
     Implementation of the ``kernel-include`` reST-directive.
 
     :copyright:  Copyright (C) 2018 Markus Heiser
-    :license:    GPL Version 2, June 1991 see linux/COPYING for details.
+    :license:    AGPL-3.0-or-later; see LICENSE for details.
 
     For user documentation see :ref:`kernel-include-directive`.
 """
 
 # ==============================================================================
 # imports
 # ==============================================================================
```

### Comparing `linuxdoc-20230321/linuxdoc/kfigure.py` & `linuxdoc-20230506/linuxdoc/kfigure.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/lint.py` & `linuxdoc-20230506/linuxdoc/lint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,117 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: AGPL-3.0-or-later
-u"""
-    lint
-    ~~~~
+"""
+lint
+~~~~
 
-    Implementation of the :ref:`kernel-lintdoc` command.
+Implementation of the :ref:`linuxdoc.lintdoc` command.
 
-    :copyright:  Copyright (C) 2018  Markus Heiser
-    :license:    GPL Version 2, June 1991 see Linux/COPYING for details.
-"""
+:copyright:  Copyright (C) 2023  Markus Heiser
+:license:    AGPL-3.0-or-later; see LICENSE for details.
 
-# ------------------------------------------------------------------------------
-# imports
-# ------------------------------------------------------------------------------
+The command ``linuxdoc.lint`` *lint* the kernel-doc comments in the source
+code::
+
+    $ linuxdoc.lint --help
+
+"""
 
 import sys
 import argparse
 
-#import six
-
 from fspath import FSPath
-from . import kernel_doc as kerneldoc
+from . import kernel_doc
 
-# ------------------------------------------------------------------------------
-# config
-# ------------------------------------------------------------------------------
+CMD = None
 
 MSG    = lambda msg: sys.__stderr__.write("INFO : %s\n" % msg)
 ERR    = lambda msg: sys.__stderr__.write("ERROR: %s\n" % msg)
 FATAL  = lambda msg: sys.__stderr__.write("FATAL: %s\n" % msg)
 
-EPILOG = u"""This implementation uses the kernel-doc parser
-from the linuxdoc extension, for detail informations read
-https://return42.github.io/linuxdoc/cmd-line.html#kernel-lintdoc"""
+EPILOG = """This command uses the kernel-doc parser from the linuxdoc Sphinx
+extension, for details see: https://return42.github.io/linuxdoc/cmd-line.html"""
+
+DESCRIPTION = """Lint the kernel-doc markup comments in the source code files."""
 
 # ------------------------------------------------------------------------------
 def main():
 # ------------------------------------------------------------------------------
 
-    "Lint *kernel-doc* comments from source code (main)"
+    global CMD  # pylint: disable=global-statement
+
+    cli = get_cli()
+    CMD = cli.parse_args()
+
+    kernel_doc.DEBUG = CMD.debug
+    kernel_doc.VERBOSE = CMD.verbose
+
+    if not CMD.srctree.EXISTS:
+        ERR("%s does not exists or is not a folder" % CMD.srctree)
+        sys.exit(42)
+
+    if CMD.srctree.ISDIR:
+        for fname in CMD.srctree.reMatchFind(r"^.*\.[ch]$"):
+            lintdoc_file(fname)
+    else:
+        fname = CMD.srctree
+        CMD.srctree = CMD.srctree.DIRNAME
+        lintdoc_file(fname)
+
+
+def get_cli():
 
-    CLI = argparse.ArgumentParser( # pylint: disable=invalid-name
-        description = ("Lint *kernel-doc* comments from source code")
+    cli = argparse.ArgumentParser(
+        description = ("")
         , epilog = EPILOG
         , formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
-    CLI.add_argument(
+    cli.add_argument(
         "srctree"
         , help    = "File or folder of source code."
-        , type    = lambda x: FSPath(x).ABSPATH)
-
-    CLI.add_argument(
+        , type    = lambda x: FSPath(x).ABSPATH
+    )
+    cli.add_argument(
         "--sloppy"
         , action  = "store_true"
-        , help    = "Sloppy linting, reports only severe errors.")
-
-    CLI.add_argument(
+        , help    = "Sloppy linting, reports only severe errors."
+    )
+    cli.add_argument(
         "--markup"
         , choices = ["reST", "kernel-doc"]
         , default = "reST"
         , help    = (
-            "Markup of the comments. Change this option only if you know"
-            " what you do. New comments must be marked up with reST!"))
-
-    CLI.add_argument(
+            "Markup of the comments.  Change this option only if you know"
+            " what you do. New comments must be marked up with reST!"
+        )
+    )
+    cli.add_argument(
         "--verbose", "-v"
         , action  = "store_true"
-        , help    = "verbose output with log messages to stderr" )
-
-    CLI.add_argument(
+        , help    = "verbose output with log messages to stderr"
+    )
+    cli.add_argument(
         "--debug"
         , action  = "store_true"
-        , help    = "debug messages to stderr" )
-
-    CMD = CLI.parse_args()  # pylint: disable=invalid-name
-    kerneldoc.DEBUG = CMD.debug
-    kerneldoc.VERBOSE = CMD.verbose
+        , help    = "debug messages to stderr"
+    )
+    return cli
 
-    if not CMD.srctree.EXISTS:
-        ERR("%s does not exists or is not a folder" % CMD.srctree)
-        sys.exit(42)
-
-    if CMD.srctree.ISDIR:
-        for fname in CMD.srctree.reMatchFind(r"^.*\.[ch]$"):
-            if fname.startswith(CMD.srctree/"Documentation"):
-                continue
-            lintdoc_file(fname, CMD)
-    else:
-        fname = CMD.srctree
-        CMD.srctree = CMD.srctree.DIRNAME
-        lintdoc_file(fname, CMD)
 
 # ------------------------------------------------------------------------------
-def lintdoc_file(fname, CMD):  # pylint: disable=invalid-name
+def lintdoc_file(fname):
 # ------------------------------------------------------------------------------
 
     "lint documentation from fname"
 
     fname = fname.relpath(CMD.srctree)
-    opts = kerneldoc.ParseOptions(
-        rel_fname       = fname
+    opts = kernel_doc.ParseOptions(
+        fname           = fname
         , src_tree      = CMD.srctree
         , verbose_warn  = not (CMD.sloppy)
-        , markup        = CMD.markup )
-
-    parser = kerneldoc.Parser(opts, kerneldoc.NullTranslator())
+        , markup        = CMD.markup
+    )
+    parser = kernel_doc.Parser(opts, kernel_doc.NullTranslator())
     try:
         parser.parse()
     except Exception:  # pylint: disable=broad-except
         FATAL("kernel-doc comments markup of %s seems buggy / can't parse" % opts.fname)
         return
```

### Comparing `linuxdoc-20230321/linuxdoc/manKernelDoc.py` & `linuxdoc-20230506/linuxdoc/manKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/rstFlatTable.py` & `linuxdoc-20230506/linuxdoc/rstFlatTable.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/linuxdoc/rstKernelDoc.py` & `linuxdoc-20230506/linuxdoc/rstKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20230321/setup.py` & `linuxdoc-20230506/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,8 +31,9 @@
     , author_email     = PKG.emails[0]
     , license          = PKG.license
     , keywords         = PKG.keywords
     , packages         = find_packages(exclude=['docs', ])
     , install_requires = PKG.install_requires
     , entry_points     = PKG.get_entry_points()
     , classifiers      = PKG.classifiers
+    , project_urls     = PKG.project_urls
 )
```

