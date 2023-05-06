# Comparing `tmp/whatthepatch-1.0.4.tar.gz` & `tmp/whatthepatch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatthepatch-1.0.4.tar", last modified: Sat Jan 28 23:28:08 2023, max compression
+gzip compressed data, was "whatthepatch-1.0.5.tar", last modified: Sat May  6 14:59:53 2023, max compression
```

## Comparing `whatthepatch-1.0.4.tar` & `whatthepatch-1.0.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:08.000180 whatthepatch-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-01-28 23:28:08.000180 whatthepatch-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-28 23:28:08.000180 whatthepatch-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:07.992180 whatthepatch-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:07.996180 whatthepatch-1.0.4/src/whatthepatch/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/src/whatthepatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/src/whatthepatch/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/src/whatthepatch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/src/whatthepatch/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/src/whatthepatch/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:07.996180 whatthepatch-1.0.4/src/whatthepatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-01-28 23:28:07.000000 whatthepatch-1.0.4/src/whatthepatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-28 23:28:07.000000 whatthepatch-1.0.4/src/whatthepatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 23:28:07.000000 whatthepatch-1.0.4/src/whatthepatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-28 23:28:07.000000 whatthepatch-1.0.4/src/whatthepatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:07.996180 whatthepatch-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:28:08.000180 whatthepatch-1.0.4/tests/casefiles/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/abc
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/apache-attachment-2241.diff
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/apache-attachment-28223.diff
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/context-header.diff
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/cvs-header.diff
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-context-blah.diff
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-context.diff
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-default-blah.diff
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-default.diff
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-ed.diff
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-rcs.diff
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-unified-bad.diff
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-unified-bad2.diff
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-unified-blah.diff
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-unified.diff
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/diff-unified2.diff
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/eclipse-attachment-126343.header
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/efg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/embedded-diff.comment
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-binary-files.diff
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-header-long.diff
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-header.diff
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-new-empty-file.diff
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-oneline-add.diff
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-oneline-change.diff
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git-oneline-rm.diff
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/git.patch
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/issue39-bash42-003.patch
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/lao
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/mozilla-252983-versionless.diff
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/mozilla-252983.diff
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/mozilla-527452-5.comment
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/mozilla-560291.diff
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-context.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-default.patch
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-ed.patch
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-git.patch
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-header.diff
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-mixed_line_ends.patch
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-rcs.patch
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/svn-unified.patch
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/tzu
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/unified-header-notab.diff
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/casefiles/unified-header.diff
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    53726 2023-01-28 23:27:55.000000 whatthepatch-1.0.4/tests/test_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.663455 whatthepatch-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-06 14:59:53.663455 whatthepatch-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 14:59:53.663455 whatthepatch-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.655455 whatthepatch-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.659455 whatthepatch-1.0.5/src/whatthepatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/src/whatthepatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/src/whatthepatch/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/src/whatthepatch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/src/whatthepatch/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/src/whatthepatch/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.659455 whatthepatch-1.0.5/src/whatthepatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-06 14:59:53.000000 whatthepatch-1.0.5/src/whatthepatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-06 14:59:53.000000 whatthepatch-1.0.5/src/whatthepatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 14:59:53.000000 whatthepatch-1.0.5/src/whatthepatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 14:59:53.000000 whatthepatch-1.0.5/src/whatthepatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.659455 whatthepatch-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:59:53.663455 whatthepatch-1.0.5/tests/casefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/abc
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/apache-attachment-2241.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/apache-attachment-28223.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/context-header.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/cvs-header.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-context-blah.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-context.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-default-blah.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-default.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-ed.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-rcs.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-unified-bad.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-unified-bad2.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-unified-blah.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-unified.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/diff-unified2.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/eclipse-attachment-126343.header
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/efg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/embedded-diff.comment
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-bin.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-binary-files.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-header-long.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-header.diff
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-new-empty-file.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-oneline-add.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-oneline-change.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git-oneline-rm.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/git.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/issue39-bash42-003.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/lao
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/mozilla-252983-versionless.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/mozilla-252983.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/mozilla-527452-5.comment
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/mozilla-560291.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-context.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-default.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-ed.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-git.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-header.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-mixed_line_ends.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-rcs.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/svn-unified.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/tzu
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/unified-header-notab.diff
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/casefiles/unified-header.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52682 2023-05-06 14:59:42.000000 whatthepatch-1.0.5/tests/test_patch.py
```

### Comparing `whatthepatch-1.0.4/LICENSE` & `whatthepatch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/PKG-INFO` & `whatthepatch-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatthepatch
-Version: 1.0.4
+Version: 1.0.5
 Summary: A patch parsing and application library.
 Maintainer-email: "Christopher S. Corley" <cscorley@gmail.com>
 Project-URL: Homepage, https://github.com/cscorley/whatthepatch
 Project-URL: Bug Tracker, https://github.com/cscorley/whatthepatch/issues
 Keywords: patch,diff,parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whatthepatch-1.0.4/README.rst` & `whatthepatch-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/pyproject.toml` & `whatthepatch-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "whatthepatch"
-version = "1.0.4"
+version = "1.0.5"
 maintainers = [{ name = "Christopher S. Corley", email = "cscorley@gmail.com" }]
 requires-python = ">=3.7"
 readme = "README.rst"
 description = "A patch parsing and application library."
 keywords = ["patch", "diff", "parser"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `whatthepatch-1.0.4/src/whatthepatch/apply.py` & `whatthepatch-1.0.5/src/whatthepatch/apply.py`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/src/whatthepatch/exceptions.py` & `whatthepatch-1.0.5/src/whatthepatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/src/whatthepatch/patch.py` & `whatthepatch-1.0.5/src/whatthepatch/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,15 +964,15 @@
             delta = git_binary_delta_start.match(line)
             if delta:
                 # not supported
                 new_size = 0
                 continue
         elif new_size > 0:
             if base85string.match(line):
-                assert len(line) >= 7 and ((len(line) - 2) % 5) != 0
+                assert len(line) >= 6 and ((len(line) - 1) % 5) == 0
                 new_encoded += line[1:]
             elif 0 == len(line):
                 decoded = base64.b85decode(new_encoded)
                 added_data = zlib.decompress(decoded)
                 assert new_size == len(added_data)
                 change = Change(None, 0, added_data, None)
                 changes.append(change)
@@ -988,15 +988,15 @@
             delta = git_binary_delta_start.match(line)
             if delta:
                 # not supported
                 old_size = 0
                 continue
         elif old_size > 0:
             if base85string.match(line):
-                assert len(line) >= 7 and ((len(line) - 2) % 5) != 0
+                assert len(line) >= 6 and ((len(line) - 1) % 5) == 0
                 old_encoded += line[1:]
             elif 0 == len(line):
                 decoded = base64.b85decode(old_encoded)
                 removed_data = zlib.decompress(decoded)
                 assert old_size == len(removed_data)
                 change = Change(0, None, None, removed_data)
                 changes.append(change)
```

### Comparing `whatthepatch-1.0.4/src/whatthepatch/snippets.py` & `whatthepatch-1.0.5/src/whatthepatch/snippets.py`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/src/whatthepatch.egg-info/PKG-INFO` & `whatthepatch-1.0.5/src/whatthepatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatthepatch
-Version: 1.0.4
+Version: 1.0.5
 Summary: A patch parsing and application library.
 Maintainer-email: "Christopher S. Corley" <cscorley@gmail.com>
 Project-URL: Homepage, https://github.com/cscorley/whatthepatch
 Project-URL: Bug Tracker, https://github.com/cscorley/whatthepatch/issues
 Keywords: patch,diff,parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `whatthepatch-1.0.4/src/whatthepatch.egg-info/SOURCES.txt` & `whatthepatch-1.0.5/src/whatthepatch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 tests/casefiles/diff-unified-bad2.diff
 tests/casefiles/diff-unified-blah.diff
 tests/casefiles/diff-unified.diff
 tests/casefiles/diff-unified2.diff
 tests/casefiles/eclipse-attachment-126343.header
 tests/casefiles/efg
 tests/casefiles/embedded-diff.comment
+tests/casefiles/git-bin.patch
 tests/casefiles/git-binary-files.diff
 tests/casefiles/git-header-long.diff
 tests/casefiles/git-header.diff
 tests/casefiles/git-new-empty-file.diff
 tests/casefiles/git-oneline-add.diff
 tests/casefiles/git-oneline-change.diff
 tests/casefiles/git-oneline-rm.diff
```

### Comparing `whatthepatch-1.0.4/tests/casefiles/apache-attachment-2241.diff` & `whatthepatch-1.0.5/tests/casefiles/apache-attachment-2241.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/apache-attachment-28223.diff` & `whatthepatch-1.0.5/tests/casefiles/apache-attachment-28223.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/cvs-header.diff` & `whatthepatch-1.0.5/tests/casefiles/cvs-header.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-context-blah.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-context-blah.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-context.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-context.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-unified-bad.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-unified-bad.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-unified-bad2.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-unified-bad2.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-unified-blah.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-unified-blah.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/diff-unified.diff` & `whatthepatch-1.0.5/tests/casefiles/diff-unified.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/embedded-diff.comment` & `whatthepatch-1.0.5/tests/casefiles/embedded-diff.comment`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/git.patch` & `whatthepatch-1.0.5/tests/casefiles/git.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/mozilla-252983-versionless.diff` & `whatthepatch-1.0.5/tests/casefiles/mozilla-252983-versionless.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/mozilla-252983.diff` & `whatthepatch-1.0.5/tests/casefiles/mozilla-252983.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/mozilla-527452-5.comment` & `whatthepatch-1.0.5/tests/casefiles/mozilla-527452-5.comment`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/mozilla-560291.diff` & `whatthepatch-1.0.5/tests/casefiles/mozilla-560291.diff`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-context.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-context.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-default.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-default.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-ed.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-ed.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-git.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-git.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-mixed_line_ends.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-mixed_line_ends.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-rcs.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-rcs.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/casefiles/svn-unified.patch` & `whatthepatch-1.0.5/tests/casefiles/svn-unified.patch`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/test_apply.py` & `whatthepatch-1.0.5/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `whatthepatch-1.0.4/tests/test_patch.py` & `whatthepatch-1.0.5/tests/test_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-
+import hashlib
 import os
 import time
 import unittest
 
 from src import whatthepatch as wtp
 from src.whatthepatch.patch import Change, diffobj
 from src.whatthepatch.patch import header as headerobj
@@ -1446,79 +1446,17 @@
         self.assertEqual(1, len(result))
         self.assertEqual(1000007, len(result[0].changes))
         # This is 2x the usual time for CI to allow for some slow tests
         # Really all we care about is that this parses faster than it used to (200s+)
         self.assertGreater(20, time.time() - start_time)
 
     def test_git_bin_patch(self):
-        text = """---
- fox.bin   | Bin 0 -> 44 bytes
- fox.txt   |   2 +-
- lorem.bin | Bin 0 -> 446 bytes
- lorem.zip | Bin 431 -> 432 bytes
- 4 files changed, 1 insertion(+), 1 deletion(-)
- create mode 100644 fox.bin
- create mode 100644 lorem.bin
-
-diff --git a/fox.bin b/fox.bin
-new file mode 100644
-index 0000000000000000000000000000000000000000..e7683ad05fd121a9ca86cab5a827d471d29b4d4f
-GIT binary patch
-literal 44
-ycmWH^NL45-%}mZ#NGi%N&r?XtuTaP;%`GTa$S+GRQYZmR=Ok8DDx~D6GXMZ<wh!6>
-
-literal 0
-HcmV?d00001
-
-diff --git a/fox.txt b/fox.txt
-index ff3bb63..8fe2a4b 100644
---- a/fox.txt
-+++ b/fox.txt
-@@ -1 +1 @@
--The quick brown fox jumps over the lazy dog
-\ No newline at end of file
-+The quick brown fox jumps over the lazy dog.
-\ No newline at end of file
-diff --git a/lorem.bin b/lorem.bin
-new file mode 100644
-index 0000000000000000000000000000000000000000..aef2724fd9ff72caf4eb1ac8333f0b5b322d82fb
-GIT binary patch
-literal 446
-zcmXw#&2d992!vD07T|eRB)42s0Fkh>Gy1ax9+w~Fm)wMaW%v8+Q!6-@SL9y$#G*l}
-z+6Ae%rODKMLNW(eV!J^Lqq#K40+haL&oHecme~?Bvp0hqihPGW)J|zdm0J@?;oarH
-zmq8nAXrppJ9#KlY;O<;#ecAL3ed<g!G4=*8MQZA&@*d*izVwphh+(LN@fx1`86ZyC
-zf%h#bZVFBhPiIy(OdV5yv}K(UJU$-1_=s~Fb|NWsEk$A}|AZot<LWnxp>0DLGNbT$
-z;NzKem<F)LV9-+%O)-~zFiWULtcEc=v$joflZvCs%aENL{d#4hAnVe(yS0~XLpC4=
-Lj`hdY>+$vrMRcVJ
-
-literal 0
-HcmV?d00001
-
-diff --git a/lorem.zip b/lorem.zip
-index 0f6beb70488e2b29fcaadf724b6f48ef0ab5bc4e..3c8a65bf1a97bb4180c83a0e31352b4edb4c245e 100644
-GIT binary patch
-delta 275
-zcmZ3_yn#6)z?+#xgn@y9gP}7+C2a4}O*1$c85s5gF(-ozLr#8CYOY>MMM-D~Cj+xl
-z?ABymATF)oW?*D_!OXw_CQK(BEOa*HaEZRjWV65P$+T=Pg^u?VBeY_ymt>hupAyrM
-zu_ldGFZao&vTKV}cPYzE-4`VHX!@1~7xxOUc%}T}z;fqZ+pf4>{#%je`L@mdh12$@
-z##~QSCtp2z)oM{#R?hTKa+j9=zO;TxpG;eTRQ}78>li9e@lU*`!E<hhw&gFg7Dwam
-z8SImV7?t(so$}Jyl=3cb^RC<rY)d+m{}%R^{b303W@M6M#^TAz$&AWOMzNDS7!}#P
-Jfj(wn0067{YH|Po
-
-delta 274
-zcmdnMyq-BCz?+#xgn@y9gW*b=N|;w+e?B`S1H&F5=46mz$jL8C&DATZC<zVWWMKXf
-zwKe%I5SLbPGcdBeU}j(d6Q&am7CIYpxJ2J%vRS9J^XV)mjz|9|Mrg$d2bs?H_R@1O
-z3ERvx-K;3mI{Tu~UBN!DcuoF~-cc7`ykS}Oi(}X0%ZjnlS&LuR*=$}?c38P&;q6b7
-zte+;GeDx$tHc;Din|CGu%S*K{!-L%UoHcs4e@O{%uz6ZO@ty`xpT$&}TIoXzX1boS
-zo-D+utS58IOJh^YyS&Z2axbtg=}i7x*!zt+z?+dtjv0#|C#NtfGku7f+{viO<^}XH
-G0|Nj=Vq`=B
+        with open("tests/casefiles/git-bin.patch") as f:
+            text = f.read()
 
--- 
-2.25.1
-"""
         result = list(wtp.patch.parse_patch(text))
         assert result
         assert len(result) == 4
         assert (
             result[0].changes[0].line
             == b"The quick brown fox jumps over the lazy dog\x00"
         )
@@ -1534,10 +1472,42 @@
             b" ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco"
             b" laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit"
             b" in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat"
             b" cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.\x00"
         )
         assert len(result[3].changes) == 0
 
+    def test_git_bin_patch_minline(self):
+        # test path with minimal line in binary diff
+        text = """---
+ 95  | Bin 94 -> 95 bytes
+ 1 files changed, 0 insertions(+), 0 deletions(-)
+
+diff --git a/95 b/95
+index cf104291536b187e299023ae37523f4649ca0600..edf50979da25419fbb399ffa6b93142e50dbbba7 100644
+GIT binary patch
+literal 95
+zcmV-l0HFT>FaHM=!1loEo7=$@IDCW@J2o!_PR6;*Rs73Fmit;^XEfl3aOa~j;?1+w
+z`|Sh7<pH~|jb8KHD!MpYia}Lyu+Ot@)&HI>XeZ(}tCx^}pPZlER5Jer^*}gX^QK-R
+BGb8{2
+
+literal 94
+zcmV-k0HObM)Jh!P2BexYI{K1M2*Xhjg<rBg95P)btB3SD62E>3TEDprVXYw<r9s|q
+z3<q^r!wu=+9KVuWwwGi0e7gXw>S|c&%Px9;9nEE3cL}-^F2dKtTQun3NbDG}SFOY=
+AaR2}S
+
+--"""
+        result = list(wtp.patch.parse_patch(text))
+        assert result
+        assert len(result) == 1
+        assert (
+            hashlib.sha1(result[0].changes[0].line).hexdigest()
+            == "732e7e005ff8b71ab4b72398db0320f2fa012b81"
+        )
+        assert (
+            hashlib.sha1(result[0].changes[1].hunk).hexdigest()
+            == "b07b94142cfce2094b5be04e9d30b653a7c63917"
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

