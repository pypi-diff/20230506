# Comparing `tmp/stmaterial-0.0.3.tar.gz` & `tmp/stmaterial-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmaterial-0.0.3.tar", last modified: Thu May  4 07:07:10 2023, max compression
+gzip compressed data, was "stmaterial-0.0.4.tar", last modified: Sat May  6 04:25:01 2023, max compression
```

## Comparing `stmaterial-0.0.3.tar` & `stmaterial-0.0.4.tar`

### file list

```diff
@@ -1,202 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:07:10.290239 stmaterial-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 07:06:18.878026 stmaterial-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 07:06:18.878026 stmaterial-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 07:06:18.878026 stmaterial-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-04 07:06:18.878026 stmaterial-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/a.png
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/b.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/books/
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/books/benders分解.png
--rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/books/内点法.png
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/c.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.878026 stmaterial-0.0.3/docs/_images/links/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_images/links/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_images/links/gallery/jupyter_book.png
--rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_images/links/gallery/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_images/links/gallery/pandas.png
--rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_images/links/gallery/sphinx_design.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_static/links/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-04 07:06:18.882026 stmaterial-0.0.3/docs/_static/links/gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/blog.md
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/plangs/
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/plangs/2021-python-pathlib.md
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/plangs/2022-pytest-tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/plangs/2022-python-setup.md
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/posts/plangs/2022-python-typing.md
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/edit-button.md
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/fonts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/header.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/logo.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/sidebar-title.md
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/sidebar.md
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/user_guide/toc.md
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-04 07:06:18.886026 stmaterial-0.0.3/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-04 07:06:18.886026 stmaterial-0.0.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-04 07:06:18.886026 stmaterial-0.0.3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-04 07:06:18.886026 stmaterial-0.0.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 07:06:18.886026 stmaterial-0.0.3/postcss.config.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-04 07:06:18.886026 stmaterial-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.886026 stmaterial-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-05-04 07:06:18.886026 stmaterial-0.0.3/src/stmaterial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-05-04 07:06:18.886026 stmaterial-0.0.3/src/stmaterial/_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-04 07:06:18.886026 stmaterial-0.0.3/src/stmaterial/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/scripts/gumshoe-patched.js
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/scripts/materialize.js
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/scripts/stmaterial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/base/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_breadcrumb.sass
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_edit-update-meta.scss
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/components/_table-of-contents.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_lists.sass
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_myst-nb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_tippy.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/patch/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/patch/_legacy.sass
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/patch/_patch.scss
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/patch/_test.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_article.sass
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_headnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/stmaterial.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/stmaterial theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3333 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/extra_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/headnav-items.html
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/postnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sidebar/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sidebar/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/theme/stmaterial/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-04 07:06:18.890026 stmaterial-0.0.3/src/stmaterial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:06:18.890026 stmaterial-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-04 07:06:18.890026 stmaterial-0.0.3/webpack.config.js
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 stmaterial-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:25:01.071255 stmaterial-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-06 04:24:42.834728 stmaterial-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-06 04:24:42.834728 stmaterial-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-06 04:24:42.834728 stmaterial-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-06 04:24:42.834728 stmaterial-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/benders分解.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/内点法.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/c.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/links/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/jupyter_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/pandas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/sphinx_design.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/links/gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/blog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2021-python-pathlib.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-pytest-tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-python-setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-python-typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/edit-button.md
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/fonts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/logo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/sidebar-title.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/sidebar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/toc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-06 04:24:42.846728 stmaterial-0.0.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-06 04:24:42.846728 stmaterial-0.0.4/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-06 04:24:42.846728 stmaterial-0.0.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 04:24:42.846728 stmaterial-0.0.4/postcss.config.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-06 04:24:42.846728 stmaterial-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/gumshoe-patched.js
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/materialize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/stmaterial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_breadcrumb.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_edit-update-meta.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_table-of-contents.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_lists.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_myst-nb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_tippy.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_legacy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_patch.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_test.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_article.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_headnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/stmaterial.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/stmaterial theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3333 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/headnav-items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/postnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sidenav-brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-06 04:24:42.850728 stmaterial-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 stmaterial-0.0.4/PKG-INFO
```

### Comparing `stmaterial-0.0.3/LICENSE` & `stmaterial-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/Makefile` & `stmaterial-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/README.md` & `stmaterial-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/a.png` & `stmaterial-0.0.4/docs/_images/a.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/b.png` & `stmaterial-0.0.4/docs/_images/b.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/books/benders分解.png` & `stmaterial-0.0.4/docs/_images/books/benders分解.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/books/内点法.png` & `stmaterial-0.0.4/docs/_images/books/内点法.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/c.png` & `stmaterial-0.0.4/docs/_images/c.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/links/gallery/jupyter_book.png` & `stmaterial-0.0.4/docs/_images/links/gallery/jupyter_book.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/links/gallery/matplotlib.png` & `stmaterial-0.0.4/docs/_images/links/gallery/matplotlib.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/links/gallery/pandas.png` & `stmaterial-0.0.4/docs/_images/links/gallery/pandas.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_images/links/gallery/sphinx_design.png` & `stmaterial-0.0.4/docs/_images/links/gallery/sphinx_design.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_static/favicon.png` & `stmaterial-0.0.4/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_static/links/gallery.yaml` & `stmaterial-0.0.4/docs/_static/links/gallery.yaml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/_static/logo.png` & `stmaterial-0.0.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/conf.py` & `stmaterial-0.0.4/docs/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,17 +14,21 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "stmaterial.demo.sphinxext",
+    "ablog",
     "myst_parser",
     "sphinx_inline_tabs",
-    "ablog",
+    "sphinx_design",
+    "sphinx_copybutton",
+    "sphinx_togglebutton",
+    "sphinx_subfigure",
     "sphinx_tippy"
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
 exclude_patterns = [
     "_build", 
@@ -65,15 +69,16 @@
     "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {"name": "Sphinx book theme", "url": "https://sphinx-book-theme.readthedocs.io/en/latest/"},
         {"name": "Pydata sphinx theme", "url": "https://pydata-sphinx-theme.readthedocs.io/"},
     ],
     "show_toc_level": 1,
     "header_icons": [
-        {"name":"Github", "url": "http://github.com/zclab/stmaterial", "svg":"github.svg"},
+        # {"name":"Github", "url": "http://github.com/zclab/stmaterial", "svg":"github.svg"},
+        {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
         {"name":"Email", "url": "example@example.com", "material_icons":"email"},
     ],
     "use_edit_page_button": True,
     "toc_title": "On this page",
     "custom_fonts": {
         "name": 'LXGWWenKaiLite',
         "type": 'truetype',
@@ -86,32 +91,36 @@
         ],
     },
     "light_css_variables": {
         "primary-color": "#5c6bc0",
         "primary-color-dark": "#283593",
         "primary-color-raised-hover-solid": "#7986cb",
         "primary-color-raised-focus-solid":"#7986cb",
-    }
+    },
+    "navigation_with_keys": True,
 }
     
 
 blog_path = "blog"
 blog_post_pattern = "posts/*/*"
 blog_authors = {
     "zclab": ("子川", "https://github.com/zclab"),
 }
 
-# https://github.com/hung1001/font-awesome-pro-v6
-fontawesome_link_cdn = "https://cdn.staticaly.com/gh/hung1001/font-awesome-pro-v6/44659d9/css/all.min.css"
-fontawesome_included = True
-
 html_sidebars = {
+    "index":[],
     "posts/**": [
-        "sidebar/search.html", "ablog/postcard.html","ablog/categories.html","ablog/tagcloud.html", "ablog/recentposts.html",
+        "search-field.html", "ablog/postcard.html","ablog/categories.html","ablog/tagcloud.html", "ablog/recentposts.html",
     ],
     "blog": [
-        "sidebar/search.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
+        "search-field.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
     ],
     "blog/**": [
-        "sidebar/search.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
+        "search-field.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
     ],
 }
+
+# https://github.com/hung1001/font-awesome-pro-v6
+html_css_files = [
+      "https://cdn.staticaly.com/gh/hung1001/font-awesome-pro-v6/44659d9/css/all.min.css",
+]
+fontawesome_included = True
```

### Comparing `stmaterial-0.0.3/docs/develop.md` & `stmaterial-0.0.4/docs/develop.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/admonitions.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/api.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/blocks.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/generic.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/images.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/index.md` & `stmaterial-0.0.4/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/lists.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/really-long.md` & `stmaterial-0.0.4/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/sphinx-design.md` & `stmaterial-0.0.4/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/structure.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/tables.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/kitchen-sink/typography.rst` & `stmaterial-0.0.4/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/admonitions.md` & `stmaterial-0.0.4/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/api.md` & `stmaterial-0.0.4/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/code-blocks.md` & `stmaterial-0.0.4/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/hyperlinks.md` & `stmaterial-0.0.4/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/images.md` & `stmaterial-0.0.4/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/index.md` & `stmaterial-0.0.4/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/lists.md` & `stmaterial-0.0.4/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/tables.md` & `stmaterial-0.0.4/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/tabs.md` & `stmaterial-0.0.4/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/examples/reference/text-formatting.md` & `stmaterial-0.0.4/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/posts/plangs/2021-python-pathlib.md` & `stmaterial-0.0.4/docs/posts/plangs/2021-python-pathlib.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/posts/plangs/2022-pytest-tutorial.md` & `stmaterial-0.0.4/docs/posts/plangs/2022-pytest-tutorial.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/posts/plangs/2022-python-setup.md` & `stmaterial-0.0.4/docs/posts/plangs/2022-python-setup.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/posts/plangs/2022-python-typing.md` & `stmaterial-0.0.4/docs/posts/plangs/2022-python-typing.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/edit-button.md` & `stmaterial-0.0.4/docs/user_guide/edit-button.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/fonts.md` & `stmaterial-0.0.4/docs/user_guide/fonts.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/header.md` & `stmaterial-0.0.4/docs/user_guide/header.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/index.md` & `stmaterial-0.0.4/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/landing-page.md` & `stmaterial-0.0.4/docs/user_guide/landing-page.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/logo.md` & `stmaterial-0.0.4/docs/user_guide/logo.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/sidebar.md` & `stmaterial-0.0.4/docs/user_guide/sidebar.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/user_guide/toc.md` & `stmaterial-0.0.4/docs/user_guide/toc.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/docs/web-components.rst` & `stmaterial-0.0.4/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/noxfile.py` & `stmaterial-0.0.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/package-lock.json` & `stmaterial-0.0.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/package.json` & `stmaterial-0.0.4/package.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/pyproject.toml` & `stmaterial-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/__init__.py` & `stmaterial-0.0.4/src/stmaterial/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from ._navigation import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
-from .utils import get_theme_options, activate_extensions, config_provided_by_user
+from .utils import get_theme_options, config_provided_by_user
 from .directives import GalleryDirective
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 logger = logging.getLogger(__name__)
 
 MESSAGE_CATALOG_NAME = "stmaterial"
 _KNOWN_STYLES_IN_USE: Dict[str, Optional[Style]] = {
     "light": None,
     "dark": None,
 }
@@ -387,18 +387,20 @@
 
     app.connect("html-page-context", _html_page_context)
     app.connect("html-page-context", update_and_remove_templates)
     app.connect("html-page-context", add_toctree_functions)
     app.connect("builder-inited", _builder_inited)
     app.connect("builder-inited", _update_config)
     app.connect("build-finished", _overwrite_pygments_css)
+    # Include component templates
+    app.config.templates_path.append(str(theme_dir / "components"))
     app.config.html_static_path.append(str(theme_dir / "static/images"))
 
-    extensions = ["sphinx_design", "sphinx_copybutton", "sphinx_togglebutton", "sphinx_subfigure"]
-    activate_extensions(app, extensions)
+    # extensions = ["sphinx_design", "sphinx_copybutton", "sphinx_togglebutton", "sphinx_subfigure"]
+    # activate_extensions(app, extensions)
 
     app.add_directive("gallery-grid", GalleryDirective)
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
         "version": __version__,
```

### Comparing `stmaterial-0.0.3/src/stmaterial/_navigation.py` & `stmaterial-0.0.4/src/stmaterial/_navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,24 +255,24 @@
 
         # Wrap the final few header items in a "more" dropdown
         links_dropdown = links_html[n_links_before_dropdown:]
         if links_dropdown:
             links_dropdown_html = "\n".join(links_dropdown)
             out_headnav += f"""
             <li class="nav-item dropdown">
-                <a class='dropdown-trigger' href='#' data-target='dropdown1'>More <i class="material-icons">arrow_drop_down</i></a>
+                <a class='dropdown-trigger' href='#' data-target='dropdown1'>{context["theme_dropdown_label_name"]} <i class="material-icons">arrow_drop_down</i></a>
                 <ul id='dropdown1' class='dropdown-content'>
                     {links_dropdown_html}
                 </ul>
             </li>
             """  # noqa
 
             out_sidenav += f"""
             <li class="nav-item dropdown">
-                <a class='dropdown-trigger' href='#' data-target='dropdown2'>More <i class="material-icons">arrow_drop_down</i></a>
+                <a class='dropdown-trigger' href='#' data-target='dropdown2'>{context["theme_dropdown_label_name"]} <i class="material-icons">arrow_drop_down</i></a>
                 <ul id='dropdown2' class='dropdown-content'>
                     {links_dropdown_html}
                 </ul>
             </li>
             """  # noqa
 
         return out_headnav, out_sidenav
```

### Comparing `stmaterial-0.0.3/src/stmaterial/_transforms.py` & `stmaterial-0.0.4/src/stmaterial/_transforms.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/_translations.py` & `stmaterial-0.0.4/src/stmaterial/_translations.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/scripts/gumshoe-patched.js` & `stmaterial-0.0.4/src/stmaterial/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/scripts/stmaterial.js` & `stmaterial-0.0.4/src/stmaterial/assets/scripts/stmaterial.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -143,39 +143,63 @@
     // if (is_touch_device()) {
     //   document.querySelector('#nav-mobile').style.overflow = 'auto';
     // }
 
     // Theme
     const theme = localStorage.getItem('theme');
     const themeSwitch = document.querySelector('#theme-switch');
+    const themeSwitch__mobile = document.querySelector('#theme-switch--mobile');
     const setTheme = (isDark) => {
         if (isDark) {
             themeSwitch.classList.add('is-dark');
             themeSwitch.querySelector('i').innerText = 'light_mode';
             themeSwitch.title = 'Switch to light mode';
+
+            themeSwitch__mobile.classList.add('is-dark');
+            themeSwitch__mobile.querySelector('i').innerText = 'light_mode';
+            themeSwitch__mobile.title = 'Switch to light mode';
         } else {
             themeSwitch.classList.remove('is-dark');
             themeSwitch.querySelector('i').innerText = 'dark_mode';
             themeSwitch.title = 'Switch to dark mode';
+
+            themeSwitch__mobile.classList.remove('is-dark');
+            themeSwitch__mobile.querySelector('i').innerText = 'dark_mode';
+            themeSwitch__mobile.title = 'Switch to dark mode';
         }
     }
-    if (themeSwitch) {
+    if (themeSwitch || themeSwitch__mobile) {
         // Load
         if (theme) setTheme(true);
         // Change
         themeSwitch.addEventListener('click', e => {
             e.preventDefault();
             if (!themeSwitch.classList.contains('is-dark')) {
                 // Dark Theme
                 document.documentElement.setAttribute('theme', 'dark');
                 localStorage.setItem('theme', 'dark');
                 setTheme(true);
             } else {
                 // Light Theme
                 document.documentElement.removeAttribute('theme');
+                localStorage.removeItem('theme');
+                setTheme(false);
+            }
+        });
+
+        themeSwitch__mobile.addEventListener('click', e => {
+            e.preventDefault();
+            if (!themeSwitch__mobile.classList.contains('is-dark')) {
+                // Dark Theme
+                document.documentElement.setAttribute('theme', 'dark');
+                localStorage.setItem('theme', 'dark');
+                setTheme(true);
+            } else {
+                // Light Theme
+                document.documentElement.removeAttribute('theme');
                 localStorage.removeItem('theme');
                 setTheme(false);
             }
         });
     }
```

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/base/_typography.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/components/_back-to-top.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/components/_prev-next.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/components/_table-of-contents.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_table-of-contents.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_admonitions.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_api.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_code.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_footnotes.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_images.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_lists.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_misc.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_sidebar.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_tables.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/content/_target.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_target.sass`

 * *Files 14% similar despite different names*

```diff
@@ -67,7 +67,13 @@
 dt:target
   background-color: var(--color-highlight-on-target) !important
 
 // When a footnote reference is selected
 .footnote > dt:target + dd,
 .footnote-reference:target
   background-color: var(--color-highlight-on-target)
+
+aside.footnote:target
+  background-color: var(--color-highlight-on-target)
+
+div.citation:target
+  background-color: var(--color-highlight-on-target)
```

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_ablog.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/extensions/_timeline.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_timeline.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/patch/_legacy.sass` & `stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_legacy.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_footer.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_footer.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .page-footer {
-  padding: 0 var(--footer-horizontal-spacing);
+  padding: 10px var(--footer-horizontal-spacing);
 }
 
 .docs-footer {
-  background-color: red;
+  background-color: var(--background-color);
   border-top: 1px solid var(--separator-color);
   color: inherit;
   position: relative;
   z-index: 1000;
 
   .footer-copyright,
   .footer-copyright a {
@@ -19,12 +19,12 @@
 .sphinx-version {
   margin-bottom: 0;
   margin-top: 0;
 }
 
 .stm-content-footer {
   margin-top: auto;
-  padding: 10px 20px;
+  padding: 10px var(--footer-horizontal-spacing);
   border-top: 1px solid var(--separator-color);
   background-color: var(--background-color);
   color: var(--font-color-medium);
 }
```

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_headnav.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_headnav.scss`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 }
 
 .headnav-item {
   display: flex;
   align-items: center;
 }
 
+.headnav-persistent--mobile {
+  margin-left: auto;
+
+  @media (min-width: $medium-screen-up) {
+    display: none;
+  }
+}
+
 nav {
   background-color: var(--primary-color);
   position: relative;
 
   @media (min-width: $medium-screen-up) {
     z-index: 1099;
   }
```

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/sections/_stm-sidenav.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_stm-sidenav.scss`

 * *Files 7% similar despite different names*

```diff
@@ -180,27 +180,42 @@
     line-height: 32px;
   }
 
   .dropdown-trigger {
     display: flex;
     align-items: center;
   }
+
+  a.nav-external {
+    display: flex;
+    align-items: center;
+    gap: 0.25rem;
+  }
 }
 
 .sidenav-header-items__end {
   display: block;
 
   ul {
     display: flex;
+    align-items: center;
     gap: 0.5rem;
     margin: 0;
   }
 
   img {
     height: 25px;
     background-color: var(--font-color-main);
   }
 
   a.ext-link {
     display: flex;
   }
+
+  a#theme-switch--mobile {
+    display: flex;
+  }
+
+  i.fa-brands {
+    font-size: 20px;
+  }
 }
```

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_admonitions.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_colors.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/styles/variables/_icons.scss` & `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/translations/README.md` & `stmaterial-0.0.4/src/stmaterial/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/Edit this page.json` & `stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/assets/translations/jsons/On this page.json` & `stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/demo/module.py` & `stmaterial-0.0.4/src/stmaterial/demo/module.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/demo/sphinxext.py` & `stmaterial-0.0.4/src/stmaterial/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/directives.py` & `stmaterial-0.0.4/src/stmaterial/directives.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/base.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/base.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/breadcrumbs.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/edit-this-page.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/postnav.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/postnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/prev-next.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/components/search-field.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-field.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/domainindex.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/domainindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/genindex.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/genindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/layout.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 {% block mainbody -%}
 <div class="stm-main">
     <div class="main-wrapper">
         {% if theme_show_back_to_top %}
         {%- include "components/back-to-top.html" -%}
         {% endif %}
 
-        <aside class="stm-sidenav {% if hide_sidenav %} hide {% endif %} ">
+        {%- include "search-wrapper.html" -%}
+
+        <aside class="stm-sidenav {% if hide_sidenav %} hide-on-large-only {% endif %} ">
             <div class="sidenav-viewport">
                 {% block left_sidebar %}
                 {%- include "sections/sidenav.html" -%}
                 {% endblock left_sidebar %}
             </div>
         </aside>
         <main class="stm-content">
```

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/search.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/search.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/headnav.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/headnav.html`

 * *Files 16% similar despite different names*

```diff
@@ -9,32 +9,47 @@
     </div>
     <div class="headnav-items__content">
         <div class="me-auto headnav-items__center">
             {% include "components/headnav-items.html" %}
         </div>
         <div class="headnav-items__end">
             <div class="headnav-item">
-                <a id="theme-switch" href="#"><i class="material-icons">dark_mode</i></a>
-            </div>
-            <div class="headnav-item">
                 <ul>
+                    <li>
+                        {% include "components/search-button.html" %}
+                    </li>
+                    <li>
+                        <a id="theme-switch" href="#"><i class="material-icons">dark_mode</i></a>
+                    </li>
                     {% if theme_header_icons -%}
                     {% for icon_dict in theme_header_icons -%}
                     <li>
-                        <a href="{{ icon_dict.url }}" target="_blank" aria-label="{{ icon_dict.name }}"
-                            class="ext-link">
+                        <a href="{{ icon_dict.url }}" target="_blank" title="{{ icon_dict.name }}" class="ext-link">
                             {% if icon_dict.class %}
                             <i class="{{ icon_dict.class }}"></i>
                             {% elif icon_dict.svg %}
                             <img src="{{ pathto(icon_dict.svg, 1) }}" style="transform: scale(0.8);">
                             {% elif icon_dict.material_icons %}
                             <i class="material-icons">{{ icon_dict.material_icons }}</i>
+                            {% elif icon_dict.fontawesome %}
+                            <i class="{{ icon_dict.fontawesome }}"></i>
                             {% endif %}
                         </a>
                     </li>
                     {% endfor %}
                     {% endif %}
                 </ul>
             </div>
         </div>
     </div>
+
+    <div class="headnav-persistent--mobile">
+        <ul>
+            <li>
+                {%- include "search-button.html" %}
+            </li>
+            <li>
+                <a id="theme-switch--mobile" href="#"><i class="material-icons">dark_mode</i></a>
+            </li>
+        </ul>
+    </div>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
  menu
 [Logo]
 {% include "components/headnav-items.html" %}
-dark_mode
+    * {% include "components/search-button.html" %}
+    * dark_mode
     * {% if theme_header_icons -%} {% for icon_dict in theme_header_icons -%}
     * {%_if_icon_dict.class_%}__{%_elif_icon_dict.svg_%}_[{{_pathto
       (icon_dict.svg,_1)_}}]_{%_elif_icon_dict.material_icons_%}_{
-      {_icon_dict.material_icons_}}_{%_endif_%}
+      {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_endif
+      %}
     * {% endfor %} {% endif %}
+    * {%- include "search-button.html" %}
+    * dark_mode
```

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/sections/sidenav.html` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/sidenav.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div class="sidenav-drawer">
     <div class="sidenav-logo">
-        {%- include "sidebar/brand.html" %}
+        {%- include "sidenav-brand.html" %}
     </div>
     <div class="sidenav-header-items hide-on-large-only">
         <div class="sidenav-header-items__center">
             <div class="headnav-item">
                 <ul>
                     {{ head_nav_html[1] }}
                 </ul>
@@ -20,14 +20,16 @@
                             class="ext-link">
                             {% if icon_dict.class %}
                             <i class="{{ icon_dict.class }}"></i>
                             {% elif icon_dict.svg %}
                             <img src="{{ pathto(icon_dict.svg, 1) }}" style="transform: scale(0.8);">
                             {% elif icon_dict.material_icons %}
                             <i class="material-icons">{{ icon_dict.material_icons }}</i>
+                            {% elif icon_dict.fontawesome %}
+                            <i class="{{ icon_dict.fontawesome }}"></i>
                             {% endif %}
                         </a>
                     </li>
                     {% endfor %}
                     {% endif %}
                 </ul>
             </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{%- include "sidebar/brand.html" %}
+{%- include "sidenav-brand.html" %}
     * {{ head_nav_html[1] }}
     * {% if theme_header_icons -%} {% for icon_dict in theme_header_icons -%}
     * {%_if_icon_dict.class_%}__{%_elif_icon_dict.svg_%}_[{{_pathto
       (icon_dict.svg,_1)_}}]_{%_elif_icon_dict.material_icons_%}_{
-      {_icon_dict.material_icons_}}_{%_endif_%}
+      {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_endif
+      %}
     * {% endfor %} {% endif %}
 {%- for sidebar_section in sidebars %} {%- include sidebar_section %} {%-
 endfor %}
```

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/static/images/github.svg` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/github.svg`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/src/stmaterial/theme/stmaterial/theme.conf` & `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/theme.conf`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [theme]
 inherit = basic-ng
 stylesheet = styles/stmaterial.css
 pygments_style = tango
 # sidebar-start
-sidebars = sidebar/search.html, sidebar/navigation.html
+sidebars = search-field.html, sidenav-nav.html
 # sidebar-end
 
 [options]
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 logo = 
@@ -25,7 +25,9 @@
 fix_header_nav = 
 light_css_variables =
 dark_css_variables =
 footer = 
 footer_content = components/sphinx-version.html, components/copyright.html
 toc_title = 
 search_bar_text = Search the docs ...
+dropdown_label_name = More
+navigation_with_keys = True
```

### Comparing `stmaterial-0.0.3/src/stmaterial/utils.py` & `stmaterial-0.0.4/src/stmaterial/utils.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/webpack.config.js` & `stmaterial-0.0.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.3/PKG-INFO` & `stmaterial-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmaterial
-Version: 0.0.3
+Version: 0.0.4
 Summary: A sphinx theme of materializecss.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

