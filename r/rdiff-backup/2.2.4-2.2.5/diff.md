# Comparing `tmp/rdiff-backup-2.2.4.tar.gz` & `tmp/rdiff-backup-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdiff-backup-2.2.4.tar", last modified: Mon Feb 27 06:45:40 2023, max compression
+gzip compressed data, was "rdiff-backup-2.2.5.tar", last modified: Sat May  6 09:24:02 2023, max compression
```

## Comparing `rdiff-backup-2.2.4.tar` & `rdiff-backup-2.2.5.tar`

### file list

```diff
@@ -1,422 +1,422 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/workflows/test_linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.github/workflows/test_windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    99914 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/CHANGELOG.adoc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/CONTRIBUTING.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/bindep.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/debian/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/autobuild.sh
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/gbp.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/debian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/tests/control
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/tests/smoke
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/debian/upstream/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/debian/upstream/metadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/dist/rdiff-backup-delete.1
--rw-r--r--   0 runner    (1001) docker     (123)    40173 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/dist/rdiff-backup-old.1
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/dist/rdiff-backup-statistics.1
--rw-r--r--   0 runner    (1001) docker     (123)    52092 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/dist/rdiff-backup.1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/docs/.bundle/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/.bundle/config
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/CODING.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/DEVELOP.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/DOCUMENTATION.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    32728 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/FAQ.adoc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/Gemfile
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/Windows-DEVELOP.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/Windows-README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.829109 rdiff-backup-2.2.4/docs/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/_layouts/default.html
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/_site_README.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.833109 rdiff-backup-2.2.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/api/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/api/index.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/api/v200.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/api/v201.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.833109 rdiff-backup-2.2.4/docs/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    76677 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/actions.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    50162 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/classes.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/completion.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/error_policy.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/index.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/locations.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/packages.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.833109 rdiff-backup-2.2.4/docs/arch/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/plugins/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/plugins/actions.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/plugins/index.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/plugins/meta.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.puml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.sh
--rw-r--r--   0 runner    (1001) docker     (123)   165260 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    95287 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/rdiffbackup_architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/arch/repository_format.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/credits.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.833109 rdiff-backup-2.2.4/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)    29310 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/asciidoctor.css
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/coderay.css
--rw-r--r--   0 runner    (1001) docker     (123)   113177 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    80651 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   200921 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/foundation.css
--rw-r--r--   0 runner    (1001) docker     (123)   196259 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/foundation.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/css/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/examples.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/features.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/index.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.833109 rdiff-backup-2.2.4/docs/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.837109 rdiff-backup-2.2.4/docs/js/foundation/
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.abide.js
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.accordion.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.alert.js
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.clearing.js
--rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.dropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.equalizer.js
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.interchange.js
--rw-r--r--   0 runner    (1001) docker     (123)    35791 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.joyride.js
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.js
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.magellan.js
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.offcanvas.js
--rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.orbit.js
--rw-r--r--   0 runner    (1001) docker     (123)    17925 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.reveal.js
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.slider.js
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.tab.js
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation/foundation.topbar.js
--rw-r--r--   0 runner    (1001) docker     (123)   233156 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/foundation.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/js/toc.js
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/migration.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.837109 rdiff-backup-2.2.4/docs/other/
--rw-r--r--   0 runner    (1001) docker     (123)    45141 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/other/rdiff-backup-old.1.html
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/other/related.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/rdiff-backup-delete.1.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    40184 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/rdiff-backup-old.1.template
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/rdiff-backup-statistics.1.adoc
--rw-r--r--   0 runner    (1001) docker     (123)    44357 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/rdiff-backup.1.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.837109 rdiff-backup-2.2.4/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-32.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-a.png
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-a.svg
--rw-r--r--   0 runner    (1001) docker     (123)    48873 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/docs/resources/logo-banner.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.837109 rdiff-backup-2.2.4/requs/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requs/00.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requs/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requs/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requs/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/requs/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.837109 rdiff-backup-2.2.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/_librsyncmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/cmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.841109 rdiff-backup-2.2.4/src/rdiff_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/FilenameMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Hardlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Rdiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Security.py
--rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/SetConnections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/Time.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35943 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/eas_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    45954 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/fs_abilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/increment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/iterfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/librsync.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/longname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/robust.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/rorpiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    73883 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/rpath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14953 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/run_delete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18811 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/run_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiff_backup/win_acls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.841109 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 06:45:40.000000 rdiff-backup-2.2.4/src/rdiff_backup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.841109 rdiff-backup-2.2.4/src/rdiffbackup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.841109 rdiff-backup-2.2.4/src/rdiffbackup/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    24583 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/list_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/actions_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.845109 rdiff-backup-2.2.4/src/rdiffbackup/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/_dir_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)    93823 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/_repo_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    45428 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/fs_abilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.845109 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/filenames.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/hardlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/longnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/map/owners.py
--rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/locations/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.845109 rdiff-backup-2.2.4/src/rdiffbackup/meta/
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta/acl_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta/acl_win.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta/ea.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta/stdattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/meta_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.845109 rdiff-backup-2.2.4/src/rdiffbackup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/argopts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/safestr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/simpleps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/src/rdiffbackup/utils/usrgrp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/FilenameMappingtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_backuprestore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_calculate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_compare_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_complete_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_regress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_remove_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/action_verify_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/backuptest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/cmdlinetest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26572 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/commontest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/comparetest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/connectiontest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/ctest.py
--rw-r--r--   0 runner    (1001) docker     (123)    27458 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/eas_aclstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/errorsrecovertest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/fileset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/find-max-ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/fs_abilitiestest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/hardlinktest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/hashtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/incrementtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/iterfiletest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/killtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/librsynctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/location_lock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/location_map_filenames_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/location_map_hardlinks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/longnametest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/makerestoretest3
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/metadatatest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/rdb_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/rdiffbackupdeletetest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/rdifftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/readonly_actions_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2219 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/regressfailedlongname.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/regresstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/resourceforktest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/restoretest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/robusttest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/roottest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/rorpitertest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/rpathtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/securitytest.py
--rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/selectiontest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      843 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/setconnectionstest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/statisticstest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/test_with_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/timetest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/user_grouptest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/utils_simpleps_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/testing/verbosity_actions_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/build_wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3638 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/check_links_in_adoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/completions/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/completions/README.adoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/completions/bash/rdiff-backup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/crossversion/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/ansible.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.821109 rdiff-backup-2.2.4/tools/crossversion/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/crossversion/host_vars/oldrdiffbackup/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/host_vars/oldrdiffbackup/version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/playbook-provision.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/crossversion/playbook-smoke-test.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/get_changelog_since.sh
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/hook-rdiffbackup.actions_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/hook-rdiffbackup.meta_mgr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3154 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/make_release.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.853109 rdiff-backup-2.2.4/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/README.adoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     4018 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/compress-rdiff-backup-increments
--rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/create_fs_as_user.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/deldiffs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/file-size-distribution.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/find2dirs
--rwxr-xr-x   0 runner    (1001) docker     (123)     2235 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/generate-code-overview.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2161 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/init_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/librsync-many-files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/make-many-data-files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2686 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/python-rdiff
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/rdiff-backup-regress.adoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     8515 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/rdiff-backup-regress.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/rdiff-backup-wrap
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/rdiff-many-files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/remove-comments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/misc/setup_dev_archlinux.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/prepare_api_doc.sh
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/rdiff-backup.bat
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/rdiff-backup.spec.template
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/rdiff-backup.spec.template-fedora
--rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/setup-testfiles.sh
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/win_build_librsync.sh
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/win_build_rdiffbackup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/win_package_rdiffbackup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/win_provision.sh
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/win_test_rdiffbackup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/README.adoc
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/ansible.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/collections/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.825109 rdiff-backup-2.2.4/tools/windows/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/group_vars/samba_servers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/samba_servers/rhbase.yml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/samba_servers/samba.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/group_vars/windows_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/windows_builders/librsync.yml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/windows_builders/rdiff-backup-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/windows_builders/rdiff-backup.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/group_vars/windows_hosts/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/group_vars/windows_hosts/generic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/playbook-debug-rdiff-backup.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/playbook-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/playbook-provision.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/playbook-test-rdiff-backup.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/defaults/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/files/dynamic-motd.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/meta/.galaxy_install_info
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/admin.yml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/auto-updates.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/install.yml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/security.yml
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/services.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/users.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_dnf.conf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_dnf_automatic.conf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_profile.d_localtime.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_yum.conf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_yum_yum-cron-hourly.conf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_yum_yum-cron.conf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/rh-base/vars/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/vars/Fedora.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/vars/RedHat.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/rh-base/vars/RedHat8.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/samba/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    18495 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/samba/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/defaults/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/samba/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.857110 rdiff-backup-2.2.4/tools/windows/roles/samba/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/meta/.galaxy_install_info
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/tools/windows/roles/samba/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/tools/windows/roles/samba/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/templates/smb.conf.j2
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/templates/smbusers.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:45:40.861110 rdiff-backup-2.2.4/tools/windows/roles/samba/vars/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/vars/os_Archlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/vars/os_Debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tools/windows/roles/samba/vars/os_RedHat.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tox_dist.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tox_root.ini
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tox_slow.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-02-27 06:45:09.000000 rdiff-backup-2.2.4/tox_win.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.525394 rdiff-backup-2.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.525394 rdiff-backup-2.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.525394 rdiff-backup-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/workflows/test_linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.github/workflows/test_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   100139 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/CHANGELOG.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/CONTRIBUTING.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/bindep.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.525394 rdiff-backup-2.2.5/debian/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/autobuild.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/gbp.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/debian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/tests/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/tests/smoke
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/debian/upstream/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/debian/upstream/metadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/dist/rdiff-backup-delete.1
+-rw-r--r--   0 runner    (1001) docker     (123)    40168 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/dist/rdiff-backup-old.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/dist/rdiff-backup-statistics.1
+-rw-r--r--   0 runner    (1001) docker     (123)    52082 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/dist/rdiff-backup.1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/docs/.bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/.bundle/config
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/CODING.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/DEVELOP.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/DOCUMENTATION.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    32728 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/FAQ.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/Windows-DEVELOP.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/Windows-README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.529394 rdiff-backup-2.2.5/docs/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/_layouts/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/_site_README.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.533394 rdiff-backup-2.2.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/api/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/api/index.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/api/v200.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/api/v201.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.533394 rdiff-backup-2.2.5/docs/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    76677 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/actions.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    50162 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/classes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/completion.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/error_policy.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/index.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/locations.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/packages.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.533394 rdiff-backup-2.2.5/docs/arch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/plugins/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/plugins/actions.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/plugins/index.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/plugins/meta.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.puml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   165260 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    95287 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/rdiffbackup_architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/arch/repository_format.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/credits.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.537394 rdiff-backup-2.2.5/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    29310 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/asciidoctor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/coderay.css
+-rw-r--r--   0 runner    (1001) docker     (123)   113177 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80651 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   200921 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/foundation.css
+-rw-r--r--   0 runner    (1001) docker     (123)   196259 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/foundation.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/examples.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/features.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/index.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.537394 rdiff-backup-2.2.5/docs/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.537394 rdiff-backup-2.2.5/docs/js/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.abide.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.accordion.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.clearing.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.dropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.equalizer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.interchange.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35791 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.joyride.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.magellan.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.offcanvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.orbit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17925 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.reveal.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.slider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.tab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation/foundation.topbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)   233156 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/foundation.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/js/toc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/migration.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.537394 rdiff-backup-2.2.5/docs/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    45141 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/other/rdiff-backup-old.1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/other/related.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/rdiff-backup-delete.1.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    40184 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/rdiff-backup-old.1.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/rdiff-backup-statistics.1.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    44357 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/rdiff-backup.1.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.541394 rdiff-backup-2.2.5/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-32.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-a.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    48873 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/docs/resources/logo-banner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.541394 rdiff-backup-2.2.5/requs/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requs/00.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requs/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requs/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requs/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/requs/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.541394 rdiff-backup-2.2.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/_librsyncmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/cmodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.545394 rdiff-backup-2.2.5/src/rdiff_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/FilenameMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14326 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Hardlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Rdiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/SetConnections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/Time.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35943 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/eas_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45954 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/fs_abilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/iterfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/librsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/longname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/regress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/rorpiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73883 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/rpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14953 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/run_delete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18811 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiff_backup/win_acls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.545394 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 09:24:02.000000 rdiff-backup-2.2.5/src/rdiff_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.545394 rdiff-backup-2.2.5/src/rdiffbackup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.549394 rdiff-backup-2.2.5/src/rdiffbackup/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/list_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/regress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/actions_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.549394 rdiff-backup-2.2.5/src/rdiffbackup/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/_dir_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93823 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/_repo_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45428 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/fs_abilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.549394 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/hardlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/longnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/map/owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/locations/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.549394 rdiff-backup-2.2.5/src/rdiffbackup/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta/acl_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta/acl_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta/ea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta/stdattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/meta_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.549394 rdiff-backup-2.2.5/src/rdiffbackup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/argopts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/quoting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/safestr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/simpleps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/src/rdiffbackup/utils/usrgrp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/FilenameMappingtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_backuprestore_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_calculate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_compare_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_complete_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_regress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_remove_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/action_verify_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/backuptest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/cmdlinetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26572 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/commontest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/comparetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/connectiontest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/ctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27458 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/eas_aclstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/errorsrecovertest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/fileset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/find-max-ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/fs_abilitiestest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/hardlinktest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/hashtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/incrementtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/iterfiletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/killtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/librsynctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/location_lock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/location_map_filenames_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/location_map_hardlinks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/longnametest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/makerestoretest3
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/metadatatest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/rdb_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/rdiffbackupdeletetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/rdifftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/readonly_actions_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2219 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/regressfailedlongname.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/regresstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/resourceforktest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/restoretest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/robusttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/roottest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/rorpitertest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/rpathtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/securitytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/selectiontest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      843 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/setconnectionstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/statisticstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/test_with_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/timetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/user_grouptest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/utils_simpleps_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/testing/verbosity_actions_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/build_wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3638 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/check_links_in_adoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/tools/completions/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/completions/README.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/tools/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/completions/bash/rdiff-backup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/tools/crossversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/ansible.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.521394 rdiff-backup-2.2.5/tools/crossversion/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.561394 rdiff-backup-2.2.5/tools/crossversion/host_vars/oldrdiffbackup/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/host_vars/oldrdiffbackup/version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/playbook-provision.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/crossversion/playbook-smoke-test.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/get_changelog_since.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/hook-rdiffbackup.actions_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/hook-rdiffbackup.meta_mgr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3154 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/make_release.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.565394 rdiff-backup-2.2.5/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/README.adoc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4018 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/compress-rdiff-backup-increments
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/create_fs_as_user.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/deldiffs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/file-size-distribution.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/find2dirs
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2235 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/generate-code-overview.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2161 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/init_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/librsync-many-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/make-many-data-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2686 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/python-rdiff
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/rdiff-backup-regress.adoc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8515 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/rdiff-backup-regress.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/rdiff-backup-wrap
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/rdiff-many-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/remove-comments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/misc/setup_dev_archlinux.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/prepare_api_doc.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/rdiff-backup.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/rdiff-backup.spec.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/rdiff-backup.spec.template-fedora
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/setup-testfiles.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/win_build_librsync.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/win_build_rdiffbackup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/win_package_rdiffbackup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/win_provision.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/win_test_rdiffbackup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.565394 rdiff-backup-2.2.5/tools/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/README.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/ansible.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.565394 rdiff-backup-2.2.5/tools/windows/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/collections/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.521394 rdiff-backup-2.2.5/tools/windows/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.565394 rdiff-backup-2.2.5/tools/windows/group_vars/samba_servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/samba_servers/rhbase.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/samba_servers/samba.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.565394 rdiff-backup-2.2.5/tools/windows/group_vars/windows_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/windows_builders/librsync.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/windows_builders/rdiff-backup-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/windows_builders/rdiff-backup.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/group_vars/windows_hosts/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/group_vars/windows_hosts/generic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/playbook-debug-rdiff-backup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/playbook-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/playbook-provision.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/playbook-test-rdiff-backup.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/files/dynamic-motd.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/meta/.galaxy_install_info
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/admin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/auto-updates.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/install.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/security.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/services.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/users.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_dnf.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_dnf_automatic.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_profile.d_localtime.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_yum.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_yum_yum-cron-hourly.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_yum_yum-cron.conf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.569394 rdiff-backup-2.2.5/tools/windows/roles/rh-base/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/vars/Fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/vars/RedHat.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/rh-base/vars/RedHat8.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18495 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/meta/.galaxy_install_info
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/templates/smb.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/templates/smbusers.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:24:02.573394 rdiff-backup-2.2.5/tools/windows/roles/samba/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/vars/os_Archlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/vars/os_Debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tools/windows/roles/samba/vars/os_RedHat.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tox_dist.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tox_root.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tox_slow.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-06 09:23:44.000000 rdiff-backup-2.2.5/tox_win.ini
```

### Comparing `rdiff-backup-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `rdiff-backup-2.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `rdiff-backup-2.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/pull_request_template.md` & `rdiff-backup-2.2.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/workflows/deploy.yml` & `rdiff-backup-2.2.5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/workflows/jekyll-gh-pages.yml` & `rdiff-backup-2.2.5/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/workflows/test_linux.yml` & `rdiff-backup-2.2.5/.github/workflows/test_linux.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/.github/workflows/test_windows.yml` & `rdiff-backup-2.2.5/.github/workflows/test_windows.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/CHANGELOG.adoc` & `rdiff-backup-2.2.5/CHANGELOG.adoc`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,40 @@
 
 The prefixes are to be understood as follows, in roughly decreasing order of importance for rdiff-backup users:
 
 * *CHG* marks changes in the behaviour of rdiff-backup, potentially _incompatible_ ones, which you will want to consider before you upgrade or use for the 1st time a new version.
 * *NEW* features and bug-**FIX**es are of course of interest as well.
 * **DOC**umentation (and website) changes are marked as such.
 
+== New in v2.2.5 (2023-05-06)
+
+=== Changes
+
+* DOC: fix man page to have correct arguments order in example, closes 
+       #867
+* FIX: cross-version issue with 2.0.5 complaining about KeyError 
+       restrict_path, closes #872
+* FIX: fail gracefully when connection(s) can't be setup e.g. in case 
+       of network error, closes #868
+
+=== Authors
+
+* Eric L
+* Frank Crawford
+
+
 == New in v2.2.4 (2023-02-27)
 
 === Changes
 
-* CHG: revert addition of Python 3.11 to 2.2 revision line
 * CHG: temp directory given by `--tempdir` isn't used as often as it 
        could to avoid cross-filesystems renaming errors (impossible to address 
        now)
 * FIX: str object has no lstat attribute when using tempdir for full 
        repository file system, closes #850
-* NEW: add Python 3.11 to the Linux versions compiled on PyPI (Windows 
-       stays on 3.10)
 
 === Authors
 
 * Eric L
 
 
 == New in v2.2.3 (2023-02-10)
```

### Comparing `rdiff-backup-2.2.4/COPYING` & `rdiff-backup-2.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/Dockerfile` & `rdiff-backup-2.2.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/Makefile` & `rdiff-backup-2.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/PKG-INFO` & `rdiff-backup-2.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdiff-backup
-Version: 2.2.4
+Version: 2.2.5
 Summary: Backup and Restore utility, easy to use, efficient, locally and remotely usable
 Home-page: https://rdiff-backup.net/
 Author: The rdiff-backup project
 Author-email: rdiff-backup-users@nongnu.org
 License: GPLv2+
 Download-URL: https://github.com/rdiff-backup/rdiff-backup/releases
 Keywords: backup,simple,easy,remote,incremental,efficient,cross-platform
```

### Comparing `rdiff-backup-2.2.4/README.adoc` & `rdiff-backup-2.2.5/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/bindep.txt` & `rdiff-backup-2.2.5/bindep.txt`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/debian/autobuild.sh` & `rdiff-backup-2.2.5/debian/autobuild.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/debian/control` & `rdiff-backup-2.2.5/debian/control`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/debian/copyright` & `rdiff-backup-2.2.5/debian/copyright`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/dist/rdiff-backup-delete.1` & `rdiff-backup-2.2.5/dist/rdiff-backup-delete.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: rdiff-backup-delete
 .\"    Author: [see the "AUTHOR(S)" section]
 .\" Generator: Asciidoctor 2.0.16
-.\"      Date: February 2023
-.\"    Manual: Rdiff-Backup-Delete Manual 2.2.4
+.\"      Date: May 2023
+.\"    Manual: Rdiff-Backup-Delete Manual 2.2.5
 .\"    Source: rdiff-backup-delete
 .\"  Language: English
 .\"
-.TH "RDIFF\-BACKUP\-DELETE" "1" "February 2023" "rdiff\-backup\-delete" "Rdiff\-Backup\-Delete Manual 2.2.4"
+.TH "RDIFF\-BACKUP\-DELETE" "1" "May 2023" "rdiff\-backup\-delete" "Rdiff\-Backup\-Delete Manual 2.2.5"
 .ie \n(.g .ds Aq \(aq
 .el       .ds Aq '
 .ss \n[.ss] 0
 .nh
 .ad l
 .de URL
 \fI\\$2\fP <\\$1>\\$3
```

### Comparing `rdiff-backup-2.2.4/dist/rdiff-backup-old.1` & `rdiff-backup-2.2.5/dist/rdiff-backup-old.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH RDIFF-BACKUP-OLD 1 "February 2023" "Version 2.2.4" "User Manuals" \" -*- nroff -*-
+.TH RDIFF-BACKUP-OLD 1 "May 2023" "Version 2.2.5" "User Manuals" \" -*- nroff -*-
 .SH NAME
 rdiff-backup \- local/remote mirror and incremental backup
 .SH SYNOPSIS
 .B rdiff-backup
 .BI [ options... ]
 .BI [[ user@ ] host1.foo:: ] source_directory
 .BI [[ user@ ] host2.foo:: ] destination_directory
```

### Comparing `rdiff-backup-2.2.4/dist/rdiff-backup-statistics.1` & `rdiff-backup-2.2.5/dist/rdiff-backup-statistics.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: rdiff-backup-statistics
 .\"    Author: [see the "AUTHOR(S)" section]
 .\" Generator: Asciidoctor 2.0.16
-.\"      Date: February 2023
-.\"    Manual: Rdiff-Backup-Statistics Manual 2.2.4
+.\"      Date: May 2023
+.\"    Manual: Rdiff-Backup-Statistics Manual 2.2.5
 .\"    Source: rdiff-backup-statistics
 .\"  Language: English
 .\"
-.TH "RDIFF\-BACKUP\-STATISTICS" "1" "February 2023" "rdiff\-backup\-statistics" "Rdiff\-Backup\-Statistics Manual 2.2.4"
+.TH "RDIFF\-BACKUP\-STATISTICS" "1" "May 2023" "rdiff\-backup\-statistics" "Rdiff\-Backup\-Statistics Manual 2.2.5"
 .ie \n(.g .ds Aq \(aq
 .el       .ds Aq '
 .ss \n[.ss] 0
 .nh
 .ad l
 .de URL
 \fI\\$2\fP <\\$1>\\$3
```

### Comparing `rdiff-backup-2.2.4/dist/rdiff-backup.1` & `rdiff-backup-2.2.5/dist/rdiff-backup.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: rdiff-backup
 .\"    Author: [see the "AUTHOR(S)" section]
 .\" Generator: Asciidoctor 2.0.16
-.\"      Date: February 2023
-.\"    Manual: Manual 2.2.4
+.\"      Date: May 2023
+.\"    Manual: Manual 2.2.5
 .\"    Source: rdiff-backup
 .\"  Language: English
 .\"
-.TH "RDIFF\-BACKUP" "1" "February 2023" "rdiff\-backup" "Manual 2.2.4"
+.TH "RDIFF\-BACKUP" "1" "May 2023" "rdiff\-backup" "Manual 2.2.5"
 .ie \n(.g .ds Aq \(aq
 .el       .ds Aq '
 .ss \n[.ss] 0
 .nh
 .ad l
 .de URL
 \fI\\$2\fP <\\$1>\\$3
@@ -875,15 +875,15 @@
 rdiff\-backup \-\-server\fP\*(Aq.
 Using \fB\-\-remote\-schema\fP, rdiff\-backup can invoke an arbitrary command in order to open up a remote pipe.
 For instance,
 .sp
 .if n .RS 4
 .nf
 .fam C
-rdiff\-backup backup \-\-remote\-schema \*(Aqcd /usr; {h}\*(Aq \(rs
+rdiff\-backup \-\-remote\-schema \*(Aqcd /usr; {h}\*(Aq backup \(rs
                     foo \*(Aqrdiff\-backup server\*(Aq::bar
 .fam
 .fi
 .if n .RE
 .sp
 is basically equivalent to (but slower than)
 .sp
```

### Comparing `rdiff-backup-2.2.4/docs/CODING.adoc` & `rdiff-backup-2.2.5/docs/CODING.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/DEVELOP.adoc` & `rdiff-backup-2.2.5/docs/DEVELOP.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/DOCUMENTATION.adoc` & `rdiff-backup-2.2.5/docs/DOCUMENTATION.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/FAQ.adoc` & `rdiff-backup-2.2.5/docs/FAQ.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/README.adoc` & `rdiff-backup-2.2.5/docs/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/Windows-DEVELOP.adoc` & `rdiff-backup-2.2.5/docs/Windows-DEVELOP.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/Windows-README.adoc` & `rdiff-backup-2.2.5/docs/Windows-README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/_layouts/default.html` & `rdiff-backup-2.2.5/docs/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/_site_README.adoc` & `rdiff-backup-2.2.5/docs/_site_README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/api/README.adoc` & `rdiff-backup-2.2.5/docs/api/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/api/index.adoc` & `rdiff-backup-2.2.5/docs/api/index.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/api/v200.adoc` & `rdiff-backup-2.2.5/docs/api/v200.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/api/v201.adoc` & `rdiff-backup-2.2.5/docs/api/v201.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/README.adoc` & `rdiff-backup-2.2.5/docs/arch/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/actions.drawio.svg` & `rdiff-backup-2.2.5/docs/arch/actions.drawio.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/classes.svg` & `rdiff-backup-2.2.5/docs/arch/classes.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/completion.adoc` & `rdiff-backup-2.2.5/docs/arch/completion.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/error_policy.adoc` & `rdiff-backup-2.2.5/docs/arch/error_policy.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/index.adoc` & `rdiff-backup-2.2.5/docs/arch/index.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/locations.adoc` & `rdiff-backup-2.2.5/docs/arch/locations.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/packages.svg` & `rdiff-backup-2.2.5/docs/arch/packages.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/plugins/README.adoc` & `rdiff-backup-2.2.5/docs/arch/plugins/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/plugins/actions.adoc` & `rdiff-backup-2.2.5/docs/arch/plugins/actions.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/plugins/index.adoc` & `rdiff-backup-2.2.5/docs/arch/plugins/index.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/plugins/meta.adoc` & `rdiff-backup-2.2.5/docs/arch/plugins/meta.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.puml` & `rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.puml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.sh` & `rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/rdiff_backup_classes.svg` & `rdiff-backup-2.2.5/docs/arch/rdiff_backup_classes.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/rdiffbackup_architecture.svg` & `rdiff-backup-2.2.5/docs/arch/rdiffbackup_architecture.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/arch/repository_format.adoc` & `rdiff-backup-2.2.5/docs/arch/repository_format.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/credits.adoc` & `rdiff-backup-2.2.5/docs/credits.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/asciidoctor.css` & `rdiff-backup-2.2.5/docs/css/asciidoctor.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/coderay.css` & `rdiff-backup-2.2.5/docs/css/coderay.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/fontawesome.css` & `rdiff-backup-2.2.5/docs/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/fontawesome.min.css` & `rdiff-backup-2.2.5/docs/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/foundation.css` & `rdiff-backup-2.2.5/docs/css/foundation.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/foundation.min.css` & `rdiff-backup-2.2.5/docs/css/foundation.min.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/css/normalize.css` & `rdiff-backup-2.2.5/docs/css/normalize.css`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/examples.adoc` & `rdiff-backup-2.2.5/docs/examples.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/features.adoc` & `rdiff-backup-2.2.5/docs/features.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/index.adoc` & `rdiff-backup-2.2.5/docs/index.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.abide.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.abide.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.accordion.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.accordion.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.alert.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.alert.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.clearing.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.clearing.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.dropdown.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.dropdown.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.equalizer.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.equalizer.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.interchange.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.interchange.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.joyride.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.joyride.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.magellan.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.magellan.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.offcanvas.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.offcanvas.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.orbit.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.orbit.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.reveal.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.reveal.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.slider.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.slider.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.tab.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.tab.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.tooltip.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.tooltip.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation/foundation.topbar.js` & `rdiff-backup-2.2.5/docs/js/foundation/foundation.topbar.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/foundation.min.js` & `rdiff-backup-2.2.5/docs/js/foundation.min.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/js/toc.js` & `rdiff-backup-2.2.5/docs/js/toc.js`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/migration.adoc` & `rdiff-backup-2.2.5/docs/migration.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/other/rdiff-backup-old.1.html` & `rdiff-backup-2.2.5/docs/other/rdiff-backup-old.1.html`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/other/related.adoc` & `rdiff-backup-2.2.5/docs/other/related.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/rdiff-backup-delete.1.adoc` & `rdiff-backup-2.2.5/docs/rdiff-backup-delete.1.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/rdiff-backup-old.1.template` & `rdiff-backup-2.2.5/docs/rdiff-backup-old.1.template`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/rdiff-backup-statistics.1.adoc` & `rdiff-backup-2.2.5/docs/rdiff-backup-statistics.1.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/rdiff-backup.1.adoc` & `rdiff-backup-2.2.5/docs/rdiff-backup.1.adoc`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
 * or a URI of the form '[.code]``ssh://[user@]hostname[:port]``'.
 
 The default remote schema is '[.code]``ssh -C {h} rdiff-backup --server``' where '[.code]``host_info``' is substituted for '[.code]``{h}``'.
 So if the '[.code]``host_info``' is '[.code]``user@host.net``', then rdiff-backup runs '[.code]``ssh user@host.net rdiff-backup --server``'.
 Using *--remote-schema*, rdiff-backup can invoke an arbitrary command in order to open up a remote pipe.
 For instance,
 
- rdiff-backup backup --remote-schema 'cd /usr; {h}' \
+ rdiff-backup --remote-schema 'cd /usr; {h}' backup \
                      foo 'rdiff-backup server'::bar
 
 is basically equivalent to (but slower than)
 
  rdiff-backup backup foo /usr/bar
 
 Concerning quoting, if for some reason you need to put two consecutive colons in the '[.code]``host_info``' section of a '[.code]``host_info::pathname``' argument, or in the pathname of a local file, you can quote one of them by prepending a backslash.
```

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-128.png` & `rdiff-backup-2.2.5/docs/resources/logo-128.png`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-32.png` & `rdiff-backup-2.2.5/docs/resources/logo-32.png`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-32.svg` & `rdiff-backup-2.2.5/docs/resources/logo-32.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-a.png` & `rdiff-backup-2.2.5/docs/resources/logo-a.png`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-a.svg` & `rdiff-backup-2.2.5/docs/resources/logo-a.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-banner.png` & `rdiff-backup-2.2.5/docs/resources/logo-banner.png`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/docs/resources/logo-banner.svg` & `rdiff-backup-2.2.5/docs/resources/logo-banner.svg`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/requirements.txt` & `rdiff-backup-2.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/requs/00.txt` & `rdiff-backup-2.2.5/requs/00.txt`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/setup.py` & `rdiff-backup-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/_librsyncmodule.c` & `rdiff-backup-2.2.5/src/_librsyncmodule.c`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/cmodule.c` & `rdiff-backup-2.2.5/src/cmodule.c`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/FilenameMapping.py` & `rdiff-backup-2.2.5/src/rdiff_backup/FilenameMapping.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Globals.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,18 @@
 # rdiff-backup-data dir.  These can sometimes take up a lot of space.
 file_statistics = 1
 
 # On the backup writer connection, holds the root incrementing branch
 # object.  Access is provided to increment error counts.
 ITRB = None
 
+# If this is set, it indicates that the remote connection should only
+# deal with paths inside of restrict_path.
+restrict_path = None  # compat200
+
 # If set, a file will be marked as changed if its inode changes.  See
 # the man page under --no-compare-inode for more information.
 compare_inode = 1
 
 # If set, directories can be fsync'd just like normal files, to
 # guarantee that any changes have been comitted to disk.
 fsync_directories = None
```

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Hardlink.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Hardlink.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Main.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Main.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Rdiff.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Rdiff.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Security.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Security.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     Also set the global variable _restrict_path_list as list of path components.
     It is assumed that the new path is a proper path, else function will fail.
     """
     assert rp.conn is Globals.local_connection, (
         "Function works locally not over '{conn}'.".format(conn=rp.conn))
     global _restrict_path, _restrict_path_list
     _restrict_path = rp.normalize().path
+    Globals.restrict_path = _restrict_path  # compat200
     _restrict_path_list = _restrict_path.split(b"/")
 
 
 def vet_request(request, arglist):
     """Examine request for security violations"""
     if _security_level == "override":
         return
```

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/SetConnections.py` & `rdiff-backup-2.2.5/src/rdiff_backup/SetConnections.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/Time.py` & `rdiff-backup-2.2.5/src/rdiff_backup/Time.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/backup.py` & `rdiff-backup-2.2.5/src/rdiff_backup/backup.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/compare.py` & `rdiff-backup-2.2.5/src/rdiff_backup/compare.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/connection.py` & `rdiff-backup-2.2.5/src/rdiff_backup/connection.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/fs_abilities.py` & `rdiff-backup-2.2.5/src/rdiff_backup/fs_abilities.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/hash.py` & `rdiff-backup-2.2.5/src/rdiff_backup/hash.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/increment.py` & `rdiff-backup-2.2.5/src/rdiff_backup/increment.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/iterfile.py` & `rdiff-backup-2.2.5/src/rdiff_backup/iterfile.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/librsync.py` & `rdiff-backup-2.2.5/src/rdiff_backup/librsync.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/log.py` & `rdiff-backup-2.2.5/src/rdiff_backup/log.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/longname.py` & `rdiff-backup-2.2.5/src/rdiff_backup/longname.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/manage.py` & `rdiff-backup-2.2.5/src/rdiff_backup/manage.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/regress.py` & `rdiff-backup-2.2.5/src/rdiff_backup/regress.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/restore.py` & `rdiff-backup-2.2.5/src/rdiff_backup/restore.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/robust.py` & `rdiff-backup-2.2.5/src/rdiff_backup/robust.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/rorpiter.py` & `rdiff-backup-2.2.5/src/rdiff_backup/rorpiter.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/rpath.py` & `rdiff-backup-2.2.5/src/rdiff_backup/rpath.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/run_delete.py` & `rdiff-backup-2.2.5/src/rdiff_backup/run_delete.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/run_stats.py` & `rdiff-backup-2.2.5/src/rdiff_backup/run_stats.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/selection.py` & `rdiff-backup-2.2.5/src/rdiff_backup/selection.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/statistics.py` & `rdiff-backup-2.2.5/src/rdiff_backup/statistics.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup/user_group.py` & `rdiff-backup-2.2.5/src/rdiff_backup/user_group.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup.egg-info/PKG-INFO` & `rdiff-backup-2.2.5/src/rdiff_backup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdiff-backup
-Version: 2.2.4
+Version: 2.2.5
 Summary: Backup and Restore utility, easy to use, efficient, locally and remotely usable
 Home-page: https://rdiff-backup.net/
 Author: The rdiff-backup project
 Author-email: rdiff-backup-users@nongnu.org
 License: GPLv2+
 Download-URL: https://github.com/rdiff-backup/rdiff-backup/releases
 Keywords: backup,simple,easy,remote,incremental,efficient,cross-platform
```

### Comparing `rdiff-backup-2.2.4/src/rdiff_backup.egg-info/SOURCES.txt` & `rdiff-backup-2.2.5/src/rdiff_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/__init__.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,17 @@
 
     # version of the action
     __version__ = "0.0.0"
 
     # list of parent parsers as defined above
     parent_parsers = []
 
+    # connection status
+    conn_status = Globals.RET_CODE_OK
+
     @classmethod
     def get_name(cls):
         """
         Return the name of the Action class.
 
         Children classes only need to define the class member 'name'.
         """
@@ -442,16 +445,14 @@
             ret_code |= Globals.RET_CODE_ERR
         return ret_code
 
     def connect(self):
         """
         Connect to potentially provided locations arguments, remote or local.
 
-        Defines the current time as being the time of a potentially upcoming
-        backup.
         Returns self, to be used as context manager.
         """
 
         if 'locations' in self.values:
             # TODO encapsulate the following lines into one
             # connections/connections_mgr construct, so that the action doesn't
             # need to care about cmdpairs and Security (which would become a
@@ -462,51 +463,47 @@
                 ssh_compression=self.values.ssh_compression,
                 remote_tempdir=self.remote_tempdir,
                 term_verbosity=log.Log.term_verbosity
             )
             Security.initialize(self.get_security_class(), cmdpairs)
             self.connected_locations = list(
                 map(SetConnections.get_connected_rpath, cmdpairs))
+
+            # if a connection is None, it's an error
+            for conn, loc in zip(self.connected_locations,
+                                 self.values.locations):
+                if conn is None:
+                    log.Log("Location '{lo}' couldn't be connected.".format(
+                        lo=loc), log.ERROR)
+                    self.conn_status = Globals.RET_CODE_ERR
         else:
             Security.initialize(self.get_security_class(), [])
             self.connected_locations = []
 
-        # once the connection is set, we can define "now" as being the current
-        # time, unless the user defined a fixed a current time.
-        Time.set_current_time(self.values.current_time)
-
         return self
 
     def check(self):
         """
         Checks that all connections are looking fine.
 
         Whatever can be checked without changing anything to the environment.
         Return 0 if everything looked good, else an error code.
         """
-        ret_code = Globals.RET_CODE_OK
-
-        if 'locations' not in self.values:
-            return ret_code
-
-        # if a connection is None, it's an error
-        for conn, loc in zip(self.connected_locations, self.values.locations):
-            if conn is None:
-                log.Log("Location '{lo}' couldn't be connected.".format(
-                    lo=loc), log.ERROR)
-                ret_code |= Globals.RET_CODE_ERR
-
-        return ret_code
+        return self.conn_status
 
     def setup(self):
         """
         Prepare the execution of the action.
 
         Return 0 if everything looked good, else an error code.
         """
+        # we can define "now" as being the current time,
+        # unless the user defined a fixed a current time.
+        Time.set_current_time(self.values.current_time)
+
         if self.values.tempdir:
             # At least until Python 3.10, the module tempfile doesn't work
             # properly,
             # especially under Windows, if tempdir is stored as bytes.
             # See https://github.com/python/cpython/pull/20442
             tempfile.tempdir = self.values.tempdir
         # Set default change ownership flag, umask, relay regexps
@@ -522,14 +519,20 @@
         """
         Execute the given action.
 
         Return 0 if everything looked good, else an error code.
         """
         return Globals.RET_CODE_OK
 
+    def is_connection_ok(self):
+        """
+        Return True if connection is OK, False else
+        """
+        return not self.conn_status & Globals.RET_CODE_ERR
+
     def _operate_regress(self, try_regress=True,
                          noticeable=False, force=False):
         """
         Check the given repository and regress it if necessary
 
         Parameter force enforces a regress even if the repo doesn't need it.
         """
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/backup.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         subparser.add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=2,
             help="locations of SOURCE_DIR and to which REPOSITORY to backup")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.dir = directory.ReadDir(self.connected_locations[0],
                                          self.values.force)
             self.repo = repository.Repo(
                 self.connected_locations[1], self.values.force,
                 must_be_writable=True, must_exist=False,
                 create_full_path=self.values.create_full_path
             )
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/calculate.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/calculate.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/compare.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=2,
             help="locations of SOURCE_DIR and backup REPOSITORY to compare"
                  " (same order as for a backup)")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.dir = directory.ReadDir(self.connected_locations[0],
                                          self.values.force)
             self.repo = repository.Repo(
                 self.connected_locations[1], self.values.force,
                 must_be_writable=False, must_exist=True, can_be_sub_path=True
             )
         return conn_value
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/complete.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/complete.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/info.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/info.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/list_.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/list_.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         entity_parsers["increments"].add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=1,
             help="location of repository to list increments from")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.repo = repository.Repo(
                 self.connected_locations[0], self.values.force,
                 must_be_writable=False, must_exist=True, can_be_sub_path=True
             )
         return conn_value
 
     def check(self):
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/regress.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/regress.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         subparser.add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=1,
             help="location of repository to check and possibly regress")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.repo = repository.Repo(
                 self.connected_locations[0], self.values.force,
                 must_be_writable=True, must_exist=True
             )
         return conn_value
 
     def check(self):
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/remove.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         entity_parsers["increments"].add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=1,
             help="location of repository to remove increments from")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.repo = repository.Repo(
                 self.connected_locations[0], self.values.force,
                 must_be_writable=True, must_exist=True
             )
         return conn_value
 
     def check(self):
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/restore.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         subparser.add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=2,
             help="locations of backup REPOSITORY/INCREMENT and to which TARGET_DIR to restore")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.repo = repository.Repo(
                 self.connected_locations[0], self.values.force,
                 must_be_writable=False, must_exist=True, can_be_sub_path=True
             )
             self.dir = directory.WriteDir(self.connected_locations[1],
                                           self.values.force,
                                           self.values.create_full_path)
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/server.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(self, values):
         super().__init__(values)
         if 'debug' in self.values and self.values.debug:
             self._set_breakpoint()
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             Security.initialize(self.get_security_class(), [],
                                 security_level=self.values.restrict_mode,
                                 restrict_path=self.values.restrict_path)
         return conn_value
 
     def run(self):
         ret_code = super().run()
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/test.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions/verify.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         subparser.add_argument(
             "locations", metavar="[[USER@]SERVER::]PATH", nargs=1,
             help="location of repository where to check files' hashes")
         return subparser
 
     def connect(self):
         conn_value = super().connect()
-        if conn_value:
+        if conn_value.is_connection_ok():
             self.repo = repository.Repo(
                 self.connected_locations[0], self.values.force,
                 must_be_writable=False, must_exist=True, can_be_sub_path=True
             )
         return conn_value
 
     def check(self):
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/actions_mgr.py` & `rdiff-backup-2.2.5/src/rdiffbackup/actions_mgr.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/arguments.py` & `rdiff-backup-2.2.5/src/rdiffbackup/arguments.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/__init__.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/_dir_shadow.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/_dir_shadow.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/_repo_shadow.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/_repo_shadow.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/directory.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/directory.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/fs_abilities.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/fs_abilities.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/map/filenames.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/map/filenames.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/map/hardlinks.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/map/hardlinks.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/map/longnames.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/map/longnames.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/map/owners.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/map/owners.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/locations/repository.py` & `rdiff-backup-2.2.5/src/rdiffbackup/locations/repository.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta/__init__.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta/acl_posix.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta/acl_posix.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta/acl_win.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta/acl_win.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta/ea.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta/ea.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta/stdattr.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta/stdattr.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/meta_mgr.py` & `rdiff-backup-2.2.5/src/rdiffbackup/meta_mgr.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/run.py` & `rdiff-backup-2.2.5/src/rdiffbackup/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         log.Log("Action {ac} failed on step {st}".format(
             ac=parsed_args.action, st="pre_check"), log.ERROR)
         return ret_val
 
     # now start for real, conn_act and action are the same object
     with action.connect() as conn_act:
 
+        if not conn_act.is_connection_ok():
+            log.Log("Action {ac} failed on step {st}".format(
+                ac=parsed_args.action, st="connect"), log.ERROR)
+            return conn_act.conn_status
+
         # For test purposes only, hence we allow ourselves to overwrite a
         # "private" variable
         if security_override:
             from rdiff_backup import Security
             Security._security_level = "override"
 
         ret_val |= conn_act.check()
```

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/argopts.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/argopts.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/locking.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/locking.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/plugins.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/quoting.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/quoting.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/safestr.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/safestr.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/simpleps.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/simpleps.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/src/rdiffbackup/utils/usrgrp.py` & `rdiff-backup-2.2.5/src/rdiffbackup/utils/usrgrp.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/FilenameMappingtest.py` & `rdiff-backup-2.2.5/testing/FilenameMappingtest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_backuprestore_test.py` & `rdiff-backup-2.2.5/testing/action_backuprestore_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,9 +275,21 @@
             fileset.remove_fileset(self.base_dir, self.from1_struct)
             fileset.remove_fileset(self.base_dir, self.from2_struct)
             fileset.remove_fileset(self.base_dir, {"bak": {"type": "dir"}})
             fileset.remove_fileset(self.base_dir, {"to1": {"type": "dir"}})
             fileset.remove_fileset(self.base_dir, {"to2": {"type": "dir"}})
 
 
+class ConnectionHandlingTest(unittest.TestCase):
+    """
+    Test handling of wrong connection
+    """
+
+    def test_wrong_connection(self):
+        # we backup using a non existing destination location
+        self.assertNotEqual(comtst.rdiff_backup_action(
+            True, True, ".", "doesnotexist::/some_dir",
+            ("--api-version", "201"), b"backup", ()), 0)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `rdiff-backup-2.2.4/testing/action_calculate_test.py` & `rdiff-backup-2.2.5/testing/action_calculate_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_compare_test.py` & `rdiff-backup-2.2.5/testing/action_compare_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_complete_test.py` & `rdiff-backup-2.2.5/testing/action_complete_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_list_test.py` & `rdiff-backup-2.2.5/testing/action_list_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_regress_test.py` & `rdiff-backup-2.2.5/testing/action_regress_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_remove_test.py` & `rdiff-backup-2.2.5/testing/action_remove_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_test_test.py` & `rdiff-backup-2.2.5/testing/action_test_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/action_verify_test.py` & `rdiff-backup-2.2.5/testing/action_verify_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/api_test.py` & `rdiff-backup-2.2.5/testing/api_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/backuptest.py` & `rdiff-backup-2.2.5/testing/backuptest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/benchmark.py` & `rdiff-backup-2.2.5/testing/benchmark.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/cmdlinetest.py` & `rdiff-backup-2.2.5/testing/cmdlinetest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/commontest.py` & `rdiff-backup-2.2.5/testing/commontest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/comparetest.py` & `rdiff-backup-2.2.5/testing/comparetest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/connectiontest.py` & `rdiff-backup-2.2.5/testing/connectiontest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/ctest.py` & `rdiff-backup-2.2.5/testing/ctest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/eas_aclstest.py` & `rdiff-backup-2.2.5/testing/eas_aclstest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/errorsrecovertest.py` & `rdiff-backup-2.2.5/testing/errorsrecovertest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/fileset.py` & `rdiff-backup-2.2.5/testing/fileset.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/find-max-ram.py` & `rdiff-backup-2.2.5/testing/find-max-ram.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/fs_abilitiestest.py` & `rdiff-backup-2.2.5/testing/fs_abilitiestest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/hardlinktest.py` & `rdiff-backup-2.2.5/testing/hardlinktest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/hashtest.py` & `rdiff-backup-2.2.5/testing/hashtest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/incrementtest.py` & `rdiff-backup-2.2.5/testing/incrementtest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/iterfiletest.py` & `rdiff-backup-2.2.5/testing/iterfiletest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/killtest.py` & `rdiff-backup-2.2.5/testing/killtest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/librsynctest.py` & `rdiff-backup-2.2.5/testing/librsynctest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/location_lock_test.py` & `rdiff-backup-2.2.5/testing/location_lock_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/location_map_filenames_test.py` & `rdiff-backup-2.2.5/testing/location_map_filenames_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/location_map_hardlinks_test.py` & `rdiff-backup-2.2.5/testing/location_map_hardlinks_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/longnametest.py` & `rdiff-backup-2.2.5/testing/longnametest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/metadatatest.py` & `rdiff-backup-2.2.5/testing/metadatatest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/rdb_arguments.py` & `rdiff-backup-2.2.5/testing/rdb_arguments.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/rdiffbackupdeletetest.py` & `rdiff-backup-2.2.5/testing/rdiffbackupdeletetest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/rdifftest.py` & `rdiff-backup-2.2.5/testing/rdifftest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/readonly_actions_test.py` & `rdiff-backup-2.2.5/testing/readonly_actions_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/regressfailedlongname.sh` & `rdiff-backup-2.2.5/testing/regressfailedlongname.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/regresstest.py` & `rdiff-backup-2.2.5/testing/regresstest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/resourceforktest.py` & `rdiff-backup-2.2.5/testing/resourceforktest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/restoretest.py` & `rdiff-backup-2.2.5/testing/restoretest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/robusttest.py` & `rdiff-backup-2.2.5/testing/robusttest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/roottest.py` & `rdiff-backup-2.2.5/testing/roottest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/rorpitertest.py` & `rdiff-backup-2.2.5/testing/rorpitertest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/rpathtest.py` & `rdiff-backup-2.2.5/testing/rpathtest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/securitytest.py` & `rdiff-backup-2.2.5/testing/securitytest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/selectiontest.py` & `rdiff-backup-2.2.5/testing/selectiontest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/server.py` & `rdiff-backup-2.2.5/testing/server.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/setconnectionstest.py` & `rdiff-backup-2.2.5/testing/setconnectionstest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/statisticstest.py` & `rdiff-backup-2.2.5/testing/statisticstest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/test_with_profiling.py` & `rdiff-backup-2.2.5/testing/test_with_profiling.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/timetest.py` & `rdiff-backup-2.2.5/testing/timetest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/user_grouptest.py` & `rdiff-backup-2.2.5/testing/user_grouptest.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/testing/utils_simpleps_test.py` & `rdiff-backup-2.2.5/testing/utils_simpleps_test.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/build_wheels.sh` & `rdiff-backup-2.2.5/tools/build_wheels.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/check_links_in_adoc.py` & `rdiff-backup-2.2.5/tools/check_links_in_adoc.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/completions/bash/rdiff-backup` & `rdiff-backup-2.2.5/tools/completions/bash/rdiff-backup`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/crossversion/README.adoc` & `rdiff-backup-2.2.5/tools/crossversion/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/crossversion/Vagrantfile` & `rdiff-backup-2.2.5/tools/crossversion/Vagrantfile`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/crossversion/playbook-provision.yml` & `rdiff-backup-2.2.5/tools/crossversion/playbook-provision.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/crossversion/playbook-smoke-test.yml` & `rdiff-backup-2.2.5/tools/crossversion/playbook-smoke-test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
   - name: call local rdiff-backup info
     command: rdiff-backup info
     delegate_to: localhost
 
   - name: check that the remote rdiff-backup works
     command: >
       rdiff-backup --remote-schema '{{ remote_schema }}' --test-server
-      {{ test_user }}\@{{ test_server }}::{{ remote_base_dir }}/simplebackup
+      {{ test_user }}\@{{ test_server }}::{{ remote_base_dir }}
     delegate_to: localhost
 
   - name: make a simple backup from the local directory to remote repo
     command: >
       rdiff-backup --remote-schema '{{ remote_schema }}'
       . {{ test_user }}\@{{ test_server }}::{{ remote_base_dir }}/simplebackup
     delegate_to: localhost
```

### Comparing `rdiff-backup-2.2.4/tools/get_changelog_since.sh` & `rdiff-backup-2.2.5/tools/get_changelog_since.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/make_release.sh` & `rdiff-backup-2.2.5/tools/make_release.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/compress-rdiff-backup-increments` & `rdiff-backup-2.2.5/tools/misc/compress-rdiff-backup-increments`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/create_fs_as_user.sh` & `rdiff-backup-2.2.5/tools/misc/create_fs_as_user.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/deldiffs.sh` & `rdiff-backup-2.2.5/tools/misc/deldiffs.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/find2dirs` & `rdiff-backup-2.2.5/tools/misc/find2dirs`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/generate-code-overview.sh` & `rdiff-backup-2.2.5/tools/misc/generate-code-overview.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/init_files.py` & `rdiff-backup-2.2.5/tools/misc/init_files.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/librsync-many-files.py` & `rdiff-backup-2.2.5/tools/misc/librsync-many-files.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/python-rdiff` & `rdiff-backup-2.2.5/tools/misc/python-rdiff`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/rdiff-backup-regress.adoc` & `rdiff-backup-2.2.5/tools/misc/rdiff-backup-regress.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/rdiff-backup-regress.sh` & `rdiff-backup-2.2.5/tools/misc/rdiff-backup-regress.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/rdiff-backup-wrap` & `rdiff-backup-2.2.5/tools/misc/rdiff-backup-wrap`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/remove-comments.py` & `rdiff-backup-2.2.5/tools/misc/remove-comments.py`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/misc/setup_dev_archlinux.sh` & `rdiff-backup-2.2.5/tools/misc/setup_dev_archlinux.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/prepare_api_doc.sh` & `rdiff-backup-2.2.5/tools/prepare_api_doc.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/rdiff-backup.spec.template` & `rdiff-backup-2.2.5/tools/rdiff-backup.spec.template`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/rdiff-backup.spec.template-fedora` & `rdiff-backup-2.2.5/tools/rdiff-backup.spec.template-fedora`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/setup-testfiles.sh` & `rdiff-backup-2.2.5/tools/setup-testfiles.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/win_build_librsync.sh` & `rdiff-backup-2.2.5/tools/win_build_librsync.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/win_build_rdiffbackup.sh` & `rdiff-backup-2.2.5/tools/win_build_rdiffbackup.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/win_package_rdiffbackup.sh` & `rdiff-backup-2.2.5/tools/win_package_rdiffbackup.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/win_provision.sh` & `rdiff-backup-2.2.5/tools/win_provision.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/win_test_rdiffbackup.sh` & `rdiff-backup-2.2.5/tools/win_test_rdiffbackup.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/README.adoc` & `rdiff-backup-2.2.5/tools/windows/README.adoc`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/Vagrantfile` & `rdiff-backup-2.2.5/tools/windows/Vagrantfile`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/group_vars/windows_hosts/generic.yml` & `rdiff-backup-2.2.5/tools/windows/group_vars/windows_hosts/generic.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/playbook-debug-rdiff-backup.yml` & `rdiff-backup-2.2.5/tools/windows/playbook-debug-rdiff-backup.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/playbook-pipeline.yml` & `rdiff-backup-2.2.5/tools/windows/playbook-pipeline.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/playbook-provision.yml` & `rdiff-backup-2.2.5/tools/windows/playbook-provision.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/playbook-test-rdiff-backup.yml` & `rdiff-backup-2.2.5/tools/windows/playbook-test-rdiff-backup.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/.yamllint` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/.yamllint`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/CHANGELOG.md` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/LICENSE.md` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/README.md` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/README.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/defaults/main.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/files/dynamic-motd.sh` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/files/dynamic-motd.sh`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/admin.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/admin.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/auto-updates.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/auto-updates.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/config.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/config.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/install.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/install.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/main.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/security.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/security.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/services.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/services.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/tasks/users.yml` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/tasks/users.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_dnf_automatic.conf.j2` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_dnf_automatic.conf.j2`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_yum_yum-cron-hourly.conf.j2` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_yum_yum-cron-hourly.conf.j2`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/rh-base/templates/etc_yum_yum-cron.conf.j2` & `rdiff-backup-2.2.5/tools/windows/roles/rh-base/templates/etc_yum_yum-cron.conf.j2`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/.travis.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/.travis.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/CHANGELOG.md` & `rdiff-backup-2.2.5/tools/windows/roles/samba/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/LICENSE.md` & `rdiff-backup-2.2.5/tools/windows/roles/samba/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/README.md` & `rdiff-backup-2.2.5/tools/windows/roles/samba/README.md`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/defaults/main.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/meta/main.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/meta/main.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/tasks/main.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/templates/smb.conf.j2` & `rdiff-backup-2.2.5/tools/windows/roles/samba/templates/smb.conf.j2`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/vars/os_Debian.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/vars/os_Debian.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tools/windows/roles/samba/vars/os_RedHat.yml` & `rdiff-backup-2.2.5/tools/windows/roles/samba/vars/os_RedHat.yml`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tox.ini` & `rdiff-backup-2.2.5/tox.ini`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tox_dist.ini` & `rdiff-backup-2.2.5/tox_dist.ini`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tox_root.ini` & `rdiff-backup-2.2.5/tox_root.ini`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tox_slow.ini` & `rdiff-backup-2.2.5/tox_slow.ini`

 * *Files identical despite different names*

### Comparing `rdiff-backup-2.2.4/tox_win.ini` & `rdiff-backup-2.2.5/tox_win.ini`

 * *Files identical despite different names*

