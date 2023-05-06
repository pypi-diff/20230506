# Comparing `tmp/pretext-1.5.3.dev20230505.tar.gz` & `tmp/pretext-1.5.3.dev20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230505.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230506.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230505.tar` & `pretext-1.5.3.dev20230506.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/README.md
--rw-r--r--   0        0        0     1440 2023-05-05 20:46:30.750810 pretext-1.5.3.dev20230505/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/core/__init__.py
--rw-r--r--   0        0        0   173946 2023-05-05 20:46:32.998828 pretext-1.5.3.dev20230505/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/core/resources.py
--rw-r--r--   0        0        0  1053273 2023-05-05 20:46:32.994828 pretext-1.5.3.dev20230505/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-05 20:46:33.070829 pretext-1.5.3.dev20230505/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-05 20:46:33.098829 pretext-1.5.3.dev20230505/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-05 20:46:33.090829 pretext-1.5.3.dev20230505/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-05 20:46:33.102829 pretext-1.5.3.dev20230505/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-05 20:46:30.750810 pretext-1.5.3.dev20230505/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230505/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/README.md
+-rw-r--r--   0        0        0     1440 2023-05-06 06:17:26.843531 pretext-1.5.3.dev20230506/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/core/__init__.py
+-rw-r--r--   0        0        0   173946 2023-05-06 06:17:31.727570 pretext-1.5.3.dev20230506/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/core/resources.py
+-rw-r--r--   0        0        0  1052517 2023-05-06 06:17:31.727570 pretext-1.5.3.dev20230506/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-06 06:17:31.771571 pretext-1.5.3.dev20230506/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-06 06:17:31.791571 pretext-1.5.3.dev20230506/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-06 06:17:31.787571 pretext-1.5.3.dev20230506/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-06 06:17:26.843531 pretext-1.5.3.dev20230506/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230506/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230505/LICENSE` & `pretext-1.5.3.dev20230506/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/README.md` & `pretext-1.5.3.dev20230506/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/__init__.py` & `pretext-1.5.3.dev20230506/pretext/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = '49b6569fc697733cea093afd581c8cc7c26cf7dd'
+CORE_COMMIT = 'd658fc893c209a8f31052b661a52fae381f7ff20'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230505/pretext/build.py` & `pretext-1.5.3.dev20230506/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/cli.py` & `pretext-1.5.3.dev20230506/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/codechat.py` & `pretext-1.5.3.dev20230506/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230506/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/core/pretext.py` & `pretext-1.5.3.dev20230506/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/core/resources.py` & `pretext-1.5.3.dev20230506/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/core/resources.zip` & `pretext-1.5.3.dev20230506/pretext/core/resources.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 1053273 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/utilities/
--rw-r--r--  2.0 unx    11766 b- defN 23-May-05 20:46 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx   262590 b- defN 23-May-05 20:46 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-05 20:46 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-05 20:46 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-05 20:46 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-05 20:46 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-05 20:46 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-May-05 20:46 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-05 20:46 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-05 20:46 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-05 20:46 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    69315 b- defN 23-May-05 20:46 xsl/pretext-braille.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-05 20:46 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   544147 b- defN 23-May-05 20:46 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    65459 b- defN 23-May-05 20:46 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-05 20:46 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-05 20:46 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-05 20:46 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-05 20:46 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-05 20:46 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-05 20:46 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139661 b- defN 23-May-05 20:46 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-05 20:46 xsl/README.md
--rw-r--r--  2.0 unx     2740 b- defN 23-May-05 20:46 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   608699 b- defN 23-May-05 20:46 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-May-05 20:46 xsl/entities.ent
--rw-r--r--  2.0 unx     2846 b- defN 23-May-05 20:46 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-05 20:46 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-05 20:46 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-05 20:46 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   541182 b- defN 23-May-05 20:46 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-05 20:46 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-05 20:46 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    39922 b- defN 23-May-05 20:46 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-05 20:46 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-05 20:46 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-05 20:46 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-05 20:46 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-05 20:46 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-05 20:46 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-May-05 20:46 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-May-05 20:46 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-05 20:46 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-May-05 20:46 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-05 20:46 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    17285 b- defN 23-May-05 20:46 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-05 20:46 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-May-05 20:46 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-05 20:46 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-05 20:46 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-05 20:46 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-05 20:46 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-05 20:46 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-05 20:46 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-05 20:46 xsl/localizations/README.md
--rw-r--r--  2.0 unx     2227 b- defN 23-May-05 20:46 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-05 20:46 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-05 20:46 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-05 20:46 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-May-05 20:46 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-05 20:46 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-05 20:46 xsl/localizations/pt-PT.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/support/play-button/
--rw-r--r--  2.0 unx     5800 b- defN 23-May-05 20:46 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-05 20:46 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-05 20:46 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-May-05 20:46 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-May-05 20:46 xsl/support/README.md
--rw-r--r--  2.0 unx      486 b- defN 23-May-05 20:46 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5241 b- defN 23-May-05 20:46 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-May-05 20:46 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-May-05 20:46 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-May-05 20:46 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     3024 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx   133917 b- defN 23-May-05 20:46 schema/pretext.xml
--rw-r--r--  2.0 unx   124561 b- defN 23-May-05 20:46 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-May-05 20:46 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx      326 b- defN 23-May-05 20:46 schema/xml.xsd
--rw-r--r--  2.0 unx    57960 b- defN 23-May-05 20:46 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-May-05 20:46 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 23-May-05 20:46 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-May-05 20:46 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    25290 b- defN 23-May-05 20:46 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-May-05 20:46 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   101402 b- defN 23-May-05 20:46 schema/pretext.rng
--rw-r--r--  2.0 unx     2446 b- defN 23-May-05 20:46 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-05 20:46 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-05 20:46 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-05 20:46 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     1280 b- defN 23-May-05 20:46 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-05 20:46 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-05 20:46 css/style_oscarlevin.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-05 20:46 css/setcolors.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-05 20:46 css/README.md
--rw-r--r--  2.0 unx     4021 b- defN 23-May-05 20:46 css/update_css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-05 20:46 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-05 20:46 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-05 20:46 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-05 20:46 css/style_default.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-05 20:46 css/epub.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-05 20:46 css/colors_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-05 20:46 css/style_soundwriting.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-05 20:46 css/mathbook-3.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-05 20:46 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-05 20:46 css/kindle.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-05 20:46 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1276 b- defN 23-May-05 20:46 css/colors_maroon_grey.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/braille/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-05 20:46 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-05 20:46 script/mbx
--rw-r--r--  2.0 unx     2573 b- defN 23-May-05 20:46 script/braille/pretext-symbol.dis
--rw-r--r--  2.0 unx     8913 b- defN 23-May-05 20:46 script/braille/pretext.sem
--rw-r--r--  2.0 unx      735 b- defN 23-May-05 20:46 script/braille/README.md
--rw-r--r--  2.0 unx     6616 b- defN 23-May-05 20:46 script/braille/pretext-liblouis.cfg
--rw-r--r--  2.0 unx     1011 b- defN 23-May-05 20:46 script/braille/pretext-liblouis-emboss.cfg
--rw-r--r--  2.0 unx      490 b- defN 23-May-05 20:46 script/braille/pretext-liblouis-electronic.cfg
--rw-r--r--  2.0 unx      481 b- defN 23-May-05 20:46 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 20:46 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-May-05 20:46 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-May-05 20:46 script/mjsre/package.json
--rw-r--r--  2.0 unx     2566 b- defN 23-May-05 20:46 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-May-05 20:46 pretext/README.md
--rw-r--r--  2.0 unx   173946 b- defN 23-May-05 20:46 pretext/pretext.py
--rw-r--r--  2.0 unx    35057 b- defN 23-May-05 20:46 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 20:46 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-05 20:46 pretext/module-test.py
--rw-r--r--  2.0 unx    31361 b- defN 23-May-05 20:46 pretext/pretext
-148 files, 4884135 bytes uncompressed, 1034849 bytes compressed:  78.8%
+Zip file size: 1052517 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/utilities/
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-06 06:17 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx   261852 b- defN 23-May-06 06:17 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-06 06:17 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-06 06:17 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-06 06:17 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-06 06:17 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-06 06:17 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-06 06:17 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-06 06:17 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-06 06:17 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-06 06:17 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    69315 b- defN 23-May-06 06:17 xsl/pretext-braille.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-06 06:17 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   544147 b- defN 23-May-06 06:17 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    65459 b- defN 23-May-06 06:17 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-06 06:17 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-06 06:17 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-06 06:17 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-06 06:17 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-06 06:17 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-06 06:17 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139661 b- defN 23-May-06 06:17 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-06 06:17 xsl/README.md
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-06 06:17 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   604338 b- defN 23-May-06 06:17 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-06 06:17 xsl/entities.ent
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-06 06:17 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-06 06:17 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-06 06:17 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-06 06:17 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   541182 b- defN 23-May-06 06:17 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-06 06:17 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-06 06:17 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    39922 b- defN 23-May-06 06:17 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-06 06:17 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-06 06:17 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-06 06:17 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-06 06:17 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-06 06:17 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-06 06:17 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-06 06:17 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-May-06 06:17 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-06 06:17 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-06 06:17 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-06 06:17 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-06 06:17 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-06 06:17 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-06 06:17 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-06 06:17 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-06 06:17 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-06 06:17 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-06 06:17 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-06 06:17 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-06 06:17 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-06 06:17 xsl/localizations/README.md
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-06 06:17 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-06 06:17 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-06 06:17 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-06 06:17 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-06 06:17 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-06 06:17 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-06 06:17 xsl/localizations/pt-PT.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-06 06:17 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-06 06:17 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-06 06:17 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-06 06:17 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-May-06 06:17 xsl/support/README.md
+-rw-r--r--  2.0 unx      486 b- defN 23-May-06 06:17 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-06 06:17 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-May-06 06:17 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-06 06:17 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-06 06:17 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx   133917 b- defN 23-May-06 06:17 schema/pretext.xml
+-rw-r--r--  2.0 unx   124561 b- defN 23-May-06 06:17 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-06 06:17 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx      326 b- defN 23-May-06 06:17 schema/xml.xsd
+-rw-r--r--  2.0 unx    57960 b- defN 23-May-06 06:17 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-06 06:17 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-06 06:17 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-06 06:17 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-06 06:17 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-06 06:17 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   101402 b- defN 23-May-06 06:17 schema/pretext.rng
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-06 06:17 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-06 06:17 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-06 06:17 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-06 06:17 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-06 06:17 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-06 06:17 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-06 06:17 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-06 06:17 css/setcolors.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-06 06:17 css/README.md
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-06 06:17 css/update_css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-06 06:17 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-06 06:17 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-06 06:17 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-06 06:17 css/style_default.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-06 06:17 css/epub.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-06 06:17 css/colors_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-06 06:17 css/style_soundwriting.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-06 06:17 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-06 06:17 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-06 06:17 css/kindle.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-06 06:17 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-06 06:17 css/colors_maroon_grey.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/braille/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-06 06:17 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-06 06:17 script/mbx
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-06 06:17 script/braille/pretext-symbol.dis
+-rw-r--r--  2.0 unx     8913 b- defN 23-May-06 06:17 script/braille/pretext.sem
+-rw-r--r--  2.0 unx      735 b- defN 23-May-06 06:17 script/braille/README.md
+-rw-r--r--  2.0 unx     6616 b- defN 23-May-06 06:17 script/braille/pretext-liblouis.cfg
+-rw-r--r--  2.0 unx     1011 b- defN 23-May-06 06:17 script/braille/pretext-liblouis-emboss.cfg
+-rw-r--r--  2.0 unx      490 b- defN 23-May-06 06:17 script/braille/pretext-liblouis-electronic.cfg
+-rw-r--r--  2.0 unx      481 b- defN 23-May-06 06:17 script/mjsre/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 06:17 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-06 06:17 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-May-06 06:17 script/mjsre/package.json
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-06 06:17 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-06 06:17 pretext/README.md
+-rw-r--r--  2.0 unx   173946 b- defN 23-May-06 06:17 pretext/pretext.py
+-rw-r--r--  2.0 unx    35057 b- defN 23-May-06 06:17 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-06 06:17 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-06 06:17 pretext/module-test.py
+-rw-r--r--  2.0 unx    31361 b- defN 23-May-06 06:17 pretext/pretext
+148 files, 4879036 bytes uncompressed, 1034093 bytes compressed:  78.8%
```

#### xsl/publisher-variables.xsl

##### xsl/publisher-variables.xsl

```diff
@@ -3062,48 +3062,14 @@
       </xsl:when>
       <!-- no effort to set this switch, so use default -->
       <xsl:otherwise>
         <xsl:value-of select="$upbutton-default"/>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:variable>
-  <!-- There are also "compact" versions of the navigation buttons in the top right -->
-  <xsl:variable name="nav-style">
-    <xsl:variable name="style-default" select="'full'"/>
-    <xsl:choose>
-      <xsl:when test="$publication/html/navigation/@style = 'full'">
-        <xsl:text>full</xsl:text>
-      </xsl:when>
-      <xsl:when test="$publication/html/navigation/@style = 'compact'">
-        <xsl:text>compact</xsl:text>
-      </xsl:when>
-      <!-- an attempt to set, but wrong -->
-      <xsl:when test="$publication/html/navigation/@style">
-        <xsl:message>
-          PTX:WARNING: HTML navigation style setting in publisher file should be &quot;full&quot; or &quot;compact&quot;, not &quot;
-          <xsl:value-of select="$publication/html/navigation/@style"/>
-          &quot;. Proceeding with default value: &quot;
-          <xsl:value-of select="$style-default"/>
-          &quot;
-        </xsl:message>
-        <xsl:value-of select="$style-default"/>
-      </xsl:when>
-      <!-- backwards compatibility, no error-checking -->
-      <xsl:when test="$html.navigation.style='full'">
-        <xsl:text>full</xsl:text>
-      </xsl:when>
-      <xsl:when test="$html.navigation.style='compact'">
-        <xsl:text>compact</xsl:text>
-      </xsl:when>
-      <!-- no effort to set this switch, so use default -->
-      <xsl:otherwise>
-        <xsl:value-of select="$style-default"/>
-      </xsl:otherwise>
-    </xsl:choose>
-  </xsl:variable>
   <!--                              -->
   <!-- HTML CSS Style Specification -->
   <!--                              -->
   <!-- Remain for testing purposes -->
   <xsl:param name="html.css.colorfile" select="''"/>
   <xsl:param name="html.css.stylefile" select="''"/>
   <!-- A temporary variable for testing -->
@@ -5063,9 +5029,16 @@
     <!-- 2023-01-11  EPUB cover image publication file entry totally reworked -->
     <xsl:call-template name="parameter-deprecation-message">
       <xsl:with-param name="date-string" select="'2023-01-11'"/>
       <xsl:with-param name="message" select="'the  epub/@cover  publication file entry has been replaced, and likely you will only get a simple generic cover image.  Please read the documentation for how to transition to the new specification'"/>
       <xsl:with-param name="incorrect-use" select="($publication/epub/@cover != '')"/>
     </xsl:call-template>
     <!--  -->
+    <!-- 2023-05-05  HTML navigation buttons' style publication file entry removed -->
+    <xsl:call-template name="parameter-deprecation-message">
+      <xsl:with-param name="date-string" select="'2023-05-05'"/>
+      <xsl:with-param name="message" select="'the  html/navigation/@style  publication file entry has been removed, since the &quot;compact&quot; option is no longer implemented, and the only option left is &quot;full&quot;.  Remove your publication file entry to stop this message re-appearing'"/>
+      <xsl:with-param name="incorrect-use" select="($publication/html/navigation/@style != '')"/>
+    </xsl:call-template>
+    <!--  -->
   </xsl:template>
 </xsl:stylesheet>
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -10078,24 +10078,20 @@
                 <!-- Alternative to "copy-of": convert $content to a  -->
                 <!-- node-set, and then hit with an identity template -->
                 <!-- to duplicate.  Experiment indicates no change in -->
                 <!-- output. (2023-01-11)                             -->
                 <xsl:copy-of select="$content"/>
               </div>
               <div class="ptx-content-footer">
-                <xsl:apply-templates select="." mode="previous-button">
-                  <xsl:with-param name="id-label" select="'previousbutton'"/>
-                </xsl:apply-templates>
+                <xsl:apply-templates select="." mode="previous-button"/>
                 <a class="top-button button" href="#" title="Top">
                   <span class="icon">^</span>
                   <span class="name">Top</span>
                 </a>
-                <xsl:apply-templates select="." mode="next-button">
-                  <xsl:with-param name="id-label" select="'nextbutton'"/>
-                </xsl:apply-templates>
+                <xsl:apply-templates select="." mode="next-button"/>
               </div>
             </main>
           </div>
           <!-- formerly "extra" -->
           <div id="ptx-page-footer">
             <xsl:apply-templates select="." mode="feedback-button"/>
             <xsl:call-template name="pretext-link"/>
@@ -10487,15 +10483,14 @@
   </xsl:template>
   <!--                     -->
   <!-- Navigation Sections -->
   <!--                     -->
   <!-- Button code, <a href=""> when active   -->
   <!-- <span> with "disabled" class otherwise -->
   <xsl:template match="*" mode="previous-button">
-    <xsl:param name="id-label" select="''"/>
     <xsl:variable name="previous-url">
       <xsl:choose>
         <xsl:when test="$nav-logic='linear'">
           <xsl:apply-templates select="." mode="previous-linear-url"/>
         </xsl:when>
         <xsl:when test="$nav-logic='tree'">
           <xsl:apply-templates select="." mode="previous-tree-url"/>
@@ -10596,15 +10591,14 @@
         <a href="#indexletter-x">X</a>
         <a href="#indexletter-y">Y</a>
         <a href="#indexletter-z">Z</a>
       </span>
     </div>
   </xsl:template>
   <xsl:template match="*" mode="next-button">
-    <xsl:param name="id-label" select="''"/>
     <xsl:variable name="next-url">
       <xsl:choose>
         <xsl:when test="$nav-logic='linear'">
           <xsl:apply-templates select="." mode="next-linear-url"/>
         </xsl:when>
         <xsl:when test="$nav-logic='tree'">
           <xsl:apply-templates select="." mode="next-tree-url"/>
@@ -10641,15 +10635,14 @@
           </span>
           <span class="icon">&gt;</span>
         </xsl:element>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
   <xsl:template match="*" mode="up-button">
-    <xsl:param name="id-label" select="''"/>
     <!-- up URL is identical for linear, tree logic -->
     <xsl:variable name="up-url">
       <xsl:apply-templates select="." mode="up-url"/>
     </xsl:variable>
     <xsl:choose>
       <xsl:when test="$up-url!=''">
         <xsl:element name="a">
@@ -10892,135 +10885,59 @@
               </li>
             </ol>
           </li>
         </ol>
       </div>
     </button>
   </xsl:template>
-  <!--    Compact Buttons no longer supported, so this can be deleted, says David F -->
-  <!-- Compact Buttons -->
-  <!-- These get smashed consecutively into a single "tool-bar" -->
-  <xsl:template match="*" mode="compact-buttons">
-    <!-- URL formation, maybe this could be consolidated with above versions -->
-    <xsl:variable name="previous-url">
-      <xsl:choose>
-        <xsl:when test="$nav-logic='linear'">
-          <xsl:apply-templates select="." mode="previous-linear-url"/>
-        </xsl:when>
-        <xsl:when test="$nav-logic='tree'">
-          <xsl:apply-templates select="." mode="previous-tree-url"/>
-        </xsl:when>
-      </xsl:choose>
-    </xsl:variable>
-    <xsl:variable name="up-url">
-      <xsl:apply-templates select="." mode="up-url"/>
-    </xsl:variable>
-    <xsl:variable name="next-url">
-      <xsl:choose>
-        <xsl:when test="$nav-logic='linear'">
-          <xsl:apply-templates select="." mode="next-linear-url"/>
-        </xsl:when>
-        <xsl:when test="$nav-logic='tree'">
-          <xsl:apply-templates select="." mode="next-tree-url"/>
-        </xsl:when>
-      </xsl:choose>
-    </xsl:variable>
-    <!-- toolbar-item when aligned right, get placed right: first in, first right -->
-    <!-- so they apparently seem in the reversed order here and in HTML output    -->
-    <!-- Empty URL, then no button                                                -->
-    <xsl:if test="not($next-url = '')">
-      <div class="toolbar-item">
-        <a href="{$next-url}">
-          <svg xmlns="https://www.w3.org/2000/svg" height="50" width="60" viewBox="0 50 110 100">
-            <polygon points="110,100 75,75 0,75 0,125 75,125 " style="fill:darkred;stroke:maroon;stroke-width:1"/>
-            <text x="13" y="108" fill="blanchedalmond" font-size="32">next</text>
-          </svg>
-        </a>
-      </div>
-    </xsl:if>
-    <xsl:if test="not($up-url = '')">
-      <div class="toolbar-item">
-        <a href="{$up-url}">
-          <svg xmlns="https://www.w3.org/2000/svg" height="50" width="60" viewBox="0 50 80 100">
-            <polygon points="75,75 37,65 0,75 0,125 75,125 " style="fill:blanchedalmond;stroke:burlywood;stroke-width:1"/>
-            <text x="13" y="108" fill="maroon" font-size="32">up</text>
-          </svg>
-        </a>
-      </div>
-    </xsl:if>
-    <xsl:if test="not($previous-url = '')">
-      <div class="toolbar-item">
-        <a href="{$previous-url}">
-          <svg xmlns="https://www.w3.org/2000/svg" height="50" width="60" viewBox="-10 50 110 100">
-            <polygon points="-10,100 25,75 100,75 100,125 25,125 " style="fill:blanchedalmond;stroke:burlywood;stroke-width:1"/>
-            <text x="28" y="108" fill="maroon" font-size="32">prev</text>
-          </svg>
-        </a>
-      </div>
-    </xsl:if>
-  </xsl:template>
   <!-- Primary Navigation Panels -->
   <!-- ToC, Prev/Up/Next/Annotation buttons  -->
   <!-- Also organized for small screen modes -->
   <xsl:template match="*" mode="primary-navigation">
     <nav id="ptx-navbar" class="navbar">
       <button class="toc-toggle button" aria-label="Show or hide table of contents">
         <span class="icon">☰</span>
         <span class="name">
           <xsl:apply-templates select="." mode="type-name">
             <xsl:with-param name="string-id" select="'toc'"/>
           </xsl:apply-templates>
         </span>
       </button>
-      <!-- Prev/Up/Next buttons on top, according to options -->
+      <!-- A page either has an/the index as    -->
+      <!-- a child, and gets the "jump to" bar, -->
+      <!-- or it deserves an index button       -->
       <xsl:choose>
-        <xsl:when test="$nav-style = 'full'">
-          <!-- A page either has an/the index as    -->
-          <!-- a child, and gets the "jump to" bar, -->
-          <!-- or it deserves an index button       -->
-          <xsl:choose>
-            <xsl:when test="index-list">
-              <xsl:apply-templates select="." mode="index-jump-nav"/>
-            </xsl:when>
-            <xsl:otherwise>
-              <xsl:apply-templates select="." mode="index-button"/>
-            </xsl:otherwise>
-          </xsl:choose>
-          <!-- Button to show/hide the calculator -->
-          <xsl:if test="$b-has-calculator">
-            <xsl:call-template name="calculator-toggle"/>
-            <xsl:call-template name="calculator"/>
-          </xsl:if>
-          <!-- Runestone user menu -->
-          <!-- Conditional on a build for Runestone hosting -->
-          <xsl:call-template name="runestone-bust-menu"/>
-          <!-- A scratch ActiveCode via a pencil icon, always -->
-          <xsl:call-template name="runestone-scratch-activecode"/>
-          <!-- The user-preferences-menu needs to be unified with the runestone-bust-menu -->
-          <xsl:call-template name="user-preferences-menu"/>
-          <!-- Span to encase Prev/Up/Next buttons and float right    -->
-          <!-- Each button gets an id for keypress recognition/action -->
-          <span class="treebuttons">
-            <xsl:apply-templates select="." mode="previous-button">
-              <xsl:with-param name="id-label" select="'previousbutton'"/>
-            </xsl:apply-templates>
-            <xsl:if test="$nav-upbutton='yes'">
-              <xsl:apply-templates select="." mode="up-button">
-                <xsl:with-param name="id-label" select="'upbutton'"/>
-              </xsl:apply-templates>
-            </xsl:if>
-            <xsl:apply-templates select="." mode="next-button">
-              <xsl:with-param name="id-label" select="'nextbutton'"/>
-            </xsl:apply-templates>
-          </span>
-        </xsl:when>
-        <xsl:when test="$nav-style = 'compact'">
-          <xsl:apply-templates select="." mode="compact-buttons"/>
+        <xsl:when test="index-list">
+          <xsl:apply-templates select="." mode="index-jump-nav"/>
         </xsl:when>
+        <xsl:otherwise>
+          <xsl:apply-templates select="." mode="index-button"/>
+        </xsl:otherwise>
       </xsl:choose>
+      <!-- Button to show/hide the calculator -->
+      <xsl:if test="$b-has-calculator">
+        <xsl:call-template name="calculator-toggle"/>
+        <xsl:call-template name="calculator"/>
+      </xsl:if>
+      <!-- Runestone user menu -->
+      <!-- Conditional on a build for Runestone hosting -->
+      <xsl:call-template name="runestone-bust-menu"/>
+      <!-- A scratch ActiveCode via a pencil icon, always -->
+      <xsl:call-template name="runestone-scratch-activecode"/>
+      <!-- The user-preferences-menu needs to be unified with the runestone-bust-menu -->
+      <xsl:call-template name="user-preferences-menu"/>
+      <!-- Span to encase Prev/Up/Next buttons and float right    -->
+      <!-- Each button gets an id for keypress recognition/action -->
+      <span class="treebuttons">
+        <xsl:apply-templates select="." mode="previous-button"/>
+        <xsl:if test="$nav-upbutton='yes'">
+          <xsl:apply-templates select="." mode="up-button"/>
+        </xsl:if>
+        <xsl:apply-templates select="." mode="next-button"/>
+      </span>
       <!-- Annotations button was once here, see GitHub issue -->
       <!-- https://github.com/rbeezer/mathbook/issues/1010    -->
       <!-- Search box at end of ptx-navbar, so it can be sticky -->
       <xsl:call-template name="google-search-box"/>
       <xsl:call-template name="native-search-box"/>
     </nav>
   </xsl:template>
```

### Comparing `pretext-1.5.3.dev20230505/pretext/generate.py` & `pretext-1.5.3.dev20230506/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/project.py` & `pretext-1.5.3.dev20230506/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230506/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230506/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230506/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-05 20:45 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-05 20:45 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-May-05 20:45 assets/frog.jpg
--rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      449 b- defN 23-May-05 20:45 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-05 20:45 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-05 20:45 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-06 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-06 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-06 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      449 b- defN 23-May-06 06:16 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-06 06:16 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-06 06:16 source/main.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230506/pretext/templates/resources/book.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-05 20:45 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
--rw-r--r--  2.0 unx     6114 b- defN 23-May-05 20:45 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-May-05 20:45 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-06 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-06 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-06 06:16 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230506/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-05 20:45 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
--rw-r--r--  2.0 unx     6092 b- defN 23-May-05 20:45 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-05 20:45 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-05 20:45 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-May-05 20:45 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-05 20:45 source/ch-generate.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-05 20:45 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-05 20:45 source/sec-features.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-May-05 20:45 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-05 20:45 source/ch-empty.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-05 20:45 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-05 20:45 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-05 20:45 source/docinfo.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-05 20:45 source/ex-first.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-05 20:45 source/backmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-05 20:45 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-05 20:45 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-05 20:45 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-05 20:45 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-05 20:45 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-May-05 20:45 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-05 20:45 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-05 20:45 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 23-May-05 20:45 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-06 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-06 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-06 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-06 06:16 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-May-06 06:16 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-06 06:16 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-06 06:16 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-06 06:16 source/sec-features.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-May-06 06:16 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-06 06:16 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-06 06:16 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-06 06:16 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-06 06:16 source/docinfo.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-06 06:16 source/ex-first.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-06 06:16 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-06 06:16 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-06 06:16 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-06 06:16 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-06 06:16 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-06 06:16 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-May-06 06:16 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-06 06:16 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-06 06:16 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 23-May-06 06:16 source/images/sageplot2d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230506/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230506/pretext/templates/resources/hello.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-May-05 20:45 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-05 20:45 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-05 20:45 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-May-05 20:45 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-May-06 06:16 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-06 06:16 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-06 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-May-06 06:16 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230506/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230506/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230506/pretext/templates/resources/slideshow.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 xsl/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-May-05 20:45 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-May-05 20:45 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-05 20:45 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx    11200 b- defN 23-May-05 20:45 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 xsl/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-May-06 06:16 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-May-06 06:16 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-06 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-06 06:16 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

### Comparing `pretext-1.5.3.dev20230505/pretext/utils.py` & `pretext-1.5.3.dev20230506/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230505/pyproject.toml` & `pretext-1.5.3.dev20230506/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230505"
+version = "1.5.3.dev20230506"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230505/PKG-INFO` & `pretext-1.5.3.dev20230506/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230505
+Version: 1.5.3.dev20230506
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

