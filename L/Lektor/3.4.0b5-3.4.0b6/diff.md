# Comparing `tmp/lektor-3.4.0b5.tar.gz` & `tmp/lektor-3.4.0b6.tar.gz`

## Comparing `lektor-3.4.0b5.tar` & `lektor-3.4.0b6.tar`

### file list

```diff
@@ -1,285 +1,298 @@
--rw-r--r--   0        0        0    38286 2020-02-02 00:00:00.000000 lektor-3.4.0b5/CHANGES.md
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lektor-3.4.0b5/build_frontend.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/__main__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/assets.py
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/build_programs.py
--rw-r--r--   0        0        0    44698 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/builder.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/buildfailures.py
--rw-r--r--   0        0        0    19191 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/cli.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/cli_utils.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/compat.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/constants.py
--rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/context.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/databags.py
--rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/datamodel.py
--rw-r--r--   0        0        0    74852 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/db.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/devcli.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/devserver.py
--rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/editor.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/exception.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/filecontents.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/i18n.py
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/imagetools.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/metaformat.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/packages.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/pagination.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/pluginsystem.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/project.py
--rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/publisher.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/reporter.py
--rw-r--r--   0        0        0     9474 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/sourceobj.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/sourcesearch.py
--rw-r--r--   0        0        0    23592 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/utils.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/videotools.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/watcher.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/__init__.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/context.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/utils.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/webui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/modules/__init__.py
--rw-r--r--   0        0        0    13890 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/modules/api.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/modules/dash.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/modules/livereload.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/modules/serve.py
--rw-r--r--   0        0        0   184378 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/app.css
--rw-r--r--   0        0        0   244973 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/app.css.map
--rw-r--r--   0        0        0   487431 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/app.js
--rw-r--r--   0        0        0   645402 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/app.js.map
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-3KIJVIEY.svg
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-FMJ3VJ65.eot
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-RJ6LE7IU.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-Z4ARLA73.woff
--rw-r--r--   0        0        0    71752 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/roboto-slab-all-300-CD7CKZ7B.woff
--rw-r--r--   0        0        0    57232 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/roboto-slab-all-300-ZPJL4QTS.woff2
--rw-r--r--   0        0        0    56724 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/roboto-slab-all-400-26JDMZKQ.woff2
--rw-r--r--   0        0        0    71132 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/static/roboto-slab-all-400-JK3TGTJI.woff
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/base.html
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/build-failure.html
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/dash.html
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/edit-button.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/layout.html
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/livereload-worker.js
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/admin/templates/livereload.html
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/environment/__init__.py
--rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/environment/config.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/environment/expressions.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/markdown/__init__.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/markdown/controller.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/markdown/mistune0.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/markdown/mistune2.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/plugin/.gitignore.in
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/plugin/@plugin_module@.py.in
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/plugin/README.md.in
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/plugin/pyproject.toml.in
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/plugin/setup.cfg.in
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/@project_name@.lektorproject.in
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/assets/static/style.css.in
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/content/contents.lr.in
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/content/about/contents.lr.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/content/blog/contents.lr.in
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/content/blog/first-post/contents.lr.in
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/content/projects/contents.lr.in
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/models/blog-post.ini.in
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/models/blog.ini.in
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/models/page.ini.in
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/blog-post.html.in
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/blog.html.in
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/layout.html.in
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/page.html.in
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/macros/blog.html.in
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/project/templates/macros/pagination.html.in
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/theme/README.md.in
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/theme/theme.ini.in
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/theme/example-site/README.md.in
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/theme/example-site/lektor-theme-@theme_id@.lektorproject.in
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/quickstart-templates/theme/images/homepage.png
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/ca.json
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/de.json
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/en.json
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/es.json
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/fr.json
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/it.json
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/ja.json
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/ko.json
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/nl.json
--rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/pl.json
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/pt.json
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/ru.json
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/translations/zh.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/base.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/fake.py
--rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/flow.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/formats.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/multi.py
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/primitives.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 lektor-3.4.0b5/lektor/types/special.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/conftest.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/markers.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_assets.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_build_frontend.py
--rw-r--r--   0        0        0    11116 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_builder.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_buildfailures.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_cli.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_compat.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_config.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_datamodel.py
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_db.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_deploy.py
--rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_devcli.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_editor.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_environment.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_filecontents.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_i18n.py
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_images.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_imports.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_issue_410.py
--rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_markdown.py
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_packages.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_pagination.py
--rw-r--r--   0        0        0    12578 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_pluginsystem.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_prev_next_sibling.py
--rw-r--r--   0        0        0    20367 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_publisher.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_quickstart.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_sourceobj.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_themes.py
--rw-r--r--   0        0        0    13013 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_tree.py
--rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_types.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_unicode.py
--rw-r--r--   0        0        0    12700 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_urls.py
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_utils.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_videotools.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/test_watcher.py
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/admin/test_api.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/admin/test_dash.py
--rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/admin/test_serve.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/admin/test_webui.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/Website.lektorproject
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/content/attachment.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/content/contents.lr
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/content/filtered-page/contents.lr
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/models/bar.ini
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/models/foo.ini
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/models/page.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/templates/bar.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/templates/foo.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/child-sources-test-project/templates/page.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/Website.lektorproject
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/_include_me_despite_underscore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/foo-prefix-makes-me-excluded
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/dir_with_index_htm/index.htm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/dir_with_index_html/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/empty/.gitkeep
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/assets/static/demo.css
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/contents.lr
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/hello.txt
--rw-r--r--   0        0        0   201837 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/test-progressive.jpg
--rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/test-sof-last.jpg
--rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/test.jpg
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/test.mp4
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/blog/contents.lr
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/blog/dummy.xml/contents.lr
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/blog/post1/contents.lr
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/blog/post1/hello.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/blog/post2/contents.lr
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/contents.lr
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/hello.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/a/contents.lr
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/b/contents.lr
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/container/contents.lr
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/container/hello.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/container/a/contents.lr
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/file.ext/contents.lr
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/paginated/contents+de.lr
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/paginated/contents.lr
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/extra/slash-slug/contents.lr
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/attachment.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/contents.lr
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/bagpipe/contents+de.lr
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/bagpipe/contents.lr
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/coffee/contents+de.lr
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/coffee/contents.lr
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/filtered/contents.lr
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/master/contents+de.lr
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/master/contents.lr
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/oven/contents+de.lr
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/oven/contents.lr
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/postage/contents+de.lr
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/postage/contents.lr
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/secret/contents.lr
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/slave/contents+de.lr
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/slave/contents.lr
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/wolf/contents.lr
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/content/projects/zaun/contents+de.lr
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/flowblocks/text.ini
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/blog-post.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/blog.ini
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/container.ini
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/page.ini
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/paginated.ini
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/project.ini
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/models/projects.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/blog-post.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/blog.html
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/dummy.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/layout.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/page.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/project.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/projects.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/demo-project/templates/blocks/text.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/Website.lektorproject
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/content/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/content/post1/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/content/post2/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/content/post4/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/models/blog-post.ini
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/models/blog.ini
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/templates/blog-post.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/dependency-test-project/templates/blog.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/pep660-dummy-plugin/lektor_dummy_plugin.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/pep660-dummy-plugin/pyproject.toml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/assets/asset.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/assets/dummy.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/flowblocks/text.ini
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/models/blog-post.ini
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/models/page.ini
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/templates/layout.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/templates/page.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/templates/blocks/text.html
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/theme.ini
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/assets/dummy.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/assets/dummy2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/assets/static/blog.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/models/blog-post.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/models/blog.ini
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/models/project.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/templates/blog-post.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/templates/blog.html
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/templates/dummy.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/blog_theme/templates/layout.html
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/theme.ini
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/assets/dummy2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/assets/static/project.css
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/flowblocks/text.ini
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/models/project.ini
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/models/projects.ini
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/templates/dummy.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/templates/layout.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/templates/project.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/templates/projects.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/themes-project/themes/project_theme/templates/blocks/text.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/test.lektorproject
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/content/contents.lr
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/content/ättachment
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/content/bäd/contents.lr
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/models/page.ini
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lektor-3.4.0b5/tests/ünicöde-project/templates/page.html
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 lektor-3.4.0b5/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 lektor-3.4.0b5/LICENSE
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 lektor-3.4.0b5/README.md
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 lektor-3.4.0b5/pyproject.toml
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 lektor-3.4.0b5/PKG-INFO
+-rw-r--r--   0        0        0    43784 2020-02-02 00:00:00.000000 lektor-3.4.0b6/CHANGES.md
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lektor-3.4.0b6/build_frontend.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/__main__.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/assets.py
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/build_programs.py
+-rw-r--r--   0        0        0    44698 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/builder.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/buildfailures.py
+-rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/cli.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/cli_utils.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/compat.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/constants.py
+-rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/context.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/databags.py
+-rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/datamodel.py
+-rw-r--r--   0        0        0    75332 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/db.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/devcli.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/devserver.py
+-rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/editor.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/exception.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/filecontents.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/i18n.py
+-rw-r--r--   0        0        0    25049 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/imagetools.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/metaformat.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/packages.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/pagination.py
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/pluginsystem.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/project.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/publisher.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/reporter.py
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/sourceobj.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/sourcesearch.py
+-rw-r--r--   0        0        0    27157 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/utils.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/videotools.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/watcher.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/__init__.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/context.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/utils.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/webui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/__init__.py
+-rw-r--r--   0        0        0    13890 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/api.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/dash.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/livereload.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/serve.py
+-rw-r--r--   0        0        0   188451 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.css
+-rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.css.map
+-rw-r--r--   0        0        0   587740 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.js
+-rw-r--r--   0        0        0   374972 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.js.map
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-400-normal-72U6HY3C.woff2
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-700-normal-2TPID6WR.woff2
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2
+-rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-400-normal-FZE4RLDU.woff2
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-700-normal-5YAILM42.woff2
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-400-normal-CARBXC53.woff2
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-700-normal-MWV52O3F.woff2
+-rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-400-normal-WDWDTZK2.woff2
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-700-normal-VK4QNPMO.woff2
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-400-normal-66GAUH66.woff2
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/base.html
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/build-failure.html
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/dash.html
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/edit-button.html
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/layout.html
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/livereload-worker.js
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/livereload.html
+-rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/__init__.py
+-rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/config.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/expressions.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/controller.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/mistune0.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/mistune2.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/.gitignore.in
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/@plugin_module@.py.in
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/README.md.in
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/pyproject.toml.in
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/setup.cfg.in
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/@project_name@.lektorproject.in
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/assets/static/style.css.in
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/contents.lr.in
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/about/contents.lr.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/blog/contents.lr.in
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/blog/first-post/contents.lr.in
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/projects/contents.lr.in
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/blog-post.ini.in
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/blog.ini.in
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/page.ini.in
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/blog-post.html.in
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/blog.html.in
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/layout.html.in
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/page.html.in
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/blog.html.in
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/pagination.html.in
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/README.md.in
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/theme.ini.in
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/example-site/README.md.in
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/example-site/lektor-theme-@theme_id@.lektorproject.in
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/images/homepage.png
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ca.json
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/de.json
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/en.json
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/es.json
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/fr.json
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/it.json
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ja.json
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ko.json
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/nl.json
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/pl.json
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/pt.json
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ru.json
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/zh.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/base.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/fake.py
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/flow.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/formats.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/multi.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/primitives.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/special.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/conftest.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_assets.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_build_frontend.py
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_builder.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_buildfailures.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_cli.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_cli_utils.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_compat.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_config.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_conftest.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_datamodel.py
+-rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_db.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_deploy.py
+-rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_devcli.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_editor.py
+-rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_environment.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_filecontents.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_i18n.py
+-rw-r--r--   0        0        0    21458 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_imagetools.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_imports.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_issue_410.py
+-rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_markdown.py
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_packages.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_pagination.py
+-rw-r--r--   0        0        0    12630 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_pluginsystem.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_prev_next_sibling.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_project.py
+-rw-r--r--   0        0        0    21409 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_publisher.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_quickstart.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_sourceobj.py
+-rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_themes.py
+-rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_tree.py
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_types.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_unicode.py
+-rw-r--r--   0        0        0    15464 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_urls.py
+-rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_utils.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_videotools.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_watcher.py
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_api.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_dash.py
+-rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_serve.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_webui.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/Website.lektorproject
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/attachment.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/contents.lr
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/filtered-page/contents.lr
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/bar.ini
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/foo.ini
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/page.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/bar.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/foo.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/page.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/Website.lektorproject
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/_include_me_despite_underscore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/foo-prefix-makes-me-excluded
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/dir_with_index_htm/index.htm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/dir_with_index_html/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/empty/.gitkeep
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/static/demo.css
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/contents.lr
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/hello.txt
+-rw-r--r--   0        0        0   201837 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test-progressive.jpg
+-rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test-sof-last.jpg
+-rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test.jpg
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test.mp4
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/contents.lr
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/dummy.xml/contents.lr
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post1/contents.lr
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post1/hello.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post2/contents.lr
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/LICENSE.txt
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/README.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/contents.lr
+-rw-r--r--   0        0        0    32912 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/rgb-to-gbr-test.jpg
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/contents.lr
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/hello.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/a/contents.lr
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/b/contents.lr
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/contents.lr
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/hello.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/a/contents.lr
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/file.ext/contents.lr
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/paginated/contents+de.lr
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/paginated/contents.lr
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/slash-slug/contents.lr
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/attachment.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/contents.lr
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/bagpipe/contents+de.lr
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/bagpipe/contents.lr
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/coffee/contents+de.lr
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/coffee/contents.lr
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/filtered/contents.lr
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/master/contents+de.lr
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/master/contents.lr
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/oven/contents+de.lr
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/oven/contents.lr
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/postage/contents+de.lr
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/postage/contents.lr
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/secret/contents.lr
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/slave/contents+de.lr
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/slave/contents.lr
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/wolf/contents.lr
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/zaun/contents+de.lr
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/flowblocks/text.ini
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/blog-post.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/blog.ini
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/container.ini
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/page.ini
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/paginated.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/project.ini
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/projects.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blog-post.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blog.html
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/colorspace-test.html
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/dummy.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/layout.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/page.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/project.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/projects.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blocks/text.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/Website.lektorproject
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post1/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post2/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post4/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/models/blog-post.ini
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/models/blog.ini
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/templates/blog-post.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/templates/blog.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/pep660-dummy-plugin/lektor_dummy_plugin.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/pep660-dummy-plugin/pyproject.toml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/assets/asset.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/assets/dummy.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/flowblocks/text.ini
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/models/blog-post.ini
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/models/page.ini
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/layout.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/page.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/blocks/text.html
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/theme.ini
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/dummy.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/dummy2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/static/blog.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/blog-post.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/blog.ini
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/project.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/blog-post.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/blog.html
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/dummy.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/layout.html
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/theme.ini
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/assets/dummy2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/assets/static/project.css
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/flowblocks/text.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/models/project.ini
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/models/projects.ini
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/dummy.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/layout.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/project.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/projects.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/blocks/text.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/test.lektorproject
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/contents.lr
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/ättachment
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/bäd/contents.lr
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/models/page.ini
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/templates/page.html
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 lektor-3.4.0b6/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 lektor-3.4.0b6/LICENSE
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/README.md
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 lektor-3.4.0b6/pyproject.toml
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 lektor-3.4.0b6/PKG-INFO
```

### Comparing `lektor-3.4.0b5/CHANGES.md` & `lektor-3.4.0b6/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,129 @@
 # Changelog
 
 These are all the changes in Lektor since the first public release.
 
+## 3.4.0b6 (2023-05-05)
+
+### Possibly Breaking Changes
+
+- Our Publisher API has changed. This will eventually require updates
+  to any custom Publisher classes provided by Lektor
+  plugins. Previously, the `publish` method of `Publisher` subclasses
+  was passed a `werkzeug.urls.URL` instance as its `target_url`
+  argument. Werkzeug has deprecated the `URL` class, so now the
+  `target_url` will be passed as a string. (The publishers are now
+  responsible for was parsing the target URL themselves.) For the
+  interim, in an effort to avoid immediately breaking existing
+  plugins, we pass a fancy subclass of `str` that implements most of
+  the attributes and methods of `werkzeug.urls.URL`. ([#1143], [#1142])
+
+- Interpret relative paths passed via the `--output-path` command-line
+  parameter relative to the current working directory. Interpret
+  relative paths configured for `output_path` in the _project file_
+  relative to the directory containing the project file (as the
+  [docs](https://www.getlektor.com/docs/project/file/#project) claim
+  should happen). Previously, both paths were interpreted —
+  incorrectly, in both cases — relative to the _project directory_.
+  ([#1103], [#1120])
+
+- The `query` attribute of fields of type `"url"` now returns the
+  IRI-encoded (internationalized) version of the URL query. (This
+  matches the existing behavior of the `host`, `path`, and `anchor`
+  attributes.) ([#1143])
+
+### Deprecations
+
+- The (unused) `lektor.db.Pad.make_absolute_url` method is deprecated. ([#1143])
+
+### Features
+
+- We now use [Pillow] (instead of ImageMagick) to generate image
+  thumbnails. Installation of ImageMagick was a significant pain-point
+  for some. In addition the Pillow-based thumbnailing code appears to
+  be noticeably faster than the ImageMagick version. ([#1104])
+
+- A _Preferences Dialog_ has been added to the admin GUI that allows
+  customization of which hotkeys trigger the _Save_, _Edit_,
+  _(Save &) Preview_, and _Search_ actions. ([#1052])
+
+### Bugs Fixed
+
+- Re-export `ImprovedRenderer`, `MarkdownConfig`, and `escape` from
+  `lektor.markdown`. These were removed in [#992] when support for
+  mistune 2.x was added. Restoring them allows most older plugins
+  written for Lektor<3.4 to work, so long as mistune is pinned to
+  version 0.x. ([#1134])
+
+- Better input validation and error reporting for the `dateformat`,
+  `timeformat` and `datetimeformat` jinja filters. Previously, these
+  filters did not handle unexpected input types gracefully. ([#1122],
+  [#1121])
+
+- Allow the user to customize the python [warnings filter] when
+  running the CLI. Previously, Lektor unconditionally set the
+  warnings filter to `"default"` (enabling one-shot display of _all_
+  warning types.) Now, if the warnings filter has been explicitly set
+  (via [PYTHONWARNINGS] or [-W][python-W]) it is left
+  alone. ([e2d0274])
+- DB-path URL resolution of relative paths from _virtual source objects_. ([#1133])
+
+- Relative URL-path resolution from pages with "." in their slug. ([#1133])
+
+- Avoid the use of `warnings.catch_warnings` which was introduced in
+  [#1113]. Its use resets the warnings registry resulting in undesired
+  repition of seen warnings. ([#1135]).
+
+### Bit-Rot
+
+- Update frontend npm dependencies. ([#1126])
+
+### Other Changes
+
+- Use [watchfiles] instead of `watchdog` when monitoring for file changes. ([#1136])
+
+- Optimization: Thumbnail file names are now generated based on the
+  final thumbnail parameters (e.g. their actual dimensions, rather than
+  their requested dimensions.) This minimizes the possibility of generating
+  multiple identical thumbnails with different file names. ([#1139])
+
+- Tighten [click] constraints on Path parameters. This results in
+  better and earlier error messages when, e.g., a readable file is
+  expected, but a path to a directory is passed. ([#1124])
+
+- We reduced the size of our distribution wheel and sdist files by
+  roughly factor of two by omitting all but the `.woff2` variants of
+  the fonts for the frontend, and by excluding [sourcesContent] from
+  the JS and CSS sourcemaps. ([#1130], [#1115])
+
+[e2d0274]: https://github.com/lektor/lektor/commit/e2d02746a488e4a4d05ba8a01443e7a90315a2fb
+[#1052]: https://github.com/lektor/lektor/pull/1052
+[#1103]: https://github.com/lektor/lektor/issues/1103
+[#1104]: https://github.com/lektor/lektor/pull/1104
+[#1115]: https://github.com/lektor/lektor/issues/1115
+[#1120]: https://github.com/lektor/lektor/pull/1120
+[#1121]: https://github.com/lektor/lektor/issues/1121
+[#1122]: https://github.com/lektor/lektor/pull/1122
+[#1124]: https://github.com/lektor/lektor/pull/1124
+[#1126]: https://github.com/lektor/lektor/pull/1126
+[#1130]: https://github.com/lektor/lektor/pull/1130
+[#1133]: https://github.com/lektor/lektor/pull/1133
+[#1134]: https://github.com/lektor/lektor/pull/1134
+[#1136]: https://github.com/lektor/lektor/pull/1136
+[#1139]: https://github.com/lektor/lektor/pull/1139
+[#1142]: https://github.com/lektor/lektor/issues/1142
+[#1143]: https://github.com/lektor/lektor/pull/1143
+[click]: https://pypi.org/project/click/
+[warnings filter]: https://docs.python.org/3/library/warnings.html#the-warnings-filter
+[PYTHONWARNINGS]: https://docs.python.org/3/using/cmdline.html#envvar-PYTHONWARNINGS
+[python-W]: https://docs.python.org/3/using/cmdline.html#cmdoption-W
+[Pillow]: https://pillow.readthedocs.io/en/stable/
+[sourcesContent]: https://esbuild.github.io/api/#sources-content
+[watchfiles]: https://github.com/samuelcolvin/watchfiles
+
 ## 3.4.0b5 (2023-03-08)
 
 ### Breaking Changes
 
 - Removed the `lektor dev publish-plugin` command. (To publish a
   plugin to PyPI, use [twine].) ([#1065])
```

### Comparing `lektor-3.4.0b5/build_frontend.py` & `lektor-3.4.0b6/build_frontend.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tox.ini` & `lektor-3.4.0b6/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -2,47 +2,52 @@
 minversion = 4.1
 envlist =
     lint
     {py37,py38,py39,py310,py311}{,-mistune0}
     py311-noutils
     py311-pytz
     py311-tzdata
+    py38-pillow6
+    py38-pillow7
     cover-{clean,report}
 isolated_build = true
 
 [gh-actions]
 python =
     3.7: py37, cover
     3.8: py38, cover
     3.9: py39, cover
     3.10: py310, cover
     3.11: py311, cover
 
 [testenv]
 commands =
-    coverage run -m pytest {posargs:tests -ra}
+    coverage run -m pytest {posargs:tests -ra --durations=20}
 passenv = USERNAME
 setenv =
     # skip building frontend js/css
     HATCH_BUILD_NO_HOOKS=true
+    # do not run marked slow tests in every variant testenv
+    {mistune0,noutils,pytz,tzdata}: PYTEST_ADDOPTS=-m "not slowtest"
 deps =
     pytest>=6
     pytest-click
     pytest-mock
     coverage[toml]
     importlib_metadata; python_version<"3.10"
     iniconfig
     hatchling
     mistune0: mistune<2
     pytz: pytz
     tzdata: tzdata
+    pillow6: pillow<6.1.0
+    pillow7: pillow<7.1.0
 depends =
-    py{37,38,39,310,311}{,-mistune0,-noutils}: cover-clean
-    cover-report: py{37,38,39,310,311}{,-mistune0,-noutils}
-
+    py{37,38,39,310,311}: cover-clean
+    cover-report: py{37,38,39,310,311}{,-mistune0,-noutils,-pytz,-tzdata,-pillow6,-pillow7}
 # XXX: I've been experiencing sporadic failures when running tox in parallel mode.
 # The crux of the error messages when this happens appears to be something like:
 #
 #     WARNING: Skipping page https://pypi.org/simple/coverage/ because the GET request
 #         got Content-Type: Unknown. The only supported Content-Types are
 #         application/vnd.pypi.simple.v1+json, application/vnd.pypi.simple.v1+html, and
 #         text/html
@@ -55,19 +60,19 @@
 # Setting download=true — which tells tox to upgrade pip to the latest version —
 # seems to fix the issue for me.
 #
 # Hopefully, at some point this can be removed.
 download = true
 
 [testenv:py{37,38,39,310,311}-noutils]
-# To test in environment without external utitilities like imagemagick and git installed,
+# To test in environment without external utitilities like ffmpeg and git installed,
 # break PATH in noutils environment(s).
 allowlist_externals = env
 commands =
-    env PATH="{env_bin_dir}" coverage run -m pytest {posargs:tests -ra}
+    env PATH="{env_bin_dir}" coverage run -m pytest {posargs:tests -ra --durations=20}
 
 [testenv:lint]
 use_develop = true
 deps =
     pylint==2.15.8
     pytest>=6
     pytest-mock
```

### Comparing `lektor-3.4.0b5/lektor/assets.py` & `lektor-3.4.0b6/lektor/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,10 +125,14 @@
     @property
     def url_path(self):
         path = super().url_path
         if not path.endswith("/"):
             path += "/"
         return path
 
+    @property
+    def url_content_path(self):
+        return self.url_path
+
 
 class File(Asset):
     """Represents a static asset file."""
```

### Comparing `lektor-3.4.0b5/lektor/build_programs.py` & `lektor-3.4.0b6/lektor/build_programs.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/builder.py` & `lektor-3.4.0b6/lektor/builder.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/buildfailures.py` & `lektor-3.4.0b6/lektor/buildfailures.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/cli.py` & `lektor-3.4.0b6/lektor/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # pylint: disable=import-outside-toplevel
 import os
 import sys
-import time
 import warnings
+from itertools import chain
 
 import click
 
 from lektor.cli_utils import AliasedGroup
 from lektor.cli_utils import echo_json
 from lektor.cli_utils import extraflag
 from lektor.cli_utils import pass_context
 from lektor.cli_utils import pruneflag
+from lektor.cli_utils import ResolvedPath
 from lektor.cli_utils import validate_language
 from lektor.compat import importlib_metadata as metadata
 from lektor.project import Project
 from lektor.utils import profile_func
 from lektor.utils import secure_url
 
 
 version = metadata.version("Lektor")
 
 
 @click.group(cls=AliasedGroup)
 @click.option(
-    "--project", type=click.Path(), help="The path to the lektor project to work with."
+    "--project",
+    type=click.Path(exists=True),
+    help="The path to the lektor project to work with.",
 )
 @click.option(
     "--language",
     default=None,
     callback=validate_language,
     help="The UI language to use (overrides autodetection).",
 )
@@ -35,24 +38,29 @@
 @pass_context
 def cli(ctx, project=None, language=None):
     """The lektor management application.
 
     This command can invoke lektor locally and serve up the website.  It's
     intended for local development of websites.
     """
-    warnings.simplefilter("default")
+    if not sys.warnoptions:
+        warnings.simplefilter("default")
     if language is not None:
         ctx.ui_lang = language
     if project is not None:
         ctx.set_project_path(project)
 
 
 @cli.command("build")
 @click.option(
-    "-O", "--output-path", type=click.Path(), default=None, help="The output path."
+    "-O",
+    "--output-path",
+    type=ResolvedPath(writable=True, file_okay=False),
+    default=None,
+    help="The output path.",
 )
 @click.option(
     "--watch",
     is_flag=True,
     help="If this is enabled the build "
     "process goes into an automatic loop where it watches the "
     "file system for changes and rebuilds.",
@@ -71,15 +79,15 @@
     help="Instead of building only updates the source infos.  The "
     "source info is used by the web admin panel to quickly find "
     "information about the source files (for instance jump to "
     "files).",
 )
 @click.option(
     "--buildstate-path",
-    type=click.Path(),
+    type=click.Path(writable=True, file_okay=False),
     default=None,
     help="Path to a directory that Lektor will use for coordinating "
     "the state of the build. Defaults to a directory named "
     "`.lektor` inside the output path.",
 )
 @extraflag
 @click.option("--profile", is_flag=True, help="Enable build profiler.")
@@ -118,52 +126,54 @@
     if output_path is None:
         output_path = ctx.get_default_output_path()
 
     ctx.load_plugins(extra_flags=extra_flags)
 
     env = ctx.get_env()
 
-    def _build():
-        builder = Builder(
-            env.new_pad(),
-            output_path,
-            buildstate_path=buildstate_path,
-            extra_flags=extra_flags,
-        )
-        if source_info_only:
-            builder.update_all_source_infos()
-            return True
+    with CliReporter(env, verbosity=verbosity):
+        builds = ["first"]
+        if watch:
+            from lektor.watcher import watch_project
+
+            click.secho("Watching for file system changes", fg="cyan")
+            builds = chain(
+                builds, watch_project(env, output_path, raise_interrupt=False)
+            )
 
-        if profile:
-            failures = profile_func(builder.build_all)
-        else:
-            failures = builder.build_all()
-        if prune:
-            builder.prune()
-        return failures == 0
+        success = False
+        for _ in builds:
+            builder = Builder(
+                env.new_pad(),
+                output_path,
+                buildstate_path=buildstate_path,
+                extra_flags=extra_flags,
+            )
+            if source_info_only:
+                builder.update_all_source_infos()
+                success = True
+            else:
+                if profile:
+                    failures = profile_func(builder.build_all)
+                else:
+                    failures = builder.build_all()
+                if prune:
+                    builder.prune()
+                success = failures == 0
 
-    reporter = CliReporter(env, verbosity=verbosity)
-    with reporter:
-        success = _build()
-        if not watch:
-            return sys.exit(0 if success else 1)
-
-        from lektor.watcher import watch
-
-        click.secho("Watching for file system changes", fg="cyan")
-        last_build = time.time()
-        for ts, _, _ in watch(env):
-            if ts > last_build:
-                _build()
-                last_build = time.time()
+        return sys.exit(0 if success else 1)
 
 
 @cli.command("clean")
 @click.option(
-    "-O", "--output-path", type=click.Path(), default=None, help="The output path."
+    "-O",
+    "--output-path",
+    type=ResolvedPath(writable=True, file_okay=False),
+    default=None,
+    help="The output path.",
 )
 @click.option(
     "-v",
     "--verbose",
     "verbosity",
     count=True,
     help="Increases the verbosity of the logging.",
@@ -191,15 +201,19 @@
         builder = Builder(env.new_pad(), output_path)
         builder.prune(all=True)
 
 
 @cli.command("deploy", short_help="Deploy the website.")
 @click.argument("server", required=False)
 @click.option(
-    "-O", "--output-path", type=click.Path(), default=None, help="The output path."
+    "-O",
+    "--output-path",
+    type=ResolvedPath(writable=True, file_okay=False),
+    default=None,
+    help="The output path.",
 )
 @click.option(
     "--username",
     envvar="LEKTOR_DEPLOY_USERNAME",
     help="An optional username to override the URL.",
 )
 @click.option(
@@ -296,15 +310,15 @@
 )
 @click.option(
     "-p", "--port", default=5000, help="The port to bind to.", show_default=True
 )
 @click.option(
     "-O",
     "--output-path",
-    type=click.Path(),
+    type=ResolvedPath(writable=True, file_okay=False),
     default=None,
     help="The dev server will build into the same folder as "
     "the build command by default.",
 )
 @pruneflag
 @click.option(
     "-v",
@@ -409,15 +423,15 @@
         click.echo("Package Cache: %s" % json_data["package_cache_path"])
 
 
 @cli.command(
     "content-file-info", short_help="Provides information for " "a set of lektor files."
 )
 @click.option("as_json", "--json", is_flag=True, help="Prints out the data as json.")
-@click.argument("files", nargs=-1, type=click.Path())
+@click.argument("files", nargs=-1, type=click.Path(dir_okay=False))
 @pass_context
 def content_file_info_cmd(ctx, files, as_json):
     """Given a list of files this returns the information for those files
     in the context of a project.  If the files are from different projects
     an error is generated.
     """
     project = None
@@ -600,15 +614,19 @@
     the plugins again.
     """
     ctx.load_plugins(reinstall=True)
 
 
 @cli.command("quickstart", short_help="Starts a new empty project.")
 @click.option("--name", help="The name of the project.")
-@click.option("--path", type=click.Path(), help="Output directory")
+@click.option(
+    "--path",
+    type=click.Path(file_okay=False, dir_okay=False, writable=True),
+    help="Output directory",
+)
 @pass_context
 def quickstart_cmd(ctx, **options):
     """Starts a new empty project with a minimum boilerplate."""
     from lektor.quickstart import project_quickstart
 
     project_quickstart(options)
```

### Comparing `lektor-3.4.0b5/lektor/cli_utils.py` & `lektor-3.4.0b6/lektor/cli_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # pylint: disable=import-outside-toplevel
+from __future__ import annotations
+
 import json
 import os
+from pathlib import Path
+from typing import Any
 
 import click
 
 from lektor.i18n import get_default_lang
 from lektor.i18n import is_valid_language
 from lektor.project import Project
 
@@ -123,7 +127,30 @@
 pass_context = click.make_pass_decorator(Context, ensure=True)
 
 
 def validate_language(ctx, param, value):
     if value is not None and not is_valid_language(value):
         raise click.BadParameter('Unsupported language "%s".' % value)
     return value
+
+
+class ResolvedPath(click.Path):
+    """A click paramter type for a resolved path.
+
+    We could just use ``click.Path(resolve_path=True)`` except that that
+    fails sometimes under Windows running python <= 3.9.
+
+    See https://github.com/pallets/click/issues/2466
+    """
+
+    def __init__(self, writable=False, file_okay=True):
+        super().__init__(
+            resolve_path=True, allow_dash=False, writable=writable, file_okay=file_okay
+        )
+
+    def convert(
+        self, value: Any, param: click.Parameter | None, ctx: click.Context | None
+    ) -> Any:
+        abspath = Path(value).absolute()
+        # fsdecode to ensure that the return value is a str.
+        # (with click<8.0.3 Path.convert will return Path if passed a Path)
+        return os.fsdecode(super().convert(abspath, param, ctx))
```

### Comparing `lektor-3.4.0b5/lektor/context.py` & `lektor-3.4.0b6/lektor/context.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/databags.py` & `lektor-3.4.0b6/lektor/databags.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/datamodel.py` & `lektor-3.4.0b6/lektor/datamodel.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/db.py` & `lektor-3.4.0b6/lektor/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import os
 import posixpath
 from collections import OrderedDict
 from datetime import timedelta
 from functools import total_ordering
 from itertools import islice
 from operator import methodcaller
+from urllib.parse import urljoin
 
 from jinja2 import is_undefined
 from jinja2 import Undefined
 from jinja2.exceptions import UndefinedError
 from jinja2.utils import LRUCache
-from werkzeug.urls import url_join
 from werkzeug.utils import cached_property
 
 from lektor import metaformat
 from lektor.assets import Directory
 from lektor.constants import PRIMARY_ALT
 from lektor.context import Context
 from lektor.context import get_ctx
@@ -570,14 +570,25 @@
                 "When file extension is provided pagination cannot be used."
             )
         # pagination is enabled
         if self.page_num in (1, None):
             return path.rstrip("/") + "/"
         return f"{path.rstrip('/')}/{pg.url_suffix.strip('/')}/{self.page_num:d}/"
 
+    @property
+    def url_content_path(self):
+        """URL path to the directory that contains children of this record."""
+        url_path = self.url_path
+        if url_path.endswith("/"):
+            return url_path
+        # See https://www.getlektor.com/docs/content/urls/#content-below-dotted-slugs
+        head, sep, tail = url_path.rpartition("/")
+        assert "." in tail
+        return f"{head}{sep}_{tail}/"
+
     def resolve_url_path(self, url_path):
         pg = self.datamodel.pagination_config
 
         # If we hit the end of the url path, then we found our target.
         # However if pagination is enabled we want to resolve the first
         # page instead of the unpaginated version.
         if not url_path:
@@ -1576,23 +1587,24 @@
         return self.db.config
 
     @property
     def env(self):
         """The env for this pad."""
         return self.db.env
 
+    @deprecated("use Pad.make_url instead", version="3.4.0")
     def make_absolute_url(self, url):
         """Given a URL this makes it absolute if this is possible."""
         base_url = self.db.config["PROJECT"].get("url")
         if base_url is None:
             raise RuntimeError(
                 "To use absolute URLs you need to configure "
                 "the URL in the project config."
             )
-        return url_join(base_url.rstrip("/") + "/", url.lstrip("/"))
+        return urljoin(base_url.rstrip("/") + "/", url.lstrip("/"))
 
     def make_url(self, url, base_url=None, absolute=None, external=None):
         """Helper method that creates a finalized URL based on the parameters
         provided and the config.
 
         :param url: URL path (starting with "/") relative to the
             configured base_path.
@@ -1609,17 +1621,17 @@
         if external:
             external_base_url = self.db.config.base_url
             if external_base_url is None:
                 raise RuntimeError(
                     "To use absolute URLs you need to "
                     "configure the URL in the project config."
                 )
-            return url_join(external_base_url, url.lstrip("/"))
+            return urljoin(external_base_url, url.lstrip("/"))
         if absolute:
-            return url_join(self.db.config.base_path, url.lstrip("/"))
+            return urljoin(self.db.config.base_path, url.lstrip("/"))
         if base_url is None:
             raise RuntimeError(
                 "Cannot calculate a relative URL if no base URL has been provided."
             )
         return make_relative_url(base_url, url)
 
     def resolve_url_path(
```

### Comparing `lektor-3.4.0b5/lektor/devcli.py` & `lektor-3.4.0b6/lektor/devcli.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/devserver.py` & `lektor-3.4.0b6/lektor/devserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os
 import threading
 import time
 import traceback
+from itertools import chain
 
 from werkzeug.serving import run_simple
 from werkzeug.serving import WSGIRequestHandler
 
 from lektor.admin import WebAdmin
 from lektor.builder import Builder
 from lektor.db import Database
 from lektor.reporter import CliReporter
 from lektor.utils import process_extra_flags
-from lektor.watcher import Watcher
+from lektor.watcher import watch_project
 
 
 class SilentWSGIRequestHandler(WSGIRequestHandler):
     def log(self, type, message, *args):
         pass
 
 
 class BackgroundBuilder(threading.Thread):
     def __init__(self, env, output_path, prune=True, verbosity=0, extra_flags=None):
         threading.Thread.__init__(self)
         self.env = env
         self.output_path = output_path
         self.prune = prune
         self.verbosity = verbosity
-        self.last_build = time.time()
         self.extra_flags = extra_flags
 
     def build(self, update_source_info_first=False):
         try:
             db = Database(self.env)
             builder = Builder(
                 db.new_pad(), self.output_path, extra_flags=self.extra_flags
@@ -38,24 +38,21 @@
             if update_source_info_first:
                 builder.update_all_source_infos()
             builder.build_all()
             if self.prune:
                 builder.prune()
         except Exception:
             traceback.print_exc()
-        else:
-            self.last_build = time.time()
 
     def run(self):
+        builds = chain(["first"], watch_project(self.env, self.output_path))
         with CliReporter(self.env, verbosity=self.verbosity):
-            self.build(update_source_info_first=True)
-            with Watcher(self.env, self.output_path) as watcher:
-                for ts, _, _ in watcher:
-                    if self.last_build is None or ts > self.last_build:
-                        self.build()
+            for n, _ in enumerate(builds):
+                is_first_build = n == 0
+                self.build(update_source_info_first=is_first_build)
 
 
 def browse_to_address(addr):
     # pylint: disable=import-outside-toplevel
     import webbrowser
 
     def browse():
```

### Comparing `lektor-3.4.0b5/lektor/editor.py` & `lektor-3.4.0b6/lektor/editor.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/exception.py` & `lektor-3.4.0b6/lektor/exception.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/filecontents.py` & `lektor-3.4.0b6/lektor/filecontents.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/i18n.py` & `lektor-3.4.0b6/lektor/i18n.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/metaformat.py` & `lektor-3.4.0b6/lektor/metaformat.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/packages.py` & `lektor-3.4.0b6/lektor/packages.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/pagination.py` & `lektor-3.4.0b6/lektor/pagination.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/pluginsystem.py` & `lektor-3.4.0b6/lektor/pluginsystem.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/project.py` & `lektor-3.4.0b6/lektor/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,20 +104,21 @@
 
     @property
     def project_path(self):
         return self.project_file or self.tree
 
     def get_output_path(self):
         """The path where output files are stored."""
-        config = self.open_config()
+        config = self.open_config()  # raises if no project_file
         output_path = config.get("project.output_path")
         if output_path:
-            return os.path.join(self.tree, os.path.normpath(output_path))
-
-        return os.path.join(get_cache_dir(), "builds", self.id)
+            path = Path(config.filename).parent / output_path
+        else:
+            path = Path(get_cache_dir(), "builds", self.id)
+        return str(path)
 
     class PackageCacheType(Enum):
         VENV = "venv"  # The new virtual environment-based package cache
         FLAT = "flat"  # No longer used flat-directory package cache
 
     def get_package_cache_path(
         self, cache_type: PackageCacheType = PackageCacheType.VENV
```

### Comparing `lektor-3.4.0b5/lektor/publisher.py` & `lektor-3.4.0b6/lektor/publisher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import errno
 import hashlib
 import io
 import os
 import posixpath
+import urllib.parse
 from contextlib import contextmanager
 from contextlib import ExitStack
 from contextlib import suppress
 from ftplib import Error as FTPError
 from inspect import cleandoc
 from pathlib import Path
 from subprocess import CalledProcessError
@@ -23,30 +26,41 @@
 from typing import Iterator
 from typing import Mapping
 from typing import NoReturn
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
+from urllib.parse import urlsplit
 from warnings import warn
 
-from werkzeug import urls
+from werkzeug.datastructures import MultiDict
 
 from lektor.compat import TemporaryDirectory
+from lektor.compat import werkzeug_urls_URL
 from lektor.exception import LektorException
 from lektor.utils import bool_from_string
 from lektor.utils import locate_executable
 from lektor.utils import portable_popen
 
 if TYPE_CHECKING:  # pragma: no cover
     from _typeshed import StrOrBytesPath
     from _typeshed import StrPath
     from lektor.environment import Environment
 
 
+def _parse_query(query: str, **kwargs: Any) -> MultiDict:
+    return MultiDict(urllib.parse.parse_qsl(query, **kwargs))
+
+
+def _ascii_host(host: str) -> str:
+    """Translate internationalized domain name to IDNA-encoded ASCII."""
+    return host.encode("idna").decode("ascii")
+
+
 @contextmanager
 def _ssh_key_file(
     credentials: Optional[Mapping[str, str]]
 ) -> Iterator[Optional["StrPath"]]:
     with ExitStack() as stack:
         key_file: Optional["StrPath"]
         key_file = credentials.get("key_file") if credentials else None
@@ -270,63 +284,69 @@
 
     def fail(self, message: str) -> NoReturn:
         # pylint: disable=no-self-use
         raise PublishError(message)
 
     def publish(
         self,
-        target_url: urls.URL,
+        target_url: str,
         credentials: Optional[Mapping[str, str]] = None,
         **extra: Any,
     ) -> Iterator[str]:
         raise NotImplementedError()
 
 
 class RsyncPublisher(Publisher):
     @contextmanager
     def get_command(self, target_url, credentials):
         credentials = credentials or {}
         argline = ["rsync", "-rclzv", "--exclude=.lektor"]
         target = []
         env = {}
 
-        options = target_url.decode_query()
+        url = urlsplit(target_url)
+        options = _parse_query(url.query, keep_blank_values=True)
         exclude = options.getlist("exclude")
         for file in exclude:
             argline.extend(("--exclude", file))
 
         delete = options.get("delete", False) in ("", "on", "yes", "true", "1", None)
         if delete:
             argline.append("--delete-after")
 
-        with _ssh_command(credentials, target_url.port) as ssh_command:
+        with _ssh_command(credentials, url.port) as ssh_command:
             if ssh_command:
                 argline.extend(("-e", ssh_command))
 
-            username = credentials.get("username") or target_url.username
+            username = credentials.get("username") or url.username
             if username:
                 target.append(username + "@")
 
-            if target_url.ascii_host is not None:
-                target.append(target_url.ascii_host)
+            if url.hostname is not None:
+                target.append(_ascii_host(url.hostname))
                 target.append(":")
-            target.append(target_url.path.rstrip("/") + "/")
+            target.append(url.path.rstrip("/") + "/")
 
             argline.append(self.output_path.rstrip("/\\") + "/")
             argline.append("".join(target))
             yield Command(argline, env=env)
 
     def publish(self, target_url, credentials=None, **extra):
         with self.get_command(target_url, credentials) as client:
             yield from client
 
 
 class FtpConnection:
-    def __init__(self, url, credentials=None):
+    def __init__(self, target_url, credentials=None):
         credentials = credentials or {}
+        url = urlsplit(target_url)
+        if url.hostname is None:
+            raise PublishError(
+                "No host name was specified in the target URL ({target_url})"
+            )
         self.con = self.make_connection()
         self.url = url
         self.username = credentials.get("username") or url.username
         self.password = credentials.get("password") or url.password
         self.log_buffer = []
         self._known_folders = set()
 
@@ -343,20 +363,23 @@
         for chunk in log:
             for line in chunk.splitlines():
                 if not isinstance(line, str):
                     line = line.decode("utf-8", "replace")
                 yield line.rstrip()
 
     def connect(self):
-        options = self.url.decode_query()
+        options = _parse_query(self.url.query, keep_blank_values=True)
+        assert self.url.hostname is not None
+        host = _ascii_host(self.url.hostname)
+        port = self.url.port or 21
 
         log = self.log_buffer
         log.append("000 Connecting to server ...")
         try:
-            log.append(self.con.connect(self.url.ascii_host, self.url.port or 21))
+            log.append(self.con.connect(host, port))
         except Exception as e:
             log.append("000 Could not connect.")
             log.append(str(e))
             return False
 
         try:
             credentials = {}
@@ -785,15 +808,15 @@
 
 
 class GithubPagesPublisher(Publisher):
     """Publish to GitHub pages."""
 
     def publish(
         self,
-        target_url: urls.URL,
+        target_url: str,
         credentials: Optional[Mapping[str, str]] = None,
         **extra: Any,
     ) -> Iterator[str]:
         if not locate_executable("git"):
             self.fail("git executable not found; cannot deploy.")
 
         push_url, branch, cname, preserve_history, warnings = self._parse_url(
@@ -807,24 +830,25 @@
             if push_url.startswith("https:"):
                 repo.set_https_credentials(creds)
             else:
                 repo.set_ssh_credentials(creds)
             yield from repo.publish_ghpages(push_url, branch, cname, preserve_history)
 
     def _parse_url(
-        self, target_url: urls.URL
+        self, target_url: str
     ) -> Tuple[str, str, Optional[str], bool, Sequence[str]]:
-        if not target_url.host:
+        url = urlsplit(target_url)
+        if not url.hostname:
             self.fail("github owner missing from target URL")
-        gh_owner = target_url.host.lower()
-        gh_project = target_url.path.strip("/").lower()
+        gh_owner = url.hostname.lower()
+        gh_project = url.path.strip("/").lower()
         if not gh_project:
             self.fail("github project missing from target URL")
 
-        params = target_url.decode_query()
+        params = _parse_query(url.query, keep_blank_values=True)
         cname = params.get("cname")
         branch = params.get("branch")
         preserve_history = bool_from_string(params.get("preserve_history"), True)
 
         warnings = []
 
         if not branch:
@@ -839,21 +863,21 @@
                     # deprecated in version 3.4.0
                     category=DeprecationWarning,
                 )
                 branch = "master"
             else:
                 branch = "gh-pages"
 
-        if target_url.scheme in ("ghpages", "ghpages+ssh"):
+        if url.scheme in ("ghpages", "ghpages+ssh"):
             push_url = f"ssh://git@github.com/{gh_owner}/{gh_project}.git"
             default_port = 22
         else:
             push_url = f"https://github.com/{gh_owner}/{gh_project}.git"
             default_port = 443
-        if target_url.port and target_url.port != default_port:
+        if url.port and url.port != default_port:
             self.fail("github does not support pushing to non-standard ports")
 
         return push_url, branch, cname, preserve_history, warnings
 
     _EXPLICIT_BRANCH_SUGGESTED_MSG = """
     ================================================================
     WARNING!!! You should explicitly set the name of the published
@@ -874,21 +898,22 @@
     deploying to GitHub pages repositories.  In a future version of
     Lektor, the default branch will GitHub's new default, 'main'.
     It is suggested that you explicitly set which branch to push to.
     """
 
     @staticmethod
     def _parse_credentials(
-        credentials: Optional[Mapping[str, str]], target_url: urls.URL
+        credentials: Optional[Mapping[str, str]], target_url: str
     ) -> Mapping[str, str]:
+        url = urlsplit(target_url)
         creds = dict(credentials or {})
         # Fill in default username/password from target url
         for key, default in [
-            ("username", target_url.username),
-            ("password", target_url.password),
+            ("username", url.username),
+            ("password", url.password),
         ]:
             if not creds.get(key) and default:
                 creds[key] = default
         return creds
 
 
 builtin_publishers = {
@@ -898,12 +923,60 @@
     "ghpages": GithubPagesPublisher,
     "ghpages+https": GithubPagesPublisher,
     "ghpages+ssh": GithubPagesPublisher,
 }
 
 
 def publish(env, target, output_path, credentials=None, **extra):
-    url = urls.url_parse(str(target))
+    target_url = _CompatURLStr(target)
+    url = urlsplit(target_url)
     publisher = env.publishers.get(url.scheme)
     if publisher is None:
         raise PublishError('"%s" is an unknown scheme.' % url.scheme)
-    return publisher(env, output_path).publish(url, credentials, **extra)
+    return publisher(env, output_path).publish(target_url, credentials, **extra)
+
+
+class _CompatURLStr(str):
+    """A string that provides some features of the werkzeug.urls.URL split URL class.
+
+    We used to pass a ``werkzeug.urls.URL`` instance as the ``target_url`` argument to
+    the ``Publisher.publish`` method.  Werkzeug has deprecated the ``URL`` class, so
+    now we've changed our API to just pass a ``str`` for ``target_url``.
+
+    There are however, Lektor plugins out in the wild that provide their own custom
+    Publisher classes, and they expect a ``URL`` instance for ``target_url``.
+
+    Here we provide most of the methods and attributes of ``URL`` that might be of use
+    to a publisher, so as to try not to break all those existing plugins.
+
+    .. tip::
+       New plugins may preserve compatibility with older versions of Lektor by
+       first coercing their ``target_url`` parameter to a ``str`` before use.
+       (This works because ``werkzeug.urls.URL.__str__`` returns the reassembled URL.)
+       E.g. using ``urllib.parse.urlsplit`` to parse the URL:
+
+       .. code:: python
+         from urllib.parse import urlsplit
+
+         class CustomPublisher(Publisher):
+             def publish(self, target_url, credentials=None, **extra):
+                 url = urlsplit(str(target_url))
+                 host = url.hostname
+                 ...
+    """
+
+    def __getattr__(self, name: str):
+        if name.startswith("_"):
+            raise AttributeError(name)
+        url = werkzeug_urls_URL(*urlsplit(self))
+        rv = getattr(url, name)
+        warn(
+            "Since Lektor version 3.4, the 'target_url' parameter to the "
+            "'Publisher.publish' method is now a string rather than a "
+            "werkzeug.urls.URL instance.  To ease the transition, some "
+            "methods and attributes of werkzeugs.urls.URL are being emulated, "
+            "however that will not last forever. The plugin should be updated "
+            "to treat 'target_url' as a string.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        return rv
```

### Comparing `lektor-3.4.0b5/lektor/quickstart.py` & `lektor-3.4.0b6/lektor/quickstart.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/reporter.py` & `lektor-3.4.0b6/lektor/reporter.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/sourceobj.py` & `lektor-3.4.0b6/lektor/sourceobj.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 from urllib.parse import parse_qsl
 from urllib.parse import urlsplit
 from weakref import ref as weakref
 
 from lektor.constants import PRIMARY_ALT
 from lektor.context import ignore_url_unaffecting_dependencies
+from lektor.reporter import reporter
 from lektor.utils import is_path_child_of
 from lektor.utils import join_path
 
 
 class SourceObject:
     source_classification = "generic"
 
@@ -148,18 +149,18 @@
         elif hasattr(path, "url_path"):  # e.g. Thumbnail
             assert path.url_path.startswith("/")
             url_path = path.url_path
         elif path[:1] == "!":
             # XXX: error if used with explicit alt?
             if resolve:
                 raise RuntimeError("Resolve=True is incompatible with '!' prefix.")
-            url_path = posixpath.join(self.url_path, path[1:])
+            url_path = _join_url_path(self, path[1:])
         elif resolve is not None and not resolve:
             # XXX: error if used with explicit alt?
-            url_path = posixpath.join(self.url_path, path)
+            url_path = _join_url_path(self, path)
         else:
             with ignore_url_unaffecting_dependencies():
                 return self._resolve_url(
                     path,
                     alt=alt,
                     absolute=absolute,
                     external=external,
@@ -196,23 +197,52 @@
             if target is not None:
                 url_path = target.url_path
                 query = ""
             elif strict:
                 raise RuntimeError(f"Can not resolve link {_url!r}")
             else:
                 # Fall back to interpreting path as (possibly relative) URL path
-                url_path = posixpath.join(self.url_path, url.path)
+                url_path = _join_url_path(self, url.path)
                 query = url.query
 
             result = self.pad.make_url(
                 url_path, absolute=absolute, external=external, base_url=base_url
             )
             resolved = urlsplit(result)._replace(query=query, fragment=url.fragment)
         return resolved.geturl()
 
+    @property
+    def url_content_path(self):
+        """URL path to the directory that contains children of this source object.
+
+        For container types, the record's ``url_content_path`` is often
+        the same as its ``url_path``. The exception to this is when
+        the page's slug contains a dot (".").
+        See https://www.getlektor.com/docs/content/urls/#content-below-dotted-slugs
+
+        The ``url_content_path`` should be ``None`` for attachments and other
+        SourceObject types that can not contain child source objects.
+        """
+        return None
+
+
+def _join_url_path(source, path):
+    """Join possibly relative url path relative to source.url_content_path."""
+    if posixpath.isabs(path):
+        return path
+    content_path = source.url_content_path
+    if content_path is None:
+        # Source is not a container type (e.g. it is an attachment).
+        # Punt and treat path as relative to the source's containing directory.
+        content_path = posixpath.dirname(source.url_path) or "/"
+        reporter.report_generic(
+            f"Suspicious use of relative URL {path!r} from non-container source {source!r}"
+        )
+    return posixpath.join(content_path, path)
+
 
 class DBSourceObject(SourceObject):
     """This is the base class for objects that live in the lektor db.
 
     I.e. this is the type of object returned by pad.get().
 
     """
```

### Comparing `lektor-3.4.0b5/lektor/sourcesearch.py` & `lektor-3.4.0b6/lektor/sourcesearch.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/utils.py` & `lektor-3.4.0b6/lektor/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 import json
 import os
 import posixpath
 import re
 import subprocess
 import sys
 import tempfile
+import threading
 import unicodedata
+import urllib.parse
 import uuid
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
 from functools import lru_cache
 from functools import wraps
 from pathlib import PurePosixPath
 from typing import Any
 from typing import Callable
+from typing import ClassVar
 from typing import Hashable
 from typing import Iterable
 from typing import overload
 from typing import TypeVar
-from urllib.parse import urlsplit
 
 from jinja2 import is_undefined
 from markupsafe import Markup
 from slugify import slugify as _slugify
-from werkzeug import urls
 from werkzeug.http import http_date
-from werkzeug.urls import url_parse
+from werkzeug.urls import iri_to_uri
+from werkzeug.urls import uri_to_iri
 
 
 is_windows = os.name == "nt"
 
 _slash_escape = "\\/" not in json.dumps("/")
 
 _last_num_re = re.compile(r"^(.*)(\d+)(.*?)$")
@@ -57,14 +59,26 @@
 
 
 def _norm_join(a, b):
     return posixpath.normpath(posixpath.join(a, b))
 
 
 def join_path(a, b):
+    """Join two DB-paths.
+
+    It is assumed that both paths are already normalized in that
+    neither contains an extra "." or ".." components, double-slashes,
+    etc.
+    """
+    # NB: This function is really only during URL resolution.  The only
+    # place that references it is lektor.source.SourceObject._resolve_url.
+
+    if posixpath.isabs(b):
+        return b
+
     a_p, a_v = split_virtual_path(a)
     b_p, b_v = split_virtual_path(b)
 
     # Special case: paginations are considered special virtual paths
     # where the parent is the actual parent of the page.  This however
     # is explicitly not done if the path we join with refers to the
     # current path (empty string or dot).
@@ -94,15 +108,15 @@
 
     This strips any query, and/or fragment that may be present in the
     input path.
 
     Raises ValueError if the path contains a _scheme_
     which is neither ``http`` nor ``https``, or a _netloc_.
     """
-    scheme, netloc, path, _, _ = urlsplit(url_path, scheme="http")
+    scheme, netloc, path, _, _ = urllib.parse.urlsplit(url_path, scheme="http")
     if scheme not in ("http", "https"):
         raise ValueError(f"Invalid scheme: {url_path!r}")
     if netloc:
         raise ValueError(f"Invalid netloc: {url_path!r}")
 
     # NB: POSIX allows for two leading slashes in a pathname, so we have to
     # deal with the possiblity of leading double-slash ourself.
@@ -371,33 +385,95 @@
     return rv
 
 
 def tojson_filter(obj, **kwargs):
     return Markup(htmlsafe_json_dump(obj, **kwargs))
 
 
-class Url:
-    def __init__(self, value):
-        self.url = value
-        u = url_parse(value)
-        i = u.to_iri_tuple()
-        self.ascii_url = str(u)
-        self.host = i.host
-        self.ascii_host = u.ascii_host
-        self.port = u.port
-        self.path = i.path
-        self.query = u.query
-        self.anchor = i.fragment
-        self.scheme = u.scheme
+class Url(urllib.parse.SplitResult):
+    """Make various parts of a URL accessible.
+
+    This is the type of the values exposed by Lektor record fields of type "url".
+
+    Since Lektor 3.4.0, this is essentially a `urllib.parse.SplitResult` as obtained by
+    calling `urlsplit` on the URL normalized to an IRI.
+
+    Generally, attributes such as ``netloc``, ``host``, ``path``, ``query``, and
+    ``fragment`` return the IRI (internationalied) versions of those components.
+
+    The URI (ASCII-encoded) version of the URL is available from the `ascii_url`
+    attribute.
+
+    NB: Changed in 3.4.0: The ``query`` attribute used to return the URI
+    (ASCII-encoded) version of the query — I'm not sure why. Now it returns
+    the IRI (internationalized) version of the query.
+
+    """
+
+    def __new__(cls, value: str):
+        # XXX: deprecate use of constructor so that eventually we can make its signature
+        # match that of the SplitResult base class.
+        warnings.warn(
+            DeprecatedWarning(
+                "Url",
+                reason=(
+                    "Direct construction of a Url instance is deprecated. "
+                    "Use the Url.from_string classmethod instead."
+                ),
+                version="3.4.0",
+            )
+        )
+        return cls.from_string(value)
 
-    def __unicode__(self):
+    @classmethod
+    def from_string(cls, value: str) -> Url:
+        """Construct instance from URL string.
+
+        The input URL can be a URI (all ASCII) or an IRI (internationalized).
+        """
+        # The iri_to_uri operation is nominally idempotent — it can be passed either an
+        # IRI or a URI (or something inbetween) and will return a URI.  So to fully
+        # normalize input which can be either an IRI or a URI, first convert to URI,
+        # then to IRI.
+        iri = uri_to_iri(iri_to_uri(value))
+        obj = cls._make(urllib.parse.urlsplit(iri))
+        obj.url = value
+        return obj
+
+    def __str__(self) -> str:
+        """The original un-normalized URL string."""
         return self.url
 
-    def __str__(self):
-        return self.ascii_url
+    @property
+    def ascii_url(self) -> str:
+        """The URL encoded to an all-ASCII URI."""
+        return iri_to_uri(self.geturl())
+
+    @property
+    def ascii_host(self) -> str | None:
+        """The hostname part of the URL IDNA-encoded to ASCII."""
+        return urllib.parse.urlsplit(self.ascii_url).hostname
+
+    @property
+    def host(self) -> str | None:
+        """The IRI (internationalized) version of the hostname.
+
+        This attribute is provided for backwards-compatibility.  New code should use the
+        ``hostname`` attribute instead.
+        """
+        return self.hostname
+
+    @property
+    def anchor(self) -> str:
+        """The IRI (internationalized) version of the "anchor" part of the URL.
+
+        This attribute is provided for backwards-compatibility.  New code should use the
+        ``fragment`` attribute instead.
+        """
+        return self.fragment
 
 
 def is_unsafe_to_delete(path, base):
     a = os.path.abspath(path)
     b = os.path.abspath(base)
     diff = os.path.relpath(a, b)
     first = diff.split(os.path.sep)[0]
@@ -495,25 +571,20 @@
         "/" not in value
         and value.strip() == value
         and value.split() == [value]
         and not value.startswith(".")
     )
 
 
-def secure_url(url):
-    url = urls.url_parse(url)
-    if url.password is not None:
-        url = url.replace(
-            netloc="%s@%s"
-            % (
-                url.username,
-                url.netloc.split("@")[-1],
-            )
-        )
-    return url.to_url()
+def secure_url(url: str) -> str:
+    parts = urllib.parse.urlsplit(url)
+    if parts.password is not None:
+        _, _, host_port = parts.netloc.rpartition("@")
+        parts = parts._replace(netloc=f"{parts.username}@{host_port}")
+    return parts.geturl()
 
 
 def bool_from_string(val, default=None):
     if val in (True, False, 1, 0):
         return bool(val)
     if isinstance(val, str):
         val = val.lower()
@@ -717,14 +788,41 @@
     seen = set()
     for val in seq:
         if val not in seen:
             seen.add(val)
             yield val
 
 
+class RecursionCheck(threading.local):
+    """A context manager that retains a count of how many times it's been entered.
+
+    Example:
+
+        >>> recursion_check = RecursionCheck()
+
+        >>> with recursion_check:
+        ...     assert recursion_check.level == 1
+        ...     with recursion_check as recursion_level:
+        ...         assert recursion_check.level == 2
+        ...         print("depth", recursion_level)
+        ...     assert recursion_check.level == 1
+        ... assert recursion_check.level == 0
+        depth 2
+    """
+
+    level = 0
+
+    def __enter__(self) -> bool:
+        self.level += 1
+        return self.level
+
+    def __exit__(self, _t, _v, _tb) -> None:
+        self.level -= 1
+
+
 class DeprecatedWarning(DeprecationWarning):
     """Warning category issued by our ``deprecated`` decorator."""
 
     def __init__(
         self,
         name: str,
         reason: str | None = None,
@@ -751,27 +849,28 @@
     """A decorator to mark callables as deprecated."""
 
     name: str | None = None
     reason: str | None = None
     version: str | None = None
     stacklevel: int = 1
 
+    _recursion_check: ClassVar = RecursionCheck()
+
     def __call__(self, wrapped: _F) -> _F:
         if not callable(wrapped):
             raise TypeError("do not know how to deprecate {wrapped!r}")
 
         name = self.name or wrapped.__name__
         message = DeprecatedWarning(name, self.reason, self.version)
 
         @wraps(wrapped)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
-            warnings.warn(message, stacklevel=self.stacklevel + 1)
-            with warnings.catch_warnings():
-                # ignore any of our own custom warnings generated by wrapped callable
-                warnings.simplefilter("ignore", category=DeprecatedWarning)
+            with self._recursion_check as recursion_level:
+                if recursion_level == 1:
+                    warnings.warn(message, stacklevel=self.stacklevel + 1)
                 return wrapped(*args, **kwargs)
 
         return wrapper  # type: ignore[return-value]
 
 
 @overload
 def deprecated(
```

### Comparing `lektor-3.4.0b5/lektor/videotools.py` & `lektor-3.4.0b6/lektor/videotools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/context.py` & `lektor-3.4.0b6/lektor/admin/context.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/utils.py` & `lektor-3.4.0b6/lektor/admin/utils.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/webui.py` & `lektor-3.4.0b6/lektor/admin/webui.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/modules/api.py` & `lektor-3.4.0b6/lektor/admin/modules/api.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/modules/dash.py` & `lektor-3.4.0b6/lektor/admin/modules/dash.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/modules/livereload.py` & `lektor-3.4.0b6/lektor/admin/modules/livereload.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/modules/serve.py` & `lektor-3.4.0b6/lektor/admin/modules/serve.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/static/app.css` & `lektor-3.4.0b6/lektor/admin/static/app.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 @charset "UTF-8";
 
 /* node_modules/font-awesome/css/font-awesome.css */
 @font-face {
   font-family: FontAwesome;
-  src: url(./fontawesome-webfont-FMJ3VJ65.eot?v=4.7.0);
+  src: url();
   src:
-    url(./fontawesome-webfont-FMJ3VJ65.eot?#iefix&v=4.7.0) format("embedded-opentype"),
+    url() format("embedded-opentype"),
     url(./fontawesome-webfont-5GKVPAEF.woff2?v=4.7.0) format("woff2"),
-    url(./fontawesome-webfont-Z4ARLA73.woff?v=4.7.0) format("woff"),
-    url(./fontawesome-webfont-RJ6LE7IU.ttf?v=4.7.0) format("truetype"),
-    url(./fontawesome-webfont-3KIJVIEY.svg?v=4.7.0#fontawesomeregular) format("svg");
+    url() format("woff"),
+    url() format("truetype"),
+    url() format("svg");
   font-weight: 400;
   font-style: normal;
 }
 .fa {
   display: inline-block;
   font: 14px/1 FontAwesome;
   font-size: inherit;
@@ -2330,35 +2330,221 @@
   width: auto;
   height: auto;
   margin: 0;
   overflow: visible;
   clip: auto;
 }
 
-/* sass:/home/runner/work/lektor/lektor/frontend/scss/main.scss */
+/* node_modules/@fontsource/roboto-slab/400.css */
 @font-face {
   font-family: Roboto Slab;
   font-style: normal;
-  font-weight: 300;
-  src:
-    local("Roboto Slab Light"),
-    local("RobotoSlab-Light"),
-    url(./roboto-slab-all-300-ZPJL4QTS.woff2) format("woff2"),
-    url(./roboto-slab-all-300-CD7CKZ7B.woff) format("woff");
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0460-052F,
+    U+1C80-1C88,
+    U+20B4,
+    U+2DE0-2DFF,
+    U+A640-A69F,
+    U+FE2E-FE2F;
 }
 @font-face {
   font-family: Roboto Slab;
   font-style: normal;
+  font-display: swap;
   font-weight: 400;
-  src:
-    local("Roboto Slab Regular"),
-    local("RobotoSlab-Regular"),
-    url(./roboto-slab-all-400-26JDMZKQ.woff2) format("woff2"),
-    url(./roboto-slab-all-400-JK3TGTJI.woff) format("woff");
+  src: url(./roboto-slab-cyrillic-400-normal-72U6HY3C.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0301,
+    U+0400-045F,
+    U+0490-0491,
+    U+04B0-04B1,
+    U+2116;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-greek-ext-400-normal-CARBXC53.woff2) format("woff2"), url() format("woff");
+  unicode-range: U+1F00-1FFF;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-greek-400-normal-FZE4RLDU.woff2) format("woff2"), url() format("woff");
+  unicode-range: U+0370-03FF;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0102-0103,
+    U+0110-0111,
+    U+0128-0129,
+    U+0168-0169,
+    U+01A0-01A1,
+    U+01AF-01B0,
+    U+1EA0-1EF9,
+    U+20AB;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-latin-ext-400-normal-66GAUH66.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0100-024F,
+    U+0259,
+    U+1E00-1EFF,
+    U+2020,
+    U+20A0-20AB,
+    U+20AD-20CF,
+    U+2113,
+    U+2C60-2C7F,
+    U+A720-A7FF;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 400;
+  src: url(./roboto-slab-latin-400-normal-WDWDTZK2.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0000-00FF,
+    U+0131,
+    U+0152-0153,
+    U+02BB-02BC,
+    U+02C6,
+    U+02DA,
+    U+02DC,
+    U+2000-206F,
+    U+2074,
+    U+20AC,
+    U+2122,
+    U+2191,
+    U+2193,
+    U+2212,
+    U+2215,
+    U+FEFF,
+    U+FFFD;
+}
+
+/* node_modules/@fontsource/roboto-slab/700.css */
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0460-052F,
+    U+1C80-1C88,
+    U+20B4,
+    U+2DE0-2DFF,
+    U+A640-A69F,
+    U+FE2E-FE2F;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-cyrillic-700-normal-2TPID6WR.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0301,
+    U+0400-045F,
+    U+0490-0491,
+    U+04B0-04B1,
+    U+2116;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-greek-ext-700-normal-MWV52O3F.woff2) format("woff2"), url() format("woff");
+  unicode-range: U+1F00-1FFF;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-greek-700-normal-5YAILM42.woff2) format("woff2"), url() format("woff");
+  unicode-range: U+0370-03FF;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0102-0103,
+    U+0110-0111,
+    U+0128-0129,
+    U+0168-0169,
+    U+01A0-01A1,
+    U+01AF-01B0,
+    U+1EA0-1EF9,
+    U+20AB;
+}
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0100-024F,
+    U+0259,
+    U+1E00-1EFF,
+    U+2020,
+    U+20A0-20AB,
+    U+20AD-20CF,
+    U+2113,
+    U+2C60-2C7F,
+    U+A720-A7FF;
 }
+@font-face {
+  font-family: Roboto Slab;
+  font-style: normal;
+  font-display: swap;
+  font-weight: 700;
+  src: url(./roboto-slab-latin-700-normal-VK4QNPMO.woff2) format("woff2"), url() format("woff");
+  unicode-range:
+    U+0000-00FF,
+    U+0131,
+    U+0152-0153,
+    U+02BB-02BC,
+    U+02C6,
+    U+02DA,
+    U+02DC,
+    U+2000-206F,
+    U+2074,
+    U+20AC,
+    U+2122,
+    U+2191,
+    U+2193,
+    U+2212,
+    U+2215,
+    U+FEFF,
+    U+FFFD;
+}
+
+/* sass:/home/runner/work/lektor/lektor/frontend/scss/main.scss */
 :root {
   --bs-blue: #0d6efd;
   --bs-indigo: #6610f2;
   --bs-purple: #6f42c1;
   --bs-pink: #d63384;
   --bs-red: #dc3545;
   --bs-orange: #fd7e14;
@@ -9276,8 +9462,16 @@
   margin-top: 20px;
 }
 pre.traceback {
   background: #3d3639;
   color: #fff;
   padding: 10px 15px;
 }
+/*! Bundled license information:
+
+font-awesome/css/font-awesome.css:
+  (*!
+   *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
+   *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
+   *)
+*/
 /*# sourceMappingURL=app.css.map */
```

### Comparing `lektor-3.4.0b5/lektor/admin/static/app.js` & `lektor-3.4.0b6/lektor/admin/static/app.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -30,35 +30,57 @@
         for (var prop in source)
             __hasOwnProp.call(source, prop) && exclude.indexOf(prop) < 0 && (target[prop] = source[prop]);
         if (source != null && __getOwnPropSymbols)
             for (var prop of __getOwnPropSymbols(source))
                 exclude.indexOf(prop) < 0 && __propIsEnum.call(source, prop) && (target[prop] = source[prop]);
         return target;
     };
-    var __commonJS = (cb, mod) => function() {
-        return mod || (0, cb[__getOwnPropNames(cb)[0]])((mod = {
+    var __commonJS = (cb, mod2) => function() {
+        return mod2 || (0, cb[__getOwnPropNames(cb)[0]])((mod2 = {
             exports: {}
-        }).exports, mod), mod.exports;
+        }).exports, mod2), mod2.exports;
     };
     var __copyProps = (to, from, except, desc) => {
         if (from && typeof from == "object" || typeof from == "function")
             for (let key of __getOwnPropNames(from))
                 !__hasOwnProp.call(to, key) && key !== except && __defProp(to, key, {
                     get: () => from[key],
                     enumerable: !(desc = __getOwnPropDesc(from, key)) || desc.enumerable
                 });
         return to;
     };
-    var __toESM = (mod, isNodeMode, target) => (target = mod != null ? __create(__getProtoOf(mod)) : {}, __copyProps(
-        isNodeMode || !mod || !mod.__esModule ? __defProp(target, "default", {
-            value: mod,
+    var __toESM = (mod2, isNodeMode, target) => (target = mod2 != null ? __create(__getProtoOf(mod2)) : {}, __copyProps(
+        // If the importer is in node compatibility mode or this is not an ESM
+        // file that has been converted to a CommonJS file using a Babel-
+        // compatible transform (i.e. "__esModule" has not been set), then set
+        // "default" to the CommonJS "module.exports" for node compatibility.
+        isNodeMode || !mod2 || !mod2.__esModule ? __defProp(target, "default", {
+            value: mod2,
             enumerable: !0
         }) : target,
-        mod
+        mod2
     ));
+    var __async = (__this, __arguments, generator) => new Promise((resolve, reject) => {
+        var fulfilled = (value) => {
+                try {
+                    step(generator.next(value));
+                } catch (e) {
+                    reject(e);
+                }
+            },
+            rejected = (value) => {
+                try {
+                    step(generator.throw(value));
+                } catch (e) {
+                    reject(e);
+                }
+            },
+            step = (x) => x.done ? resolve(x.value) : Promise.resolve(x.value).then(fulfilled, rejected);
+        step((generator = generator.apply(__this, __arguments)).next());
+    });
 
     // node_modules/react/cjs/react.production.min.js
     var require_react_production_min = __commonJS({
         "node_modules/react/cjs/react.production.min.js"(exports) {
             "use strict";
             var l = Symbol.for("react.element"),
                 n = Symbol.for("react.portal"),
@@ -7636,269 +7658,375 @@
         }
     });
 
     // js/main.tsx
     var import_react59 = __toESM(require_react()),
         import_client = __toESM(require_client());
 
-    // node_modules/react-router-dom/index.js
-    var import_react2 = __toESM(require_react());
+    // node_modules/react-router-dom/dist/index.js
+    var React2 = __toESM(require_react());
 
-    // node_modules/@babel/runtime/helpers/esm/extends.js
+    // node_modules/@remix-run/router/dist/router.js
     function _extends() {
         return _extends = Object.assign ? Object.assign.bind() : function(target) {
             for (var i = 1; i < arguments.length; i++) {
                 var source = arguments[i];
                 for (var key in source)
                     Object.prototype.hasOwnProperty.call(source, key) && (target[key] = source[key]);
             }
             return target;
         }, _extends.apply(this, arguments);
     }
-
-    // node_modules/history/index.js
     var Action;
     (function(Action2) {
         Action2.Pop = "POP", Action2.Push = "PUSH", Action2.Replace = "REPLACE";
     })(Action || (Action = {}));
-    var readOnly = function(obj) {
-        return obj;
-    };
-    var BeforeUnloadEventType = "beforeunload";
     var PopStateEventType = "popstate";
 
     function createBrowserHistory(options) {
         options === void 0 && (options = {});
-        var _options = options,
-            _options$window = _options.window,
-            window2 = _options$window === void 0 ? document.defaultView : _options$window,
-            globalHistory = window2.history;
-
-        function getIndexAndLocation() {
-            var _window$location = window2.location,
-                pathname = _window$location.pathname,
-                search = _window$location.search,
-                hash = _window$location.hash,
-                state = globalHistory.state || {};
-            return [state.idx, readOnly({
+
+        function createBrowserLocation(window2, globalHistory) {
+            let {
                 pathname,
                 search,
-                hash,
-                state: state.usr || null,
-                key: state.key || "default"
-            })];
+                hash
+            } = window2.location;
+            return createLocation(
+                "", {
+                    pathname,
+                    search,
+                    hash
+                },
+                // state defaults to `null` because `window.history.state` does
+                globalHistory.state && globalHistory.state.usr || null,
+                globalHistory.state && globalHistory.state.key || "default"
+            );
         }
-        var blockedPopTx = null;
 
-        function handlePop() {
-            if (blockedPopTx)
-                blockers.call(blockedPopTx), blockedPopTx = null;
-            else {
-                var nextAction = Action.Pop,
-                    _getIndexAndLocation = getIndexAndLocation(),
-                    nextIndex = _getIndexAndLocation[0],
-                    nextLocation = _getIndexAndLocation[1];
-                if (blockers.length) {
-                    if (nextIndex != null) {
-                        var delta = index - nextIndex;
-                        delta && (blockedPopTx = {
-                            action: nextAction,
-                            location: nextLocation,
-                            retry: function() {
-                                go(delta * -1);
-                            }
-                        }, go(delta));
-                    }
-                } else
-                    applyTx(nextAction);
-            }
+        function createBrowserHref(window2, to) {
+            return typeof to == "string" ? to : createPath(to);
         }
-        window2.addEventListener(PopStateEventType, handlePop);
-        var action = Action.Pop,
-            _getIndexAndLocation2 = getIndexAndLocation(),
-            index = _getIndexAndLocation2[0],
-            location = _getIndexAndLocation2[1],
-            listeners = createEvents(),
-            blockers = createEvents();
-        index == null && (index = 0, globalHistory.replaceState(_extends({}, globalHistory.state, {
+        return getUrlBasedHistory(createBrowserLocation, createBrowserHref, null, options);
+    }
+
+    function invariant(value, message) {
+        if (value === !1 || value === null || typeof value > "u")
+            throw new Error(message);
+    }
+
+    function warning(cond, message) {
+        if (!cond) {
+            typeof console < "u" && console.warn(message);
+            try {
+                throw new Error(message);
+            } catch {}
+        }
+    }
+
+    function createKey() {
+        return Math.random().toString(36).substr(2, 8);
+    }
+
+    function getHistoryState(location, index) {
+        return {
+            usr: location.state,
+            key: location.key,
             idx: index
-        }), ""));
+        };
+    }
 
-        function createHref(to) {
-            return typeof to == "string" ? to : createPath(to);
+    function createLocation(current, to, state, key) {
+        return state === void 0 && (state = null), _extends({
+            pathname: typeof current == "string" ? current : current.pathname,
+            search: "",
+            hash: ""
+        }, typeof to == "string" ? parsePath(to) : to, {
+            state,
+            // TODO: This could be cleaned up.  push/replace should probably just take
+            // full Locations now and avoid the need to run through this flow at all
+            // But that's a pretty big refactor to the current test suite so going to
+            // keep as is for the time being and just let any incoming keys take precedence
+            key: to && to.key || key || createKey()
+        });
+    }
+
+    function createPath(_ref) {
+        let {
+            pathname = "/",
+                search = "",
+                hash = ""
+        } = _ref;
+        return search && search !== "?" && (pathname += search.charAt(0) === "?" ? search : "?" + search), hash && hash !== "#" && (pathname += hash.charAt(0) === "#" ? hash : "#" + hash), pathname;
+    }
+
+    function parsePath(path) {
+        let parsedPath = {};
+        if (path) {
+            let hashIndex = path.indexOf("#");
+            hashIndex >= 0 && (parsedPath.hash = path.substr(hashIndex), path = path.substr(0, hashIndex));
+            let searchIndex = path.indexOf("?");
+            searchIndex >= 0 && (parsedPath.search = path.substr(searchIndex), path = path.substr(0, searchIndex)), path && (parsedPath.pathname = path);
         }
+        return parsedPath;
+    }
 
-        function getNextLocation(to, state) {
-            return state === void 0 && (state = null), readOnly(_extends({
-                pathname: location.pathname,
-                hash: "",
-                search: ""
-            }, typeof to == "string" ? parsePath(to) : to, {
-                state,
-                key: createKey()
-            }));
+    function getUrlBasedHistory(getLocation, createHref, validateLocation, options) {
+        options === void 0 && (options = {});
+        let {
+            window: window2 = document.defaultView,
+            v5Compat = !1
+        } = options, globalHistory = window2.history, action = Action.Pop, listener = null, index = getIndex();
+        index == null && (index = 0, globalHistory.replaceState(_extends({}, globalHistory.state, {
+            idx: index
+        }), ""));
+
+        function getIndex() {
+            return (globalHistory.state || {
+                idx: null
+            }).idx;
         }
 
-        function getHistoryStateAndUrl(nextLocation, index2) {
-            return [{
-                usr: nextLocation.state,
-                key: nextLocation.key,
-                idx: index2
-            }, createHref(nextLocation)];
-        }
-
-        function allowTx(action2, location2, retry) {
-            return !blockers.length || (blockers.call({
-                action: action2,
-                location: location2,
-                retry
-            }), !1);
-        }
-
-        function applyTx(nextAction) {
-            action = nextAction;
-            var _getIndexAndLocation3 = getIndexAndLocation();
-            index = _getIndexAndLocation3[0], location = _getIndexAndLocation3[1], listeners.call({
+        function handlePop() {
+            action = Action.Pop;
+            let nextIndex = getIndex(),
+                delta = nextIndex == null ? null : nextIndex - index;
+            index = nextIndex, listener && listener({
                 action,
-                location
+                location: history.location,
+                delta
             });
         }
 
         function push(to, state) {
-            var nextAction = Action.Push,
-                nextLocation = getNextLocation(to, state);
-
-            function retry() {
-                push(to, state);
-            }
-            if (allowTx(nextAction, nextLocation, retry)) {
-                var _getHistoryStateAndUr = getHistoryStateAndUrl(nextLocation, index + 1),
-                    historyState = _getHistoryStateAndUr[0],
-                    url = _getHistoryStateAndUr[1];
-                try {
-                    globalHistory.pushState(historyState, "", url);
-                } catch {
-                    window2.location.assign(url);
-                }
-                applyTx(nextAction);
+            action = Action.Push;
+            let location = createLocation(history.location, to, state);
+            validateLocation && validateLocation(location, to), index = getIndex() + 1;
+            let historyState = getHistoryState(location, index),
+                url = history.createHref(location);
+            try {
+                globalHistory.pushState(historyState, "", url);
+            } catch {
+                window2.location.assign(url);
             }
+            v5Compat && listener && listener({
+                action,
+                location: history.location,
+                delta: 1
+            });
         }
 
         function replace(to, state) {
-            var nextAction = Action.Replace,
-                nextLocation = getNextLocation(to, state);
-
-            function retry() {
-                replace(to, state);
-            }
-            if (allowTx(nextAction, nextLocation, retry)) {
-                var _getHistoryStateAndUr2 = getHistoryStateAndUrl(nextLocation, index),
-                    historyState = _getHistoryStateAndUr2[0],
-                    url = _getHistoryStateAndUr2[1];
-                globalHistory.replaceState(historyState, "", url), applyTx(nextAction);
-            }
+            action = Action.Replace;
+            let location = createLocation(history.location, to, state);
+            validateLocation && validateLocation(location, to), index = getIndex();
+            let historyState = getHistoryState(location, index),
+                url = history.createHref(location);
+            globalHistory.replaceState(historyState, "", url), v5Compat && listener && listener({
+                action,
+                location: history.location,
+                delta: 0
+            });
         }
 
-        function go(delta) {
-            globalHistory.go(delta);
+        function createURL(to) {
+            let base = window2.location.origin !== "null" ? window2.location.origin : window2.location.href,
+                href = typeof to == "string" ? to : createPath(to);
+            return invariant(base, "No window.location.(origin|href) available to create URL for href: " + href), new URL(href, base);
         }
-        var history = {
+        let history = {
             get action() {
                 return action;
             },
             get location() {
-                return location;
+                return getLocation(window2, globalHistory);
+            },
+            listen(fn) {
+                if (listener)
+                    throw new Error("A history only accepts one active listener");
+                return window2.addEventListener(PopStateEventType, handlePop), listener = fn, () => {
+                    window2.removeEventListener(PopStateEventType, handlePop), listener = null;
+                };
+            },
+            createHref(to) {
+                return createHref(window2, to);
+            },
+            createURL,
+            encodeLocation(to) {
+                let url = createURL(to);
+                return {
+                    pathname: url.pathname,
+                    search: url.search,
+                    hash: url.hash
+                };
             },
-            createHref,
             push,
             replace,
-            go,
-            back: function() {
-                go(-1);
-            },
-            forward: function() {
-                go(1);
-            },
-            listen: function(listener) {
-                return listeners.push(listener);
-            },
-            block: function(blocker) {
-                var unblock = blockers.push(blocker);
-                return blockers.length === 1 && window2.addEventListener(BeforeUnloadEventType, promptBeforeUnload),
-                    function() {
-                        unblock(), blockers.length || window2.removeEventListener(BeforeUnloadEventType, promptBeforeUnload);
-                    };
+            go(n) {
+                return globalHistory.go(n);
             }
         };
         return history;
     }
-
-    function promptBeforeUnload(event) {
-        event.preventDefault(), event.returnValue = "";
-    }
-
-    function createEvents() {
-        var handlers = [];
-        return {
-            get length() {
-                return handlers.length;
-            },
-            push: function(fn) {
-                return handlers.push(fn),
-                    function() {
-                        handlers = handlers.filter(function(handler) {
-                            return handler !== fn;
-                        });
-                    };
-            },
-            call: function(arg) {
-                handlers.forEach(function(fn) {
-                    return fn && fn(arg);
+    var ResultType;
+    (function(ResultType2) {
+        ResultType2.data = "data", ResultType2.deferred = "deferred", ResultType2.redirect = "redirect", ResultType2.error = "error";
+    })(ResultType || (ResultType = {}));
+    var immutableRouteKeys = /* @__PURE__ */ new Set(["lazy", "caseSensitive", "path", "id", "index", "children"]);
+
+    function isIndexRoute(route) {
+        return route.index === !0;
+    }
+
+    function convertRoutesToDataRoutes(routes, detectErrorBoundary2, parentPath, manifest) {
+        return parentPath === void 0 && (parentPath = []), manifest === void 0 && (manifest = {}), routes.map((route, index) => {
+            let treePath = [...parentPath, index],
+                id = typeof route.id == "string" ? route.id : treePath.join("-");
+            if (invariant(route.index !== !0 || !route.children, "Cannot specify children on an index route"), invariant(!manifest[id], 'Found a route id collision on id "' + id + `".  Route id's must be globally unique within Data Router usages`), isIndexRoute(route)) {
+                let indexRoute = _extends({}, route, {
+                    hasErrorBoundary: detectErrorBoundary2(route),
+                    id
                 });
+                return manifest[id] = indexRoute, indexRoute;
+            } else {
+                let pathOrLayoutRoute = _extends({}, route, {
+                    id,
+                    hasErrorBoundary: detectErrorBoundary2(route),
+                    children: void 0
+                });
+                return manifest[id] = pathOrLayoutRoute, route.children && (pathOrLayoutRoute.children = convertRoutesToDataRoutes(route.children, detectErrorBoundary2, treePath, manifest)), pathOrLayoutRoute;
             }
-        };
+        });
     }
 
-    function createKey() {
-        return Math.random().toString(36).substr(2, 8);
+    function matchRoutes(routes, locationArg, basename) {
+        basename === void 0 && (basename = "/");
+        let location = typeof locationArg == "string" ? parsePath(locationArg) : locationArg,
+            pathname = stripBasename(location.pathname || "/", basename);
+        if (pathname == null)
+            return null;
+        let branches = flattenRoutes(routes);
+        rankRouteBranches(branches);
+        let matches = null;
+        for (let i = 0; matches == null && i < branches.length; ++i)
+            matches = matchRouteBranch(
+                branches[i],
+                // Incoming pathnames are generally encoded from either window.location
+                // or from router.navigate, but we want to match against the unencoded
+                // paths in the route definitions.  Memory router locations won't be
+                // encoded here but there also shouldn't be anything to decode so this
+                // should be a safe operation.  This avoids needing matchRoutes to be
+                // history-aware.
+                safelyDecodeURI(pathname)
+            );
+        return matches;
     }
 
-    function createPath(_ref) {
-        var _ref$pathname = _ref.pathname,
-            pathname = _ref$pathname === void 0 ? "/" : _ref$pathname,
-            _ref$search = _ref.search,
-            search = _ref$search === void 0 ? "" : _ref$search,
-            _ref$hash = _ref.hash,
-            hash = _ref$hash === void 0 ? "" : _ref$hash;
-        return search && search !== "?" && (pathname += search.charAt(0) === "?" ? search : "?" + search), hash && hash !== "#" && (pathname += hash.charAt(0) === "#" ? hash : "#" + hash), pathname;
+    function flattenRoutes(routes, branches, parentsMeta, parentPath) {
+        branches === void 0 && (branches = []), parentsMeta === void 0 && (parentsMeta = []), parentPath === void 0 && (parentPath = "");
+        let flattenRoute = (route, index, relativePath) => {
+            let meta = {
+                relativePath: relativePath === void 0 ? route.path || "" : relativePath,
+                caseSensitive: route.caseSensitive === !0,
+                childrenIndex: index,
+                route
+            };
+            meta.relativePath.startsWith("/") && (invariant(meta.relativePath.startsWith(parentPath), 'Absolute route path "' + meta.relativePath + '" nested under path ' + ('"' + parentPath + '" is not valid. An absolute child route path ') + "must start with the combined path of all its parent routes."), meta.relativePath = meta.relativePath.slice(parentPath.length));
+            let path = joinPaths([parentPath, meta.relativePath]),
+                routesMeta = parentsMeta.concat(meta);
+            route.children && route.children.length > 0 && (invariant(
+                // Our types know better, but runtime JS may not!
+                // @ts-expect-error
+                route.index !== !0,
+                "Index routes must not have child routes. Please remove " + ('all child routes from route path "' + path + '".')
+            ), flattenRoutes(route.children, branches, routesMeta, path)), !(route.path == null && !route.index) && branches.push({
+                path,
+                score: computeScore(path, route.index),
+                routesMeta
+            });
+        };
+        return routes.forEach((route, index) => {
+            var _route$path;
+            if (route.path === "" || !((_route$path = route.path) != null && _route$path.includes("?")))
+                flattenRoute(route, index);
+            else
+                for (let exploded of explodeOptionalSegments(route.path))
+                    flattenRoute(route, index, exploded);
+        }), branches;
+    }
+
+    function explodeOptionalSegments(path) {
+        let segments = path.split("/");
+        if (segments.length === 0)
+            return [];
+        let [first, ...rest] = segments, isOptional = first.endsWith("?"), required = first.replace(/\?$/, "");
+        if (rest.length === 0)
+            return isOptional ? [required, ""] : [required];
+        let restExploded = explodeOptionalSegments(rest.join("/")),
+            result = [];
+        return result.push(...restExploded.map((subpath) => subpath === "" ? required : [required, subpath].join("/"))), isOptional && result.push(...restExploded), result.map((exploded) => path.startsWith("/") && exploded === "" ? "/" : exploded);
+    }
+
+    function rankRouteBranches(branches) {
+        branches.sort((a, b) => a.score !== b.score ? b.score - a.score : compareIndexes(a.routesMeta.map((meta) => meta.childrenIndex), b.routesMeta.map((meta) => meta.childrenIndex)));
+    }
+    var paramRe = /^:\w+$/,
+        dynamicSegmentValue = 3,
+        indexRouteValue = 2,
+        emptySegmentValue = 1,
+        staticSegmentValue = 10,
+        splatPenalty = -2,
+        isSplat = (s) => s === "*";
+
+    function computeScore(path, index) {
+        let segments = path.split("/"),
+            initialScore = segments.length;
+        return segments.some(isSplat) && (initialScore += splatPenalty), index && (initialScore += indexRouteValue), segments.filter((s) => !isSplat(s)).reduce((score, segment) => score + (paramRe.test(segment) ? dynamicSegmentValue : segment === "" ? emptySegmentValue : staticSegmentValue), initialScore);
+    }
+
+    function compareIndexes(a, b) {
+        return a.length === b.length && a.slice(0, -1).every((n, i) => n === b[i]) ? (
+            // If two routes are siblings, we should try to match the earlier sibling
+            // first. This allows people to have fine-grained control over the matching
+            // behavior by simply putting routes with identical paths in the order they
+            // want them tried.
+            a[a.length - 1] - b[b.length - 1]
+        ) : (
+            // Otherwise, it doesn't really make sense to rank non-siblings by index,
+            // so they sort equally.
+            0
+        );
     }
 
-    function parsePath(path) {
-        var parsedPath = {};
-        if (path) {
-            var hashIndex = path.indexOf("#");
-            hashIndex >= 0 && (parsedPath.hash = path.substr(hashIndex), path = path.substr(0, hashIndex));
-            var searchIndex = path.indexOf("?");
-            searchIndex >= 0 && (parsedPath.search = path.substr(searchIndex), path = path.substr(0, searchIndex)), path && (parsedPath.pathname = path);
+    function matchRouteBranch(branch, pathname) {
+        let {
+            routesMeta
+        } = branch, matchedParams = {}, matchedPathname = "/", matches = [];
+        for (let i = 0; i < routesMeta.length; ++i) {
+            let meta = routesMeta[i],
+                end = i === routesMeta.length - 1,
+                remainingPathname = matchedPathname === "/" ? pathname : pathname.slice(matchedPathname.length) || "/",
+                match = matchPath({
+                    path: meta.relativePath,
+                    caseSensitive: meta.caseSensitive,
+                    end
+                }, remainingPathname);
+            if (!match)
+                return null;
+            Object.assign(matchedParams, match.params);
+            let route = meta.route;
+            matches.push({
+                // TODO: Can this as be avoided?
+                params: matchedParams,
+                pathname: joinPaths([matchedPathname, match.pathname]),
+                pathnameBase: normalizePathname(joinPaths([matchedPathname, match.pathnameBase])),
+                route
+            }), match.pathnameBase !== "/" && (matchedPathname = joinPaths([matchedPathname, match.pathnameBase]));
         }
-        return parsedPath;
-    }
-
-    // node_modules/react-router/index.js
-    var import_react = __toESM(require_react());
-    var NavigationContext = /* @__PURE__ */ (0, import_react.createContext)(null),
-        LocationContext = /* @__PURE__ */ (0, import_react.createContext)(null),
-        RouteContext = /* @__PURE__ */ (0, import_react.createContext)({
-            outlet: null,
-            matches: []
-        });
-
-    function invariant(cond, message) {
-        if (!cond)
-            throw new Error(message);
+        return matches;
     }
 
     function matchPath(pattern, pathname) {
         typeof pattern == "string" && (pattern = {
             path: pattern,
             caseSensitive: !1,
             end: !0
@@ -7920,28 +8048,46 @@
             pathname: matchedPathname,
             pathnameBase,
             pattern
         };
     }
 
     function compilePath(path, caseSensitive, end) {
-        caseSensitive === void 0 && (caseSensitive = !1), end === void 0 && (end = !0);
+        caseSensitive === void 0 && (caseSensitive = !1), end === void 0 && (end = !0), warning(path === "*" || !path.endsWith("*") || path.endsWith("/*"), 'Route path "' + path + '" will be treated as if it were ' + ('"' + path.replace(/\*$/, "/*") + '" because the `*` character must ') + "always follow a `/` in the pattern. To get rid of this warning, " + ('please change the route path to "' + path.replace(/\*$/, "/*") + '".'));
         let paramNames = [],
-            regexpSource = "^" + path.replace(/\/*\*?$/, "").replace(/^\/*/, "/").replace(/[\\.*+^$?{}|()[\]]/g, "\\$&").replace(/:(\w+)/g, (_, paramName) => (paramNames.push(paramName), "([^\\/]+)"));
-        return path.endsWith("*") ? (paramNames.push("*"), regexpSource += path === "*" || path === "/*" ? "(.*)$" : "(?:\\/(.+)|\\/*)$") : regexpSource += end ? "\\/*$" : "(?:(?=[.~-]|%[0-9A-F]{2})|\\b|\\/|$)", [new RegExp(regexpSource, caseSensitive ? void 0 : "i"), paramNames];
+            regexpSource = "^" + path.replace(/\/*\*?$/, "").replace(/^\/*/, "/").replace(/[\\.*+^$?{}|()[\]]/g, "\\$&").replace(/\/:(\w+)/g, (_, paramName) => (paramNames.push(paramName), "/([^\\/]+)"));
+        return path.endsWith("*") ? (paramNames.push("*"), regexpSource += path === "*" || path === "/*" ? "(.*)$" : "(?:\\/(.+)|\\/*)$") : end ? regexpSource += "\\/*$" : path !== "" && path !== "/" && (regexpSource += "(?:(?=\\/|$))"), [new RegExp(regexpSource, caseSensitive ? void 0 : "i"), paramNames];
+    }
+
+    function safelyDecodeURI(value) {
+        try {
+            return decodeURI(value);
+        } catch (error) {
+            return warning(!1, 'The URL path "' + value + '" could not be decoded because it is is a malformed URL segment. This is probably due to a bad percent ' + ("encoding (" + error + ").")), value;
+        }
     }
 
     function safelyDecodeURIComponent(value, paramName) {
         try {
             return decodeURIComponent(value);
-        } catch {
-            return value;
+        } catch (error) {
+            return warning(!1, 'The value for the URL param "' + paramName + '" will not be decoded because' + (' the string "' + value + '" is a malformed URL segment. This is probably') + (" due to a bad percent encoding (" + error + ").")), value;
         }
     }
 
+    function stripBasename(pathname, basename) {
+        if (basename === "/")
+            return pathname;
+        if (!pathname.toLowerCase().startsWith(basename.toLowerCase()))
+            return null;
+        let startIndex = basename.endsWith("/") ? basename.length - 1 : basename.length,
+            nextChar = pathname.charAt(startIndex);
+        return nextChar && nextChar !== "/" ? null : pathname.slice(startIndex) || "/";
+    }
+
     function resolvePath(to, fromPathname) {
         fromPathname === void 0 && (fromPathname = "/");
         let {
             pathname: toPathname,
             search = "",
             hash = ""
         } = typeof to == "string" ? parsePath(to) : to;
@@ -7955,304 +8101,2176 @@
     function resolvePathname(relativePath, fromPathname) {
         let segments = fromPathname.replace(/\/+$/, "").split("/");
         return relativePath.split("/").forEach((segment) => {
             segment === ".." ? segments.length > 1 && segments.pop() : segment !== "." && segments.push(segment);
         }), segments.length > 1 ? segments.join("/") : "/";
     }
 
-    function resolveTo(toArg, routePathnames, locationPathname) {
-        let to = typeof toArg == "string" ? parsePath(toArg) : toArg,
-            toPathname = toArg === "" || to.pathname === "" ? "/" : to.pathname,
+    function getInvalidPathError(char, field, dest, path) {
+        return "Cannot include a '" + char + "' character in a manually specified " + ("`to." + field + "` field [" + JSON.stringify(path) + "].  Please separate it out to the ") + ("`to." + dest + "` field. Alternatively you may provide the full path as ") + 'a string in <Link to="..."> and the router will parse it for you.';
+    }
+
+    function getPathContributingMatches(matches) {
+        return matches.filter((match, index) => index === 0 || match.route.path && match.route.path.length > 0);
+    }
+
+    function resolveTo(toArg, routePathnames, locationPathname, isPathRelative) {
+        isPathRelative === void 0 && (isPathRelative = !1);
+        let to;
+        typeof toArg == "string" ? to = parsePath(toArg) : (to = _extends({}, toArg), invariant(!to.pathname || !to.pathname.includes("?"), getInvalidPathError("?", "pathname", "search", to)), invariant(!to.pathname || !to.pathname.includes("#"), getInvalidPathError("#", "pathname", "hash", to)), invariant(!to.search || !to.search.includes("#"), getInvalidPathError("#", "search", "hash", to)));
+        let isEmptyPath = toArg === "" || to.pathname === "",
+            toPathname = isEmptyPath ? "/" : to.pathname,
             from;
-        if (toPathname == null)
+        if (isPathRelative || toPathname == null)
             from = locationPathname;
         else {
             let routePathnameIndex = routePathnames.length - 1;
             if (toPathname.startsWith("..")) {
                 let toSegments = toPathname.split("/");
                 for (; toSegments[0] === "..";)
                     toSegments.shift(), routePathnameIndex -= 1;
                 to.pathname = toSegments.join("/");
             }
             from = routePathnameIndex >= 0 ? routePathnames[routePathnameIndex] : "/";
         }
-        let path = resolvePath(to, from);
-        return toPathname && toPathname !== "/" && toPathname.endsWith("/") && !path.pathname.endsWith("/") && (path.pathname += "/"), path;
+        let path = resolvePath(to, from),
+            hasExplicitTrailingSlash = toPathname && toPathname !== "/" && toPathname.endsWith("/"),
+            hasCurrentTrailingSlash = (isEmptyPath || toPathname === ".") && locationPathname.endsWith("/");
+        return !path.pathname.endsWith("/") && (hasExplicitTrailingSlash || hasCurrentTrailingSlash) && (path.pathname += "/"), path;
     }
+    var joinPaths = (paths) => paths.join("/").replace(/\/\/+/g, "/"),
+        normalizePathname = (pathname) => pathname.replace(/\/+$/, "").replace(/^\/*/, "/"),
+        normalizeSearch = (search) => !search || search === "?" ? "" : search.startsWith("?") ? search : "?" + search,
+        normalizeHash = (hash) => !hash || hash === "#" ? "" : hash.startsWith("#") ? hash : "#" + hash;
+    var ErrorResponse = class {
+        constructor(status, statusText, data, internal) {
+            internal === void 0 && (internal = !1), this.status = status, this.statusText = statusText || "", this.internal = internal, data instanceof Error ? (this.data = data.toString(), this.error = data) : this.data = data;
+        }
+    };
 
-    function getToPathname(to) {
-        return to === "" || to.pathname === "" ? "/" : typeof to == "string" ? parsePath(to).pathname : to.pathname;
+    function isRouteErrorResponse(error) {
+        return error != null && typeof error.status == "number" && typeof error.statusText == "string" && typeof error.internal == "boolean" && "data" in error;
     }
+    var validMutationMethodsArr = ["post", "put", "patch", "delete"],
+        validMutationMethods = new Set(validMutationMethodsArr),
+        validRequestMethodsArr = ["get", ...validMutationMethodsArr],
+        validRequestMethods = new Set(validRequestMethodsArr),
+        redirectStatusCodes = /* @__PURE__ */ new Set([301, 302, 303, 307, 308]),
+        redirectPreserveMethodStatusCodes = /* @__PURE__ */ new Set([307, 308]),
+        IDLE_NAVIGATION = {
+            state: "idle",
+            location: void 0,
+            formMethod: void 0,
+            formAction: void 0,
+            formEncType: void 0,
+            formData: void 0
+        },
+        IDLE_FETCHER = {
+            state: "idle",
+            data: void 0,
+            formMethod: void 0,
+            formAction: void 0,
+            formEncType: void 0,
+            formData: void 0
+        },
+        IDLE_BLOCKER = {
+            state: "unblocked",
+            proceed: void 0,
+            reset: void 0,
+            location: void 0
+        },
+        ABSOLUTE_URL_REGEX = /^(?:[a-z][a-z0-9+.-]*:|\/\/)/i,
+        isBrowser = typeof window < "u" && typeof window.document < "u" && typeof window.document.createElement < "u",
+        isServer = !isBrowser,
+        defaultDetectErrorBoundary = (route) => !!route.hasErrorBoundary;
+
+    function createRouter(init) {
+        invariant(init.routes.length > 0, "You must provide a non-empty routes array to createRouter");
+        let detectErrorBoundary2 = init.detectErrorBoundary || defaultDetectErrorBoundary,
+            manifest = {},
+            dataRoutes = convertRoutesToDataRoutes(init.routes, detectErrorBoundary2, void 0, manifest),
+            inFlightDataRoutes, future = _extends({
+                v7_normalizeFormMethod: !1
+            }, init.future),
+            unlistenHistory = null,
+            subscribers = /* @__PURE__ */ new Set(),
+            savedScrollPositions = null,
+            getScrollRestorationKey = null,
+            getScrollPosition = null,
+            initialScrollRestored = init.hydrationData != null,
+            initialMatches = matchRoutes(dataRoutes, init.history.location, init.basename),
+            initialErrors = null;
+        if (initialMatches == null) {
+            let error = getInternalRouterError(404, {
+                    pathname: init.history.location.pathname
+                }),
+                {
+                    matches,
+                    route
+                } = getShortCircuitMatches(dataRoutes);
+            initialMatches = matches, initialErrors = {
+                [route.id]: error
+            };
+        }
+        let initialized = (
+                // All initialMatches need to be loaded before we're ready.  If we have lazy
+                // functions around still then we'll need to run them in initialize()
+                !initialMatches.some((m) => m.route.lazy) && // And we have to either have no loaders or have been provided hydrationData
+                (!initialMatches.some((m) => m.route.loader) || init.hydrationData != null)
+            ),
+            router, state = {
+                historyAction: init.history.action,
+                location: init.history.location,
+                matches: initialMatches,
+                initialized,
+                navigation: IDLE_NAVIGATION,
+                // Don't restore on initial updateState() if we were SSR'd
+                restoreScrollPosition: init.hydrationData != null ? !1 : null,
+                preventScrollReset: !1,
+                revalidation: "idle",
+                loaderData: init.hydrationData && init.hydrationData.loaderData || {},
+                actionData: init.hydrationData && init.hydrationData.actionData || null,
+                errors: init.hydrationData && init.hydrationData.errors || initialErrors,
+                fetchers: /* @__PURE__ */ new Map(),
+                blockers: /* @__PURE__ */ new Map()
+            },
+            pendingAction = Action.Pop,
+            pendingPreventScrollReset = !1,
+            pendingNavigationController, isUninterruptedRevalidation = !1,
+            isRevalidationRequired = !1,
+            cancelledDeferredRoutes = [],
+            cancelledFetcherLoads = [],
+            fetchControllers = /* @__PURE__ */ new Map(),
+            incrementingLoadId = 0,
+            pendingNavigationLoadId = -1,
+            fetchReloadIds = /* @__PURE__ */ new Map(),
+            fetchRedirectIds = /* @__PURE__ */ new Set(),
+            fetchLoadMatches = /* @__PURE__ */ new Map(),
+            activeDeferreds = /* @__PURE__ */ new Map(),
+            blockerFunctions = /* @__PURE__ */ new Map(),
+            ignoreNextHistoryUpdate = !1;
+
+        function initialize() {
+            return unlistenHistory = init.history.listen((_ref) => {
+                let {
+                    action: historyAction,
+                    location,
+                    delta
+                } = _ref;
+                if (ignoreNextHistoryUpdate) {
+                    ignoreNextHistoryUpdate = !1;
+                    return;
+                }
+                warning(blockerFunctions.size === 0 || delta != null, "You are trying to use a blocker on a POP navigation to a location that was not created by @remix-run/router. This will fail silently in production. This can happen if you are navigating outside the router via `window.history.pushState`/`window.location.hash` instead of using router navigation APIs.  This can also happen if you are using createHashRouter and the user manually changes the URL.");
+                let blockerKey = shouldBlockNavigation({
+                    currentLocation: state.location,
+                    nextLocation: location,
+                    historyAction
+                });
+                if (blockerKey && delta != null) {
+                    ignoreNextHistoryUpdate = !0, init.history.go(delta * -1), updateBlocker(blockerKey, {
+                        state: "blocked",
+                        location,
+                        proceed() {
+                            updateBlocker(blockerKey, {
+                                state: "proceeding",
+                                proceed: void 0,
+                                reset: void 0,
+                                location
+                            }), init.history.go(delta);
+                        },
+                        reset() {
+                            deleteBlocker(blockerKey), updateState({
+                                blockers: new Map(router.state.blockers)
+                            });
+                        }
+                    });
+                    return;
+                }
+                return startNavigation(historyAction, location);
+            }), state.initialized || startNavigation(Action.Pop, state.location), router;
+        }
 
-    function stripBasename(pathname, basename) {
-        if (basename === "/")
-            return pathname;
-        if (!pathname.toLowerCase().startsWith(basename.toLowerCase()))
+        function dispose() {
+            unlistenHistory && unlistenHistory(), subscribers.clear(), pendingNavigationController && pendingNavigationController.abort(), state.fetchers.forEach((_, key) => deleteFetcher(key)), state.blockers.forEach((_, key) => deleteBlocker(key));
+        }
+
+        function subscribe2(fn) {
+            return subscribers.add(fn), () => subscribers.delete(fn);
+        }
+
+        function updateState(newState) {
+            state = _extends({}, state, newState), subscribers.forEach((subscriber) => subscriber(state));
+        }
+
+        function completeNavigation(location, newState) {
+            var _location$state, _location$state2;
+            let isActionReload = state.actionData != null && state.navigation.formMethod != null && isMutationMethod(state.navigation.formMethod) && state.navigation.state === "loading" && ((_location$state = location.state) == null ? void 0 : _location$state._isRedirect) !== !0,
+                actionData;
+            newState.actionData ? Object.keys(newState.actionData).length > 0 ? actionData = newState.actionData : actionData = null : isActionReload ? actionData = state.actionData : actionData = null;
+            let loaderData = newState.loaderData ? mergeLoaderData(state.loaderData, newState.loaderData, newState.matches || [], newState.errors) : state.loaderData;
+            for (let [key] of blockerFunctions)
+                deleteBlocker(key);
+            let preventScrollReset = pendingPreventScrollReset === !0 || state.navigation.formMethod != null && isMutationMethod(state.navigation.formMethod) && ((_location$state2 = location.state) == null ? void 0 : _location$state2._isRedirect) !== !0;
+            inFlightDataRoutes && (dataRoutes = inFlightDataRoutes, inFlightDataRoutes = void 0), updateState(_extends({}, newState, {
+                actionData,
+                loaderData,
+                historyAction: pendingAction,
+                location,
+                initialized: !0,
+                navigation: IDLE_NAVIGATION,
+                revalidation: "idle",
+                restoreScrollPosition: getSavedScrollPosition(location, newState.matches || state.matches),
+                preventScrollReset,
+                blockers: new Map(state.blockers)
+            })), isUninterruptedRevalidation || pendingAction === Action.Pop || (pendingAction === Action.Push ? init.history.push(location, location.state) : pendingAction === Action.Replace && init.history.replace(location, location.state)), pendingAction = Action.Pop, pendingPreventScrollReset = !1, isUninterruptedRevalidation = !1, isRevalidationRequired = !1, cancelledDeferredRoutes = [], cancelledFetcherLoads = [];
+        }
+        async function navigate(to, opts) {
+            if (typeof to == "number") {
+                init.history.go(to);
+                return;
+            }
+            let {
+                path,
+                submission,
+                error
+            } = normalizeNavigateOptions(to, future, opts), currentLocation = state.location, nextLocation = createLocation(state.location, path, opts && opts.state);
+            nextLocation = _extends({}, nextLocation, init.history.encodeLocation(nextLocation));
+            let userReplace = opts && opts.replace != null ? opts.replace : void 0,
+                historyAction = Action.Push;
+            userReplace === !0 ? historyAction = Action.Replace : userReplace === !1 || submission != null && isMutationMethod(submission.formMethod) && submission.formAction === state.location.pathname + state.location.search && (historyAction = Action.Replace);
+            let preventScrollReset = opts && "preventScrollReset" in opts ? opts.preventScrollReset === !0 : void 0,
+                blockerKey = shouldBlockNavigation({
+                    currentLocation,
+                    nextLocation,
+                    historyAction
+                });
+            if (blockerKey) {
+                updateBlocker(blockerKey, {
+                    state: "blocked",
+                    location: nextLocation,
+                    proceed() {
+                        updateBlocker(blockerKey, {
+                            state: "proceeding",
+                            proceed: void 0,
+                            reset: void 0,
+                            location: nextLocation
+                        }), navigate(to, opts);
+                    },
+                    reset() {
+                        deleteBlocker(blockerKey), updateState({
+                            blockers: new Map(state.blockers)
+                        });
+                    }
+                });
+                return;
+            }
+            return await startNavigation(historyAction, nextLocation, {
+                submission,
+                // Send through the formData serialization error if we have one so we can
+                // render at the right error boundary after we match routes
+                pendingError: error,
+                preventScrollReset,
+                replace: opts && opts.replace
+            });
+        }
+
+        function revalidate() {
+            if (interruptActiveLoads(), updateState({
+                    revalidation: "loading"
+                }), state.navigation.state !== "submitting") {
+                if (state.navigation.state === "idle") {
+                    startNavigation(state.historyAction, state.location, {
+                        startUninterruptedRevalidation: !0
+                    });
+                    return;
+                }
+                startNavigation(pendingAction || state.historyAction, state.navigation.location, {
+                    overrideNavigation: state.navigation
+                });
+            }
+        }
+        async function startNavigation(historyAction, location, opts) {
+            pendingNavigationController && pendingNavigationController.abort(), pendingNavigationController = null, pendingAction = historyAction, isUninterruptedRevalidation = (opts && opts.startUninterruptedRevalidation) === !0, saveScrollPosition(state.location, state.matches), pendingPreventScrollReset = (opts && opts.preventScrollReset) === !0;
+            let routesToUse = inFlightDataRoutes || dataRoutes,
+                loadingNavigation = opts && opts.overrideNavigation,
+                matches = matchRoutes(routesToUse, location, init.basename);
+            if (!matches) {
+                let error = getInternalRouterError(404, {
+                        pathname: location.pathname
+                    }),
+                    {
+                        matches: notFoundMatches,
+                        route
+                    } = getShortCircuitMatches(routesToUse);
+                cancelActiveDeferreds(), completeNavigation(location, {
+                    matches: notFoundMatches,
+                    loaderData: {},
+                    errors: {
+                        [route.id]: error
+                    }
+                });
+                return;
+            }
+            if (isHashChangeOnly(state.location, location) && !(opts && opts.submission && isMutationMethod(opts.submission.formMethod))) {
+                completeNavigation(location, {
+                    matches
+                });
+                return;
+            }
+            pendingNavigationController = new AbortController();
+            let request = createClientSideRequest(init.history, location, pendingNavigationController.signal, opts && opts.submission),
+                pendingActionData, pendingError;
+            if (opts && opts.pendingError)
+                pendingError = {
+                    [findNearestBoundary(matches).route.id]: opts.pendingError
+                };
+            else if (opts && opts.submission && isMutationMethod(opts.submission.formMethod)) {
+                let actionOutput = await handleAction(request, location, opts.submission, matches, {
+                    replace: opts.replace
+                });
+                if (actionOutput.shortCircuited)
+                    return;
+                pendingActionData = actionOutput.pendingActionData, pendingError = actionOutput.pendingActionError, loadingNavigation = _extends({
+                    state: "loading",
+                    location
+                }, opts.submission), request = new Request(request.url, {
+                    signal: request.signal
+                });
+            }
+            let {
+                shortCircuited,
+                loaderData,
+                errors
+            } = await handleLoaders(request, location, matches, loadingNavigation, opts && opts.submission, opts && opts.fetcherSubmission, opts && opts.replace, pendingActionData, pendingError);
+            shortCircuited || (pendingNavigationController = null, completeNavigation(location, _extends({
+                matches
+            }, pendingActionData ? {
+                actionData: pendingActionData
+            } : {}, {
+                loaderData,
+                errors
+            })));
+        }
+        async function handleAction(request, location, submission, matches, opts) {
+            interruptActiveLoads();
+            let navigation = _extends({
+                state: "submitting",
+                location
+            }, submission);
+            updateState({
+                navigation
+            });
+            let result, actionMatch = getTargetMatch(matches, location);
+            if (!actionMatch.route.action && !actionMatch.route.lazy)
+                result = {
+                    type: ResultType.error,
+                    error: getInternalRouterError(405, {
+                        method: request.method,
+                        pathname: location.pathname,
+                        routeId: actionMatch.route.id
+                    })
+                };
+            else if (result = await callLoaderOrAction("action", request, actionMatch, matches, manifest, detectErrorBoundary2, router.basename), request.signal.aborted)
+                return {
+                    shortCircuited: !0
+                };
+            if (isRedirectResult(result)) {
+                let replace;
+                return opts && opts.replace != null ? replace = opts.replace : replace = result.location === state.location.pathname + state.location.search, await startRedirectNavigation(state, result, {
+                    submission,
+                    replace
+                }), {
+                    shortCircuited: !0
+                };
+            }
+            if (isErrorResult(result)) {
+                let boundaryMatch = findNearestBoundary(matches, actionMatch.route.id);
+                return (opts && opts.replace) !== !0 && (pendingAction = Action.Push), {
+                    // Send back an empty object we can use to clear out any prior actionData
+                    pendingActionData: {},
+                    pendingActionError: {
+                        [boundaryMatch.route.id]: result.error
+                    }
+                };
+            }
+            if (isDeferredResult(result))
+                throw getInternalRouterError(400, {
+                    type: "defer-action"
+                });
+            return {
+                pendingActionData: {
+                    [actionMatch.route.id]: result.data
+                }
+            };
+        }
+        async function handleLoaders(request, location, matches, overrideNavigation, submission, fetcherSubmission, replace, pendingActionData, pendingError) {
+            let loadingNavigation = overrideNavigation;
+            loadingNavigation || (loadingNavigation = _extends({
+                state: "loading",
+                location,
+                formMethod: void 0,
+                formAction: void 0,
+                formEncType: void 0,
+                formData: void 0
+            }, submission));
+            let activeSubmission = submission || fetcherSubmission ? submission || fetcherSubmission : loadingNavigation.formMethod && loadingNavigation.formAction && loadingNavigation.formData && loadingNavigation.formEncType ? {
+                    formMethod: loadingNavigation.formMethod,
+                    formAction: loadingNavigation.formAction,
+                    formData: loadingNavigation.formData,
+                    formEncType: loadingNavigation.formEncType
+                } : void 0,
+                routesToUse = inFlightDataRoutes || dataRoutes,
+                [matchesToLoad, revalidatingFetchers] = getMatchesToLoad(init.history, state, matches, activeSubmission, location, isRevalidationRequired, cancelledDeferredRoutes, cancelledFetcherLoads, fetchLoadMatches, routesToUse, init.basename, pendingActionData, pendingError);
+            if (cancelActiveDeferreds((routeId) => !(matches && matches.some((m) => m.route.id === routeId)) || matchesToLoad && matchesToLoad.some((m) => m.route.id === routeId)), matchesToLoad.length === 0 && revalidatingFetchers.length === 0)
+                return completeNavigation(location, _extends({
+                    matches,
+                    loaderData: {},
+                    // Commit pending error if we're short circuiting
+                    errors: pendingError || null
+                }, pendingActionData ? {
+                    actionData: pendingActionData
+                } : {})), {
+                    shortCircuited: !0
+                };
+            if (!isUninterruptedRevalidation) {
+                revalidatingFetchers.forEach((rf) => {
+                    let fetcher = state.fetchers.get(rf.key),
+                        revalidatingFetcher = {
+                            state: "loading",
+                            data: fetcher && fetcher.data,
+                            formMethod: void 0,
+                            formAction: void 0,
+                            formEncType: void 0,
+                            formData: void 0,
+                            " _hasFetcherDoneAnything ": !0
+                        };
+                    state.fetchers.set(rf.key, revalidatingFetcher);
+                });
+                let actionData = pendingActionData || state.actionData;
+                updateState(_extends({
+                    navigation: loadingNavigation
+                }, actionData ? Object.keys(actionData).length === 0 ? {
+                    actionData: null
+                } : {
+                    actionData
+                } : {}, revalidatingFetchers.length > 0 ? {
+                    fetchers: new Map(state.fetchers)
+                } : {}));
+            }
+            pendingNavigationLoadId = ++incrementingLoadId, revalidatingFetchers.forEach((rf) => fetchControllers.set(rf.key, pendingNavigationController));
+            let {
+                results,
+                loaderResults,
+                fetcherResults
+            } = await callLoadersAndMaybeResolveData(state.matches, matches, matchesToLoad, revalidatingFetchers, request);
+            if (request.signal.aborted)
+                return {
+                    shortCircuited: !0
+                };
+            revalidatingFetchers.forEach((rf) => fetchControllers.delete(rf.key));
+            let redirect2 = findRedirect(results);
+            if (redirect2)
+                return await startRedirectNavigation(state, redirect2, {
+                    replace
+                }), {
+                    shortCircuited: !0
+                };
+            let {
+                loaderData,
+                errors
+            } = processLoaderData(state, matches, matchesToLoad, loaderResults, pendingError, revalidatingFetchers, fetcherResults, activeDeferreds);
+            activeDeferreds.forEach((deferredData, routeId) => {
+                deferredData.subscribe((aborted) => {
+                    (aborted || deferredData.done) && activeDeferreds.delete(routeId);
+                });
+            }), markFetchRedirectsDone();
+            let didAbortFetchLoads = abortStaleFetchLoads(pendingNavigationLoadId);
+            return _extends({
+                loaderData,
+                errors
+            }, didAbortFetchLoads || revalidatingFetchers.length > 0 ? {
+                fetchers: new Map(state.fetchers)
+            } : {});
+        }
+
+        function getFetcher(key) {
+            return state.fetchers.get(key) || IDLE_FETCHER;
+        }
+
+        function fetch2(key, routeId, href, opts) {
+            if (isServer)
+                throw new Error("router.fetch() was called during the server render, but it shouldn't be. You are likely calling a useFetcher() method in the body of your component. Try moving it to a useEffect or a callback.");
+            fetchControllers.has(key) && abortFetcher(key);
+            let matches = matchRoutes(inFlightDataRoutes || dataRoutes, href, init.basename);
+            if (!matches) {
+                setFetcherError(key, routeId, getInternalRouterError(404, {
+                    pathname: href
+                }));
+                return;
+            }
+            let {
+                path,
+                submission
+            } = normalizeNavigateOptions(href, future, opts, !0), match = getTargetMatch(matches, path);
+            if (pendingPreventScrollReset = (opts && opts.preventScrollReset) === !0, submission && isMutationMethod(submission.formMethod)) {
+                handleFetcherAction(key, routeId, path, match, matches, submission);
+                return;
+            }
+            fetchLoadMatches.set(key, {
+                routeId,
+                path
+            }), handleFetcherLoader(key, routeId, path, match, matches, submission);
+        }
+        async function handleFetcherAction(key, routeId, path, match, requestMatches, submission) {
+            if (interruptActiveLoads(), fetchLoadMatches.delete(key), !match.route.action && !match.route.lazy) {
+                let error = getInternalRouterError(405, {
+                    method: submission.formMethod,
+                    pathname: path,
+                    routeId
+                });
+                setFetcherError(key, routeId, error);
+                return;
+            }
+            let existingFetcher = state.fetchers.get(key),
+                fetcher = _extends({
+                    state: "submitting"
+                }, submission, {
+                    data: existingFetcher && existingFetcher.data,
+                    " _hasFetcherDoneAnything ": !0
+                });
+            state.fetchers.set(key, fetcher), updateState({
+                fetchers: new Map(state.fetchers)
+            });
+            let abortController = new AbortController(),
+                fetchRequest = createClientSideRequest(init.history, path, abortController.signal, submission);
+            fetchControllers.set(key, abortController);
+            let actionResult = await callLoaderOrAction("action", fetchRequest, match, requestMatches, manifest, detectErrorBoundary2, router.basename);
+            if (fetchRequest.signal.aborted) {
+                fetchControllers.get(key) === abortController && fetchControllers.delete(key);
+                return;
+            }
+            if (isRedirectResult(actionResult)) {
+                fetchControllers.delete(key), fetchRedirectIds.add(key);
+                let loadingFetcher = _extends({
+                    state: "loading"
+                }, submission, {
+                    data: void 0,
+                    " _hasFetcherDoneAnything ": !0
+                });
+                return state.fetchers.set(key, loadingFetcher), updateState({
+                    fetchers: new Map(state.fetchers)
+                }), startRedirectNavigation(state, actionResult, {
+                    submission,
+                    isFetchActionRedirect: !0
+                });
+            }
+            if (isErrorResult(actionResult)) {
+                setFetcherError(key, routeId, actionResult.error);
+                return;
+            }
+            if (isDeferredResult(actionResult))
+                throw getInternalRouterError(400, {
+                    type: "defer-action"
+                });
+            let nextLocation = state.navigation.location || state.location,
+                revalidationRequest = createClientSideRequest(init.history, nextLocation, abortController.signal),
+                routesToUse = inFlightDataRoutes || dataRoutes,
+                matches = state.navigation.state !== "idle" ? matchRoutes(routesToUse, state.navigation.location, init.basename) : state.matches;
+            invariant(matches, "Didn't find any matches after fetcher action");
+            let loadId = ++incrementingLoadId;
+            fetchReloadIds.set(key, loadId);
+            let loadFetcher = _extends({
+                state: "loading",
+                data: actionResult.data
+            }, submission, {
+                " _hasFetcherDoneAnything ": !0
+            });
+            state.fetchers.set(key, loadFetcher);
+            let [matchesToLoad, revalidatingFetchers] = getMatchesToLoad(
+                init.history,
+                state,
+                matches,
+                submission,
+                nextLocation,
+                isRevalidationRequired,
+                cancelledDeferredRoutes,
+                cancelledFetcherLoads,
+                fetchLoadMatches,
+                routesToUse,
+                init.basename, {
+                    [match.route.id]: actionResult.data
+                },
+                void 0
+                // No need to send through errors since we short circuit above
+            );
+            revalidatingFetchers.filter((rf) => rf.key !== key).forEach((rf) => {
+                let staleKey = rf.key,
+                    existingFetcher2 = state.fetchers.get(staleKey),
+                    revalidatingFetcher = {
+                        state: "loading",
+                        data: existingFetcher2 && existingFetcher2.data,
+                        formMethod: void 0,
+                        formAction: void 0,
+                        formEncType: void 0,
+                        formData: void 0,
+                        " _hasFetcherDoneAnything ": !0
+                    };
+                state.fetchers.set(staleKey, revalidatingFetcher), fetchControllers.set(staleKey, abortController);
+            }), updateState({
+                fetchers: new Map(state.fetchers)
+            });
+            let {
+                results,
+                loaderResults,
+                fetcherResults
+            } = await callLoadersAndMaybeResolveData(state.matches, matches, matchesToLoad, revalidatingFetchers, revalidationRequest);
+            if (abortController.signal.aborted)
+                return;
+            fetchReloadIds.delete(key), fetchControllers.delete(key), revalidatingFetchers.forEach((r) => fetchControllers.delete(r.key));
+            let redirect2 = findRedirect(results);
+            if (redirect2)
+                return startRedirectNavigation(state, redirect2);
+            let {
+                loaderData,
+                errors
+            } = processLoaderData(state, state.matches, matchesToLoad, loaderResults, void 0, revalidatingFetchers, fetcherResults, activeDeferreds), doneFetcher = {
+                state: "idle",
+                data: actionResult.data,
+                formMethod: void 0,
+                formAction: void 0,
+                formEncType: void 0,
+                formData: void 0,
+                " _hasFetcherDoneAnything ": !0
+            };
+            state.fetchers.set(key, doneFetcher);
+            let didAbortFetchLoads = abortStaleFetchLoads(loadId);
+            state.navigation.state === "loading" && loadId > pendingNavigationLoadId ? (invariant(pendingAction, "Expected pending action"), pendingNavigationController && pendingNavigationController.abort(), completeNavigation(state.navigation.location, {
+                matches,
+                loaderData,
+                errors,
+                fetchers: new Map(state.fetchers)
+            })) : (updateState(_extends({
+                errors,
+                loaderData: mergeLoaderData(state.loaderData, loaderData, matches, errors)
+            }, didAbortFetchLoads ? {
+                fetchers: new Map(state.fetchers)
+            } : {})), isRevalidationRequired = !1);
+        }
+        async function handleFetcherLoader(key, routeId, path, match, matches, submission) {
+            let existingFetcher = state.fetchers.get(key),
+                loadingFetcher = _extends({
+                    state: "loading",
+                    formMethod: void 0,
+                    formAction: void 0,
+                    formEncType: void 0,
+                    formData: void 0
+                }, submission, {
+                    data: existingFetcher && existingFetcher.data,
+                    " _hasFetcherDoneAnything ": !0
+                });
+            state.fetchers.set(key, loadingFetcher), updateState({
+                fetchers: new Map(state.fetchers)
+            });
+            let abortController = new AbortController(),
+                fetchRequest = createClientSideRequest(init.history, path, abortController.signal);
+            fetchControllers.set(key, abortController);
+            let result = await callLoaderOrAction("loader", fetchRequest, match, matches, manifest, detectErrorBoundary2, router.basename);
+            if (isDeferredResult(result) && (result = await resolveDeferredData(result, fetchRequest.signal, !0) || result), fetchControllers.get(key) === abortController && fetchControllers.delete(key), fetchRequest.signal.aborted)
+                return;
+            if (isRedirectResult(result)) {
+                await startRedirectNavigation(state, result);
+                return;
+            }
+            if (isErrorResult(result)) {
+                let boundaryMatch = findNearestBoundary(state.matches, routeId);
+                state.fetchers.delete(key), updateState({
+                    fetchers: new Map(state.fetchers),
+                    errors: {
+                        [boundaryMatch.route.id]: result.error
+                    }
+                });
+                return;
+            }
+            invariant(!isDeferredResult(result), "Unhandled fetcher deferred data");
+            let doneFetcher = {
+                state: "idle",
+                data: result.data,
+                formMethod: void 0,
+                formAction: void 0,
+                formEncType: void 0,
+                formData: void 0,
+                " _hasFetcherDoneAnything ": !0
+            };
+            state.fetchers.set(key, doneFetcher), updateState({
+                fetchers: new Map(state.fetchers)
+            });
+        }
+        async function startRedirectNavigation(state2, redirect2, _temp) {
+            var _window;
+            let {
+                submission,
+                replace,
+                isFetchActionRedirect
+            } = _temp === void 0 ? {} : _temp;
+            redirect2.revalidate && (isRevalidationRequired = !0);
+            let redirectLocation = createLocation(
+                state2.location,
+                redirect2.location,
+                // TODO: This can be removed once we get rid of useTransition in Remix v2
+                _extends({
+                    _isRedirect: !0
+                }, isFetchActionRedirect ? {
+                    _isFetchActionRedirect: !0
+                } : {})
+            );
+            if (invariant(redirectLocation, "Expected a location on the redirect navigation"), ABSOLUTE_URL_REGEX.test(redirect2.location) && isBrowser && typeof((_window = window) == null ? void 0 : _window.location) < "u") {
+                let url = init.history.createURL(redirect2.location),
+                    isDifferentBasename = stripBasename(url.pathname, init.basename || "/") == null;
+                if (window.location.origin !== url.origin || isDifferentBasename) {
+                    replace ? window.location.replace(redirect2.location) : window.location.assign(redirect2.location);
+                    return;
+                }
+            }
+            pendingNavigationController = null;
+            let redirectHistoryAction = replace === !0 ? Action.Replace : Action.Push,
+                {
+                    formMethod,
+                    formAction,
+                    formEncType,
+                    formData
+                } = state2.navigation;
+            !submission && formMethod && formAction && formData && formEncType && (submission = {
+                formMethod,
+                formAction,
+                formEncType,
+                formData
+            }), redirectPreserveMethodStatusCodes.has(redirect2.status) && submission && isMutationMethod(submission.formMethod) ? await startNavigation(redirectHistoryAction, redirectLocation, {
+                submission: _extends({}, submission, {
+                    formAction: redirect2.location
+                }),
+                // Preserve this flag across redirects
+                preventScrollReset: pendingPreventScrollReset
+            }) : isFetchActionRedirect ? await startNavigation(redirectHistoryAction, redirectLocation, {
+                overrideNavigation: {
+                    state: "loading",
+                    location: redirectLocation,
+                    formMethod: void 0,
+                    formAction: void 0,
+                    formEncType: void 0,
+                    formData: void 0
+                },
+                fetcherSubmission: submission,
+                // Preserve this flag across redirects
+                preventScrollReset: pendingPreventScrollReset
+            }) : await startNavigation(redirectHistoryAction, redirectLocation, {
+                overrideNavigation: {
+                    state: "loading",
+                    location: redirectLocation,
+                    formMethod: submission ? submission.formMethod : void 0,
+                    formAction: submission ? submission.formAction : void 0,
+                    formEncType: submission ? submission.formEncType : void 0,
+                    formData: submission ? submission.formData : void 0
+                },
+                // Preserve this flag across redirects
+                preventScrollReset: pendingPreventScrollReset
+            });
+        }
+        async function callLoadersAndMaybeResolveData(currentMatches, matches, matchesToLoad, fetchersToLoad, request) {
+            let results = await Promise.all([...matchesToLoad.map((match) => callLoaderOrAction("loader", request, match, matches, manifest, detectErrorBoundary2, router.basename)), ...fetchersToLoad.map((f) => f.matches && f.match ? callLoaderOrAction("loader", createClientSideRequest(init.history, f.path, request.signal), f.match, f.matches, manifest, detectErrorBoundary2, router.basename) : {
+                    type: ResultType.error,
+                    error: getInternalRouterError(404, {
+                        pathname: f.path
+                    })
+                })]),
+                loaderResults = results.slice(0, matchesToLoad.length),
+                fetcherResults = results.slice(matchesToLoad.length);
+            return await Promise.all([resolveDeferredResults(currentMatches, matchesToLoad, loaderResults, request.signal, !1, state.loaderData), resolveDeferredResults(currentMatches, fetchersToLoad.map((f) => f.match), fetcherResults, request.signal, !0)]), {
+                results,
+                loaderResults,
+                fetcherResults
+            };
+        }
+
+        function interruptActiveLoads() {
+            isRevalidationRequired = !0, cancelledDeferredRoutes.push(...cancelActiveDeferreds()), fetchLoadMatches.forEach((_, key) => {
+                fetchControllers.has(key) && (cancelledFetcherLoads.push(key), abortFetcher(key));
+            });
+        }
+
+        function setFetcherError(key, routeId, error) {
+            let boundaryMatch = findNearestBoundary(state.matches, routeId);
+            deleteFetcher(key), updateState({
+                errors: {
+                    [boundaryMatch.route.id]: error
+                },
+                fetchers: new Map(state.fetchers)
+            });
+        }
+
+        function deleteFetcher(key) {
+            fetchControllers.has(key) && abortFetcher(key), fetchLoadMatches.delete(key), fetchReloadIds.delete(key), fetchRedirectIds.delete(key), state.fetchers.delete(key);
+        }
+
+        function abortFetcher(key) {
+            let controller = fetchControllers.get(key);
+            invariant(controller, "Expected fetch controller: " + key), controller.abort(), fetchControllers.delete(key);
+        }
+
+        function markFetchersDone(keys) {
+            for (let key of keys) {
+                let doneFetcher = {
+                    state: "idle",
+                    data: getFetcher(key).data,
+                    formMethod: void 0,
+                    formAction: void 0,
+                    formEncType: void 0,
+                    formData: void 0,
+                    " _hasFetcherDoneAnything ": !0
+                };
+                state.fetchers.set(key, doneFetcher);
+            }
+        }
+
+        function markFetchRedirectsDone() {
+            let doneKeys = [];
+            for (let key of fetchRedirectIds) {
+                let fetcher = state.fetchers.get(key);
+                invariant(fetcher, "Expected fetcher: " + key), fetcher.state === "loading" && (fetchRedirectIds.delete(key), doneKeys.push(key));
+            }
+            markFetchersDone(doneKeys);
+        }
+
+        function abortStaleFetchLoads(landedId) {
+            let yeetedKeys = [];
+            for (let [key, id] of fetchReloadIds)
+                if (id < landedId) {
+                    let fetcher = state.fetchers.get(key);
+                    invariant(fetcher, "Expected fetcher: " + key), fetcher.state === "loading" && (abortFetcher(key), fetchReloadIds.delete(key), yeetedKeys.push(key));
+                }
+            return markFetchersDone(yeetedKeys), yeetedKeys.length > 0;
+        }
+
+        function getBlocker(key, fn) {
+            let blocker = state.blockers.get(key) || IDLE_BLOCKER;
+            return blockerFunctions.get(key) !== fn && blockerFunctions.set(key, fn), blocker;
+        }
+
+        function deleteBlocker(key) {
+            state.blockers.delete(key), blockerFunctions.delete(key);
+        }
+
+        function updateBlocker(key, newBlocker) {
+            let blocker = state.blockers.get(key) || IDLE_BLOCKER;
+            invariant(blocker.state === "unblocked" && newBlocker.state === "blocked" || blocker.state === "blocked" && newBlocker.state === "blocked" || blocker.state === "blocked" && newBlocker.state === "proceeding" || blocker.state === "blocked" && newBlocker.state === "unblocked" || blocker.state === "proceeding" && newBlocker.state === "unblocked", "Invalid blocker state transition: " + blocker.state + " -> " + newBlocker.state), state.blockers.set(key, newBlocker), updateState({
+                blockers: new Map(state.blockers)
+            });
+        }
+
+        function shouldBlockNavigation(_ref2) {
+            let {
+                currentLocation,
+                nextLocation,
+                historyAction
+            } = _ref2;
+            if (blockerFunctions.size === 0)
+                return;
+            blockerFunctions.size > 1 && warning(!1, "A router only supports one blocker at a time");
+            let entries = Array.from(blockerFunctions.entries()),
+                [blockerKey, blockerFunction] = entries[entries.length - 1],
+                blocker = state.blockers.get(blockerKey);
+            if (!(blocker && blocker.state === "proceeding") && blockerFunction({
+                    currentLocation,
+                    nextLocation,
+                    historyAction
+                }))
+                return blockerKey;
+        }
+
+        function cancelActiveDeferreds(predicate) {
+            let cancelledRouteIds = [];
+            return activeDeferreds.forEach((dfd, routeId) => {
+                (!predicate || predicate(routeId)) && (dfd.cancel(), cancelledRouteIds.push(routeId), activeDeferreds.delete(routeId));
+            }), cancelledRouteIds;
+        }
+
+        function enableScrollRestoration(positions, getPosition, getKey) {
+            if (savedScrollPositions = positions, getScrollPosition = getPosition, getScrollRestorationKey = getKey || ((location) => location.key), !initialScrollRestored && state.navigation === IDLE_NAVIGATION) {
+                initialScrollRestored = !0;
+                let y = getSavedScrollPosition(state.location, state.matches);
+                y != null && updateState({
+                    restoreScrollPosition: y
+                });
+            }
+            return () => {
+                savedScrollPositions = null, getScrollPosition = null, getScrollRestorationKey = null;
+            };
+        }
+
+        function saveScrollPosition(location, matches) {
+            if (savedScrollPositions && getScrollRestorationKey && getScrollPosition) {
+                let userMatches = matches.map((m) => createUseMatchesMatch(m, state.loaderData)),
+                    key = getScrollRestorationKey(location, userMatches) || location.key;
+                savedScrollPositions[key] = getScrollPosition();
+            }
+        }
+
+        function getSavedScrollPosition(location, matches) {
+            if (savedScrollPositions && getScrollRestorationKey && getScrollPosition) {
+                let userMatches = matches.map((m) => createUseMatchesMatch(m, state.loaderData)),
+                    key = getScrollRestorationKey(location, userMatches) || location.key,
+                    y = savedScrollPositions[key];
+                if (typeof y == "number")
+                    return y;
+            }
             return null;
-        let nextChar = pathname.charAt(basename.length);
-        return nextChar && nextChar !== "/" ? null : pathname.slice(basename.length) || "/";
+        }
+
+        function _internalSetRoutes(newRoutes) {
+            inFlightDataRoutes = newRoutes;
+        }
+        return router = {
+            get basename() {
+                return init.basename;
+            },
+            get state() {
+                return state;
+            },
+            get routes() {
+                return dataRoutes;
+            },
+            initialize,
+            subscribe: subscribe2,
+            enableScrollRestoration,
+            navigate,
+            fetch: fetch2,
+            revalidate,
+            // Passthrough to history-aware createHref used by useHref so we get proper
+            // hash-aware URLs in DOM paths
+            createHref: (to) => init.history.createHref(to),
+            encodeLocation: (to) => init.history.encodeLocation(to),
+            getFetcher,
+            deleteFetcher,
+            dispose,
+            getBlocker,
+            deleteBlocker,
+            _internalFetchControllers: fetchControllers,
+            _internalActiveDeferreds: activeDeferreds,
+            // TODO: Remove setRoutes, it's temporary to avoid dealing with
+            // updating the tree while validating the update algorithm.
+            _internalSetRoutes
+        }, router;
+    }
+    var UNSAFE_DEFERRED_SYMBOL = Symbol("deferred");
+
+    function isSubmissionNavigation(opts) {
+        return opts != null && "formData" in opts;
+    }
+
+    function normalizeNavigateOptions(to, future, opts, isFetcher) {
+        isFetcher === void 0 && (isFetcher = !1);
+        let path = typeof to == "string" ? to : createPath(to);
+        if (!opts || !isSubmissionNavigation(opts))
+            return {
+                path
+            };
+        if (opts.formMethod && !isValidMethod(opts.formMethod))
+            return {
+                path,
+                error: getInternalRouterError(405, {
+                    method: opts.formMethod
+                })
+            };
+        let submission;
+        if (opts.formData) {
+            let formMethod = opts.formMethod || "get";
+            if (submission = {
+                    formMethod: future.v7_normalizeFormMethod ? formMethod.toUpperCase() : formMethod.toLowerCase(),
+                    formAction: stripHashFromPath(path),
+                    formEncType: opts && opts.formEncType || "application/x-www-form-urlencoded",
+                    formData: opts.formData
+                }, isMutationMethod(submission.formMethod))
+                return {
+                    path,
+                    submission
+                };
+        }
+        let parsedPath = parsePath(path),
+            searchParams = convertFormDataToSearchParams(opts.formData);
+        return isFetcher && parsedPath.search && hasNakedIndexQuery(parsedPath.search) && searchParams.append("index", ""), parsedPath.search = "?" + searchParams, {
+            path: createPath(parsedPath),
+            submission
+        };
     }
-    var joinPaths = (paths) => paths.join("/").replace(/\/\/+/g, "/"),
-        normalizePathname = (pathname) => pathname.replace(/\/+$/, "").replace(/^\/*/, "/"),
-        normalizeSearch = (search) => !search || search === "?" ? "" : search.startsWith("?") ? search : "?" + search,
-        normalizeHash = (hash) => !hash || hash === "#" ? "" : hash.startsWith("#") ? hash : "#" + hash;
 
-    function useHref(to) {
+    function getLoaderMatchesUntilBoundary(matches, boundaryId) {
+        let boundaryMatches = matches;
+        if (boundaryId) {
+            let index = matches.findIndex((m) => m.route.id === boundaryId);
+            index >= 0 && (boundaryMatches = matches.slice(0, index));
+        }
+        return boundaryMatches;
+    }
+
+    function getMatchesToLoad(history, state, matches, submission, location, isRevalidationRequired, cancelledDeferredRoutes, cancelledFetcherLoads, fetchLoadMatches, routesToUse, basename, pendingActionData, pendingError) {
+        let actionResult = pendingError ? Object.values(pendingError)[0] : pendingActionData ? Object.values(pendingActionData)[0] : void 0,
+            currentUrl = history.createURL(state.location),
+            nextUrl = history.createURL(location),
+            defaultShouldRevalidate = (
+                // Forced revalidation due to submission, useRevalidate, or X-Remix-Revalidate
+                isRevalidationRequired || // Clicked the same link, resubmitted a GET form
+                currentUrl.toString() === nextUrl.toString() || // Search params affect all loaders
+                currentUrl.search !== nextUrl.search
+            ),
+            boundaryId = pendingError ? Object.keys(pendingError)[0] : void 0,
+            navigationMatches = getLoaderMatchesUntilBoundary(matches, boundaryId).filter((match, index) => {
+                if (match.route.lazy)
+                    return !0;
+                if (match.route.loader == null)
+                    return !1;
+                if (isNewLoader(state.loaderData, state.matches[index], match) || cancelledDeferredRoutes.some((id) => id === match.route.id))
+                    return !0;
+                let currentRouteMatch = state.matches[index],
+                    nextRouteMatch = match;
+                return shouldRevalidateLoader(match, _extends({
+                    currentUrl,
+                    currentParams: currentRouteMatch.params,
+                    nextUrl,
+                    nextParams: nextRouteMatch.params
+                }, submission, {
+                    actionResult,
+                    defaultShouldRevalidate: defaultShouldRevalidate || isNewRouteInstance(currentRouteMatch, nextRouteMatch)
+                }));
+            }),
+            revalidatingFetchers = [];
+        return fetchLoadMatches.forEach((f, key) => {
+            if (!matches.some((m) => m.route.id === f.routeId))
+                return;
+            let fetcherMatches = matchRoutes(routesToUse, f.path, basename);
+            if (!fetcherMatches) {
+                revalidatingFetchers.push(_extends({
+                    key
+                }, f, {
+                    matches: null,
+                    match: null
+                }));
+                return;
+            }
+            let fetcherMatch = getTargetMatch(fetcherMatches, f.path);
+            if (cancelledFetcherLoads.includes(key)) {
+                revalidatingFetchers.push(_extends({
+                    key,
+                    matches: fetcherMatches,
+                    match: fetcherMatch
+                }, f));
+                return;
+            }
+            shouldRevalidateLoader(fetcherMatch, _extends({
+                currentUrl,
+                currentParams: state.matches[state.matches.length - 1].params,
+                nextUrl,
+                nextParams: matches[matches.length - 1].params
+            }, submission, {
+                actionResult,
+                defaultShouldRevalidate
+            })) && revalidatingFetchers.push(_extends({
+                key,
+                matches: fetcherMatches,
+                match: fetcherMatch
+            }, f));
+        }), [navigationMatches, revalidatingFetchers];
+    }
+
+    function isNewLoader(currentLoaderData, currentMatch, match) {
+        let isNew = (
+                // [a] -> [a, b]
+                !currentMatch || // [a, b] -> [a, c]
+                match.route.id !== currentMatch.route.id
+            ),
+            isMissingData = currentLoaderData[match.route.id] === void 0;
+        return isNew || isMissingData;
+    }
+
+    function isNewRouteInstance(currentMatch, match) {
+        let currentPath = currentMatch.route.path;
+        return (
+            // param change for this match, /users/123 -> /users/456
+            currentMatch.pathname !== match.pathname || // splat param changed, which is not present in match.path
+            // e.g. /files/images/avatar.jpg -> files/finances.xls
+            currentPath != null && currentPath.endsWith("*") && currentMatch.params["*"] !== match.params["*"]
+        );
+    }
+
+    function shouldRevalidateLoader(loaderMatch, arg) {
+        if (loaderMatch.route.shouldRevalidate) {
+            let routeChoice = loaderMatch.route.shouldRevalidate(arg);
+            if (typeof routeChoice == "boolean")
+                return routeChoice;
+        }
+        return arg.defaultShouldRevalidate;
+    }
+    async function loadLazyRouteModule(route, detectErrorBoundary2, manifest) {
+        if (!route.lazy)
+            return;
+        let lazyRoute = await route.lazy();
+        if (!route.lazy)
+            return;
+        let routeToUpdate = manifest[route.id];
+        invariant(routeToUpdate, "No route found in manifest");
+        let routeUpdates = {};
+        for (let lazyRouteProperty in lazyRoute) {
+            let isPropertyStaticallyDefined = routeToUpdate[lazyRouteProperty] !== void 0 && // This property isn't static since it should always be updated based
+                // on the route updates
+                lazyRouteProperty !== "hasErrorBoundary";
+            warning(!isPropertyStaticallyDefined, 'Route "' + routeToUpdate.id + '" has a static property "' + lazyRouteProperty + '" defined but its lazy function is also returning a value for this property. ' + ('The lazy route property "' + lazyRouteProperty + '" will be ignored.')), !isPropertyStaticallyDefined && !immutableRouteKeys.has(lazyRouteProperty) && (routeUpdates[lazyRouteProperty] = lazyRoute[lazyRouteProperty]);
+        }
+        Object.assign(routeToUpdate, routeUpdates), Object.assign(routeToUpdate, {
+            // To keep things framework agnostic, we use the provided
+            // `detectErrorBoundary` function to set the `hasErrorBoundary` route
+            // property since the logic will differ between frameworks.
+            hasErrorBoundary: detectErrorBoundary2(_extends({}, routeToUpdate)),
+            lazy: void 0
+        });
+    }
+    async function callLoaderOrAction(type, request, match, matches, manifest, detectErrorBoundary2, basename, isStaticRequest, isRouteRequest, requestContext) {
+        basename === void 0 && (basename = "/"), isStaticRequest === void 0 && (isStaticRequest = !1), isRouteRequest === void 0 && (isRouteRequest = !1);
+        let resultType, result, onReject, runHandler = (handler) => {
+            let reject, abortPromise = new Promise((_, r) => reject = r);
+            return onReject = () => reject(), request.signal.addEventListener("abort", onReject), Promise.race([handler({
+                request,
+                params: match.params,
+                context: requestContext
+            }), abortPromise]);
+        };
+        try {
+            let handler = match.route[type];
+            if (match.route.lazy)
+                if (handler)
+                    result = (await Promise.all([runHandler(handler), loadLazyRouteModule(match.route, detectErrorBoundary2, manifest)]))[0];
+                else if (await loadLazyRouteModule(match.route, detectErrorBoundary2, manifest), handler = match.route[type], handler)
+                result = await runHandler(handler);
+            else {
+                if (type === "action")
+                    throw getInternalRouterError(405, {
+                        method: request.method,
+                        pathname: new URL(request.url).pathname,
+                        routeId: match.route.id
+                    });
+                return {
+                    type: ResultType.data,
+                    data: void 0
+                };
+            } else
+                invariant(handler, "Could not find the " + type + ' to run on the "' + match.route.id + '" route'), result = await runHandler(handler);
+            invariant(result !== void 0, "You defined " + (type === "action" ? "an action" : "a loader") + " for route " + ('"' + match.route.id + "\" but didn't return anything from your `" + type + "` ") + "function. Please return a value or `null`.");
+        } catch (e) {
+            resultType = ResultType.error, result = e;
+        } finally {
+            onReject && request.signal.removeEventListener("abort", onReject);
+        }
+        if (isResponse(result)) {
+            let status = result.status;
+            if (redirectStatusCodes.has(status)) {
+                let location = result.headers.get("Location");
+                if (invariant(location, "Redirects returned/thrown from loaders/actions must have a Location header"), ABSOLUTE_URL_REGEX.test(location)) {
+                    if (!isStaticRequest) {
+                        let currentUrl = new URL(request.url),
+                            url = location.startsWith("//") ? new URL(currentUrl.protocol + location) : new URL(location),
+                            isSameBasename = stripBasename(url.pathname, basename) != null;
+                        url.origin === currentUrl.origin && isSameBasename && (location = url.pathname + url.search + url.hash);
+                    }
+                } else {
+                    let activeMatches = matches.slice(0, matches.indexOf(match) + 1),
+                        routePathnames = getPathContributingMatches(activeMatches).map((match2) => match2.pathnameBase),
+                        resolvedLocation = resolveTo(location, routePathnames, new URL(request.url).pathname);
+                    if (invariant(createPath(resolvedLocation), "Unable to resolve redirect location: " + location), basename) {
+                        let path = resolvedLocation.pathname;
+                        resolvedLocation.pathname = path === "/" ? basename : joinPaths([basename, path]);
+                    }
+                    location = createPath(resolvedLocation);
+                }
+                if (isStaticRequest)
+                    throw result.headers.set("Location", location), result;
+                return {
+                    type: ResultType.redirect,
+                    status,
+                    location,
+                    revalidate: result.headers.get("X-Remix-Revalidate") !== null
+                };
+            }
+            if (isRouteRequest)
+                throw {
+                    type: resultType || ResultType.data,
+                    response: result
+                };
+            let data, contentType = result.headers.get("Content-Type");
+            return contentType && /\bapplication\/json\b/.test(contentType) ? data = await result.json() : data = await result.text(), resultType === ResultType.error ? {
+                type: resultType,
+                error: new ErrorResponse(status, result.statusText, data),
+                headers: result.headers
+            } : {
+                type: ResultType.data,
+                data,
+                statusCode: result.status,
+                headers: result.headers
+            };
+        }
+        if (resultType === ResultType.error)
+            return {
+                type: resultType,
+                error: result
+            };
+        if (isDeferredData(result)) {
+            var _result$init, _result$init2;
+            return {
+                type: ResultType.deferred,
+                deferredData: result,
+                statusCode: (_result$init = result.init) == null ? void 0 : _result$init.status,
+                headers: ((_result$init2 = result.init) == null ? void 0 : _result$init2.headers) && new Headers(result.init.headers)
+            };
+        }
+        return {
+            type: ResultType.data,
+            data: result
+        };
+    }
+
+    function createClientSideRequest(history, location, signal, submission) {
+        let url = history.createURL(stripHashFromPath(location)).toString(),
+            init = {
+                signal
+            };
+        if (submission && isMutationMethod(submission.formMethod)) {
+            let {
+                formMethod,
+                formEncType,
+                formData
+            } = submission;
+            init.method = formMethod.toUpperCase(), init.body = formEncType === "application/x-www-form-urlencoded" ? convertFormDataToSearchParams(formData) : formData;
+        }
+        return new Request(url, init);
+    }
+
+    function convertFormDataToSearchParams(formData) {
+        let searchParams = new URLSearchParams();
+        for (let [key, value] of formData.entries())
+            searchParams.append(key, value instanceof File ? value.name : value);
+        return searchParams;
+    }
+
+    function processRouteLoaderData(matches, matchesToLoad, results, pendingError, activeDeferreds) {
+        let loaderData = {},
+            errors = null,
+            statusCode, foundError = !1,
+            loaderHeaders = {};
+        return results.forEach((result, index) => {
+            let id = matchesToLoad[index].route.id;
+            if (invariant(!isRedirectResult(result), "Cannot handle redirect results in processLoaderData"), isErrorResult(result)) {
+                let boundaryMatch = findNearestBoundary(matches, id),
+                    error = result.error;
+                pendingError && (error = Object.values(pendingError)[0], pendingError = void 0), errors = errors || {}, errors[boundaryMatch.route.id] == null && (errors[boundaryMatch.route.id] = error), loaderData[id] = void 0, foundError || (foundError = !0, statusCode = isRouteErrorResponse(result.error) ? result.error.status : 500), result.headers && (loaderHeaders[id] = result.headers);
+            } else
+                isDeferredResult(result) ? (activeDeferreds.set(id, result.deferredData), loaderData[id] = result.deferredData.data) : loaderData[id] = result.data, result.statusCode != null && result.statusCode !== 200 && !foundError && (statusCode = result.statusCode), result.headers && (loaderHeaders[id] = result.headers);
+        }), pendingError && (errors = pendingError, loaderData[Object.keys(pendingError)[0]] = void 0), {
+            loaderData,
+            errors,
+            statusCode: statusCode || 200,
+            loaderHeaders
+        };
+    }
+
+    function processLoaderData(state, matches, matchesToLoad, results, pendingError, revalidatingFetchers, fetcherResults, activeDeferreds) {
+        let {
+            loaderData,
+            errors
+        } = processRouteLoaderData(matches, matchesToLoad, results, pendingError, activeDeferreds);
+        for (let index = 0; index < revalidatingFetchers.length; index++) {
+            let {
+                key,
+                match
+            } = revalidatingFetchers[index];
+            invariant(fetcherResults !== void 0 && fetcherResults[index] !== void 0, "Did not find corresponding fetcher result");
+            let result = fetcherResults[index];
+            if (isErrorResult(result)) {
+                let boundaryMatch = findNearestBoundary(state.matches, match?.route.id);
+                errors && errors[boundaryMatch.route.id] || (errors = _extends({}, errors, {
+                    [boundaryMatch.route.id]: result.error
+                })), state.fetchers.delete(key);
+            } else if (isRedirectResult(result))
+                invariant(!1, "Unhandled fetcher revalidation redirect");
+            else if (isDeferredResult(result))
+                invariant(!1, "Unhandled fetcher deferred data");
+            else {
+                let doneFetcher = {
+                    state: "idle",
+                    data: result.data,
+                    formMethod: void 0,
+                    formAction: void 0,
+                    formEncType: void 0,
+                    formData: void 0,
+                    " _hasFetcherDoneAnything ": !0
+                };
+                state.fetchers.set(key, doneFetcher);
+            }
+        }
+        return {
+            loaderData,
+            errors
+        };
+    }
+
+    function mergeLoaderData(loaderData, newLoaderData, matches, errors) {
+        let mergedLoaderData = _extends({}, newLoaderData);
+        for (let match of matches) {
+            let id = match.route.id;
+            if (newLoaderData.hasOwnProperty(id) ? newLoaderData[id] !== void 0 && (mergedLoaderData[id] = newLoaderData[id]) : loaderData[id] !== void 0 && match.route.loader && (mergedLoaderData[id] = loaderData[id]), errors && errors.hasOwnProperty(id))
+                break;
+        }
+        return mergedLoaderData;
+    }
+
+    function findNearestBoundary(matches, routeId) {
+        return (routeId ? matches.slice(0, matches.findIndex((m) => m.route.id === routeId) + 1) : [...matches]).reverse().find((m) => m.route.hasErrorBoundary === !0) || matches[0];
+    }
+
+    function getShortCircuitMatches(routes) {
+        let route = routes.find((r) => r.index || !r.path || r.path === "/") || {
+            id: "__shim-error-route__"
+        };
+        return {
+            matches: [{
+                params: {},
+                pathname: "",
+                pathnameBase: "",
+                route
+            }],
+            route
+        };
+    }
+
+    function getInternalRouterError(status, _temp4) {
+        let {
+            pathname,
+            routeId,
+            method,
+            type
+        } = _temp4 === void 0 ? {} : _temp4, statusText = "Unknown Server Error", errorMessage = "Unknown @remix-run/router error";
+        return status === 400 ? (statusText = "Bad Request", method && pathname && routeId ? errorMessage = "You made a " + method + ' request to "' + pathname + '" but ' + ('did not provide a `loader` for route "' + routeId + '", ') + "so there is no way to handle the request." : type === "defer-action" && (errorMessage = "defer() is not supported in actions")) : status === 403 ? (statusText = "Forbidden", errorMessage = 'Route "' + routeId + '" does not match URL "' + pathname + '"') : status === 404 ? (statusText = "Not Found", errorMessage = 'No route matches URL "' + pathname + '"') : status === 405 && (statusText = "Method Not Allowed", method && pathname && routeId ? errorMessage = "You made a " + method.toUpperCase() + ' request to "' + pathname + '" but ' + ('did not provide an `action` for route "' + routeId + '", ') + "so there is no way to handle the request." : method && (errorMessage = 'Invalid request method "' + method.toUpperCase() + '"')), new ErrorResponse(status || 500, statusText, new Error(errorMessage), !0);
+    }
+
+    function findRedirect(results) {
+        for (let i = results.length - 1; i >= 0; i--) {
+            let result = results[i];
+            if (isRedirectResult(result))
+                return result;
+        }
+    }
+
+    function stripHashFromPath(path) {
+        let parsedPath = typeof path == "string" ? parsePath(path) : path;
+        return createPath(_extends({}, parsedPath, {
+            hash: ""
+        }));
+    }
+
+    function isHashChangeOnly(a, b) {
+        return a.pathname === b.pathname && a.search === b.search && a.hash !== b.hash;
+    }
+
+    function isDeferredResult(result) {
+        return result.type === ResultType.deferred;
+    }
+
+    function isErrorResult(result) {
+        return result.type === ResultType.error;
+    }
+
+    function isRedirectResult(result) {
+        return (result && result.type) === ResultType.redirect;
+    }
+
+    function isDeferredData(value) {
+        let deferred = value;
+        return deferred && typeof deferred == "object" && typeof deferred.data == "object" && typeof deferred.subscribe == "function" && typeof deferred.cancel == "function" && typeof deferred.resolveData == "function";
+    }
+
+    function isResponse(value) {
+        return value != null && typeof value.status == "number" && typeof value.statusText == "string" && typeof value.headers == "object" && typeof value.body < "u";
+    }
+
+    function isValidMethod(method) {
+        return validRequestMethods.has(method.toLowerCase());
+    }
+
+    function isMutationMethod(method) {
+        return validMutationMethods.has(method.toLowerCase());
+    }
+    async function resolveDeferredResults(currentMatches, matchesToLoad, results, signal, isFetcher, currentLoaderData) {
+        for (let index = 0; index < results.length; index++) {
+            let result = results[index],
+                match = matchesToLoad[index];
+            if (!match)
+                continue;
+            let currentMatch = currentMatches.find((m) => m.route.id === match.route.id),
+                isRevalidatingLoader = currentMatch != null && !isNewRouteInstance(currentMatch, match) && (currentLoaderData && currentLoaderData[match.route.id]) !== void 0;
+            isDeferredResult(result) && (isFetcher || isRevalidatingLoader) && await resolveDeferredData(result, signal, isFetcher).then((result2) => {
+                result2 && (results[index] = result2 || results[index]);
+            });
+        }
+    }
+    async function resolveDeferredData(result, signal, unwrap) {
+        if (unwrap === void 0 && (unwrap = !1), !await result.deferredData.resolveData(signal)) {
+            if (unwrap)
+                try {
+                    return {
+                        type: ResultType.data,
+                        data: result.deferredData.unwrappedData
+                    };
+                } catch (e) {
+                    return {
+                        type: ResultType.error,
+                        error: e
+                    };
+                }
+            return {
+                type: ResultType.data,
+                data: result.deferredData.data
+            };
+        }
+    }
+
+    function hasNakedIndexQuery(search) {
+        return new URLSearchParams(search).getAll("index").some((v) => v === "");
+    }
+
+    function createUseMatchesMatch(match, loaderData) {
+        let {
+            route,
+            pathname,
+            params
+        } = match;
+        return {
+            id: route.id,
+            pathname,
+            params,
+            data: loaderData[route.id],
+            handle: route.handle
+        };
+    }
+
+    function getTargetMatch(matches, location) {
+        let search = typeof location == "string" ? parsePath(location).search : location.search;
+        if (matches[matches.length - 1].route.index && hasNakedIndexQuery(search || ""))
+            return matches[matches.length - 1];
+        let pathMatches = getPathContributingMatches(matches);
+        return pathMatches[pathMatches.length - 1];
+    }
+
+    // node_modules/react-router/dist/index.js
+    var React = __toESM(require_react());
+
+    function isPolyfill(x, y) {
+        return x === y && (x !== 0 || 1 / x === 1 / y) || x !== x && y !== y;
+    }
+    var is = typeof Object.is == "function" ? Object.is : isPolyfill,
+        {
+            useState: useState2,
+            useEffect: useEffect2,
+            useLayoutEffect: useLayoutEffect2,
+            useDebugValue
+        } = React;
+
+    function useSyncExternalStore$2(subscribe2, getSnapshot, getServerSnapshot) {
+        let value = getSnapshot(),
+            [{
+                inst
+            }, forceUpdate] = useState2({
+                inst: {
+                    value,
+                    getSnapshot
+                }
+            });
+        return useLayoutEffect2(() => {
+            inst.value = value, inst.getSnapshot = getSnapshot, checkIfSnapshotChanged(inst) && forceUpdate({
+                inst
+            });
+        }, [subscribe2, value, getSnapshot]), useEffect2(() => (checkIfSnapshotChanged(inst) && forceUpdate({
+            inst
+        }), subscribe2(() => {
+            checkIfSnapshotChanged(inst) && forceUpdate({
+                inst
+            });
+        })), [subscribe2]), useDebugValue(value), value;
+    }
+
+    function checkIfSnapshotChanged(inst) {
+        let latestGetSnapshot = inst.getSnapshot,
+            prevValue = inst.value;
+        try {
+            let nextValue = latestGetSnapshot();
+            return !is(prevValue, nextValue);
+        } catch {
+            return !0;
+        }
+    }
+
+    function useSyncExternalStore$1(subscribe2, getSnapshot, getServerSnapshot) {
+        return getSnapshot();
+    }
+    var canUseDOM = typeof window < "u" && typeof window.document < "u" && typeof window.document.createElement < "u",
+        isServerEnvironment = !canUseDOM,
+        shim = isServerEnvironment ? useSyncExternalStore$1 : useSyncExternalStore$2,
+        useSyncExternalStore = "useSyncExternalStore" in React ? ((module) => module.useSyncExternalStore)(React) : shim,
+        DataRouterContext = /* @__PURE__ */ React.createContext(null),
+        DataRouterStateContext = /* @__PURE__ */ React.createContext(null);
+    var NavigationContext = /* @__PURE__ */ React.createContext(null),
+        LocationContext = /* @__PURE__ */ React.createContext(null),
+        RouteContext = /* @__PURE__ */ React.createContext({
+            outlet: null,
+            matches: []
+        }),
+        RouteErrorContext = /* @__PURE__ */ React.createContext(null);
+
+    function _extends2() {
+        return _extends2 = Object.assign ? Object.assign.bind() : function(target) {
+            for (var i = 1; i < arguments.length; i++) {
+                var source = arguments[i];
+                for (var key in source)
+                    Object.prototype.hasOwnProperty.call(source, key) && (target[key] = source[key]);
+            }
+            return target;
+        }, _extends2.apply(this, arguments);
+    }
+
+    function useHref(to, _temp) {
+        let {
+            relative
+        } = _temp === void 0 ? {} : _temp;
         useInRouterContext() || invariant(!1);
         let {
             basename,
             navigator: navigator2
-        } = (0, import_react.useContext)(NavigationContext), {
+        } = React.useContext(NavigationContext), {
             hash,
             pathname,
             search
-        } = useResolvedPath(to), joinedPathname = pathname;
-        if (basename !== "/") {
-            let toPathname = getToPathname(to),
-                endsWithSlash = toPathname != null && toPathname.endsWith("/");
-            joinedPathname = pathname === "/" ? basename + (endsWithSlash ? "/" : "") : joinPaths([basename, pathname]);
-        }
-        return navigator2.createHref({
+        } = useResolvedPath(to, {
+            relative
+        }), joinedPathname = pathname;
+        return basename !== "/" && (joinedPathname = pathname === "/" ? basename : joinPaths([basename, pathname])), navigator2.createHref({
             pathname: joinedPathname,
             search,
             hash
         });
     }
 
     function useInRouterContext() {
-        return (0, import_react.useContext)(LocationContext) != null;
+        return React.useContext(LocationContext) != null;
     }
 
     function useLocation() {
-        return useInRouterContext() || invariant(!1), (0, import_react.useContext)(LocationContext).location;
+        return useInRouterContext() || invariant(!1), React.useContext(LocationContext).location;
     }
 
     function useMatch(pattern) {
         useInRouterContext() || invariant(!1);
         let {
             pathname
         } = useLocation();
-        return (0, import_react.useMemo)(() => matchPath(pattern, pathname), [pathname, pattern]);
+        return React.useMemo(() => matchPath(pattern, pathname), [pathname, pattern]);
     }
 
     function useNavigate() {
         useInRouterContext() || invariant(!1);
         let {
             basename,
             navigator: navigator2
-        } = (0, import_react.useContext)(NavigationContext), {
+        } = React.useContext(NavigationContext), {
             matches
-        } = (0, import_react.useContext)(RouteContext), {
+        } = React.useContext(RouteContext), {
             pathname: locationPathname
-        } = useLocation(), routePathnamesJson = JSON.stringify(matches.map((match) => match.pathnameBase)), activeRef = (0, import_react.useRef)(!1);
-        return (0, import_react.useEffect)(() => {
+        } = useLocation(), routePathnamesJson = JSON.stringify(getPathContributingMatches(matches).map((match) => match.pathnameBase)), activeRef = React.useRef(!1);
+        return React.useEffect(() => {
             activeRef.current = !0;
-        }), (0, import_react.useCallback)(function(to, options) {
+        }), React.useCallback(function(to, options) {
             if (options === void 0 && (options = {}), !activeRef.current)
                 return;
             if (typeof to == "number") {
                 navigator2.go(to);
                 return;
             }
-            let path = resolveTo(to, JSON.parse(routePathnamesJson), locationPathname);
-            basename !== "/" && (path.pathname = joinPaths([basename, path.pathname])), (options.replace ? navigator2.replace : navigator2.push)(path, options.state);
+            let path = resolveTo(to, JSON.parse(routePathnamesJson), locationPathname, options.relative === "path");
+            basename !== "/" && (path.pathname = path.pathname === "/" ? basename : joinPaths([basename, path.pathname])), (options.replace ? navigator2.replace : navigator2.push)(path, options.state, options);
         }, [basename, navigator2, routePathnamesJson, locationPathname]);
     }
 
-    function useResolvedPath(to) {
+    function useResolvedPath(to, _temp2) {
         let {
+            relative
+        } = _temp2 === void 0 ? {} : _temp2, {
             matches
-        } = (0, import_react.useContext)(RouteContext), {
+        } = React.useContext(RouteContext), {
             pathname: locationPathname
-        } = useLocation(), routePathnamesJson = JSON.stringify(matches.map((match) => match.pathnameBase));
-        return (0, import_react.useMemo)(() => resolveTo(to, JSON.parse(routePathnamesJson), locationPathname), [to, routePathnamesJson, locationPathname]);
+        } = useLocation(), routePathnamesJson = JSON.stringify(getPathContributingMatches(matches).map((match) => match.pathnameBase));
+        return React.useMemo(() => resolveTo(to, JSON.parse(routePathnamesJson), locationPathname, relative === "path"), [to, routePathnamesJson, locationPathname, relative]);
+    }
+
+    function useRoutes(routes, locationArg) {
+        useInRouterContext() || invariant(!1);
+        let {
+            navigator: navigator2
+        } = React.useContext(NavigationContext), dataRouterStateContext = React.useContext(DataRouterStateContext), {
+            matches: parentMatches
+        } = React.useContext(RouteContext), routeMatch = parentMatches[parentMatches.length - 1], parentParams = routeMatch ? routeMatch.params : {}, parentPathname = routeMatch ? routeMatch.pathname : "/", parentPathnameBase = routeMatch ? routeMatch.pathnameBase : "/", parentRoute = routeMatch && routeMatch.route, locationFromContext = useLocation(), location;
+        if (locationArg) {
+            var _parsedLocationArg$pa;
+            let parsedLocationArg = typeof locationArg == "string" ? parsePath(locationArg) : locationArg;
+            parentPathnameBase === "/" || (_parsedLocationArg$pa = parsedLocationArg.pathname) != null && _parsedLocationArg$pa.startsWith(parentPathnameBase) || invariant(!1), location = parsedLocationArg;
+        } else
+            location = locationFromContext;
+        let pathname = location.pathname || "/",
+            remainingPathname = parentPathnameBase === "/" ? pathname : pathname.slice(parentPathnameBase.length) || "/",
+            matches = matchRoutes(routes, {
+                pathname: remainingPathname
+            }),
+            renderedMatches = _renderMatches(matches && matches.map((match) => Object.assign({}, match, {
+                params: Object.assign({}, parentParams, match.params),
+                pathname: joinPaths([
+                    parentPathnameBase,
+                    // Re-encode pathnames that were decoded inside matchRoutes
+                    navigator2.encodeLocation ? navigator2.encodeLocation(match.pathname).pathname : match.pathname
+                ]),
+                pathnameBase: match.pathnameBase === "/" ? parentPathnameBase : joinPaths([
+                    parentPathnameBase,
+                    // Re-encode pathnames that were decoded inside matchRoutes
+                    navigator2.encodeLocation ? navigator2.encodeLocation(match.pathnameBase).pathname : match.pathnameBase
+                ])
+            })), parentMatches, dataRouterStateContext || void 0);
+        return locationArg && renderedMatches ? /* @__PURE__ */ React.createElement(LocationContext.Provider, {
+            value: {
+                location: _extends2({
+                    pathname: "/",
+                    search: "",
+                    hash: "",
+                    state: null,
+                    key: "default"
+                }, location),
+                navigationType: Action.Pop
+            }
+        }, renderedMatches) : renderedMatches;
+    }
+
+    function DefaultErrorComponent() {
+        let error = useRouteError(),
+            message = isRouteErrorResponse(error) ? error.status + " " + error.statusText : error instanceof Error ? error.message : JSON.stringify(error),
+            stack = error instanceof Error ? error.stack : null,
+            lightgrey = "rgba(200,200,200, 0.5)",
+            preStyles = {
+                padding: "0.5rem",
+                backgroundColor: lightgrey
+            },
+            codeStyles = {
+                padding: "2px 4px",
+                backgroundColor: lightgrey
+            };
+        return /* @__PURE__ */ React.createElement(React.Fragment, null, /* @__PURE__ */ React.createElement("h2", null, "Unexpected Application Error!"), /* @__PURE__ */ React.createElement("h3", {
+            style: {
+                fontStyle: "italic"
+            }
+        }, message), stack ? /* @__PURE__ */ React.createElement("pre", {
+            style: preStyles
+        }, stack) : null, null);
+    }
+    var RenderErrorBoundary = class extends React.Component {
+        constructor(props) {
+            super(props), this.state = {
+                location: props.location,
+                error: props.error
+            };
+        }
+        static getDerivedStateFromError(error) {
+            return {
+                error
+            };
+        }
+        static getDerivedStateFromProps(props, state) {
+            return state.location !== props.location ? {
+                error: props.error,
+                location: props.location
+            } : {
+                error: props.error || state.error,
+                location: state.location
+            };
+        }
+        componentDidCatch(error, errorInfo) {
+            console.error("React Router caught the following error during render", error, errorInfo);
+        }
+        render() {
+            return this.state.error ? /* @__PURE__ */ React.createElement(RouteContext.Provider, {
+                value: this.props.routeContext
+            }, /* @__PURE__ */ React.createElement(RouteErrorContext.Provider, {
+                value: this.state.error,
+                children: this.props.component
+            })) : this.props.children;
+        }
+    };
+
+    function RenderedRoute(_ref) {
+        let {
+            routeContext,
+            match,
+            children
+        } = _ref, dataRouterContext = React.useContext(DataRouterContext);
+        return dataRouterContext && dataRouterContext.static && dataRouterContext.staticContext && (match.route.errorElement || match.route.ErrorBoundary) && (dataRouterContext.staticContext._deepestRenderedBoundaryId = match.route.id), /* @__PURE__ */ React.createElement(RouteContext.Provider, {
+            value: routeContext
+        }, children);
+    }
+
+    function _renderMatches(matches, parentMatches, dataRouterState) {
+        if (parentMatches === void 0 && (parentMatches = []), matches == null)
+            if (dataRouterState != null && dataRouterState.errors)
+                matches = dataRouterState.matches;
+            else
+                return null;
+        let renderedMatches = matches,
+            errors = dataRouterState?.errors;
+        if (errors != null) {
+            let errorIndex = renderedMatches.findIndex((m) => m.route.id && errors?.[m.route.id]);
+            errorIndex >= 0 || invariant(!1), renderedMatches = renderedMatches.slice(0, Math.min(renderedMatches.length, errorIndex + 1));
+        }
+        return renderedMatches.reduceRight((outlet, match, index) => {
+            let error = match.route.id ? errors?.[match.route.id] : null,
+                errorElement = null;
+            dataRouterState && (match.route.ErrorBoundary ? errorElement = /* @__PURE__ */ React.createElement(match.route.ErrorBoundary, null) : match.route.errorElement ? errorElement = match.route.errorElement : errorElement = /* @__PURE__ */ React.createElement(DefaultErrorComponent, null));
+            let matches2 = parentMatches.concat(renderedMatches.slice(0, index + 1)),
+                getChildren = () => {
+                    let children = outlet;
+                    return error ? children = errorElement : match.route.Component ? children = /* @__PURE__ */ React.createElement(match.route.Component, null) : match.route.element && (children = match.route.element), /* @__PURE__ */ React.createElement(RenderedRoute, {
+                        match,
+                        routeContext: {
+                            outlet,
+                            matches: matches2
+                        },
+                        children
+                    });
+                };
+            return dataRouterState && (match.route.ErrorBoundary || match.route.errorElement || index === 0) ? /* @__PURE__ */ React.createElement(RenderErrorBoundary, {
+                location: dataRouterState.location,
+                component: errorElement,
+                error,
+                children: getChildren(),
+                routeContext: {
+                    outlet: null,
+                    matches: matches2
+                }
+            }) : getChildren();
+        }, null);
+    }
+    var DataRouterHook;
+    (function(DataRouterHook3) {
+        DataRouterHook3.UseBlocker = "useBlocker", DataRouterHook3.UseRevalidator = "useRevalidator";
+    })(DataRouterHook || (DataRouterHook = {}));
+    var DataRouterStateHook;
+    (function(DataRouterStateHook3) {
+        DataRouterStateHook3.UseBlocker = "useBlocker", DataRouterStateHook3.UseLoaderData = "useLoaderData", DataRouterStateHook3.UseActionData = "useActionData", DataRouterStateHook3.UseRouteError = "useRouteError", DataRouterStateHook3.UseNavigation = "useNavigation", DataRouterStateHook3.UseRouteLoaderData = "useRouteLoaderData", DataRouterStateHook3.UseMatches = "useMatches", DataRouterStateHook3.UseRevalidator = "useRevalidator";
+    })(DataRouterStateHook || (DataRouterStateHook = {}));
+
+    function useDataRouterContext(hookName) {
+        let ctx = React.useContext(DataRouterContext);
+        return ctx || invariant(!1), ctx;
+    }
+
+    function useDataRouterState(hookName) {
+        let state = React.useContext(DataRouterStateContext);
+        return state || invariant(!1), state;
+    }
+
+    function useRouteContext(hookName) {
+        let route = React.useContext(RouteContext);
+        return route || invariant(!1), route;
+    }
+
+    function useCurrentRouteId(hookName) {
+        let route = useRouteContext(hookName),
+            thisRoute = route.matches[route.matches.length - 1];
+        return thisRoute.route.id || invariant(!1), thisRoute.route.id;
+    }
+
+    function useRouteError() {
+        var _state$errors;
+        let error = React.useContext(RouteErrorContext),
+            state = useDataRouterState(DataRouterStateHook.UseRouteError),
+            routeId = useCurrentRouteId(DataRouterStateHook.UseRouteError);
+        return error || ((_state$errors = state.errors) == null ? void 0 : _state$errors[routeId]);
+    }
+    var blockerId = 0;
+
+    function useBlocker(shouldBlock) {
+        let {
+            router
+        } = useDataRouterContext(DataRouterHook.UseBlocker), state = useDataRouterState(DataRouterStateHook.UseBlocker), [blockerKey] = React.useState(() => String(++blockerId)), blockerFunction = React.useCallback((args) => typeof shouldBlock == "function" ? !!shouldBlock(args) : !!shouldBlock, [shouldBlock]), blocker = router.getBlocker(blockerKey, blockerFunction);
+        return React.useEffect(() => () => router.deleteBlocker(blockerKey), [router, blockerKey]), state.blockers.get(blockerKey) || blocker;
     }
 
-    function Navigate(_ref2) {
+    function RouterProvider(_ref) {
+        let {
+            fallbackElement,
+            router
+        } = _ref, getState = React.useCallback(() => router.state, [router]), state = useSyncExternalStore(
+            router.subscribe,
+            getState,
+            // We have to provide this so React@18 doesn't complain during hydration,
+            // but we pass our serialized hydration data into the router so state here
+            // is already synced with what the server saw
+            getState
+        ), navigator2 = React.useMemo(() => ({
+            createHref: router.createHref,
+            encodeLocation: router.encodeLocation,
+            go: (n) => router.navigate(n),
+            push: (to, state2, opts) => router.navigate(to, {
+                state: state2,
+                preventScrollReset: opts?.preventScrollReset
+            }),
+            replace: (to, state2, opts) => router.navigate(to, {
+                replace: !0,
+                state: state2,
+                preventScrollReset: opts?.preventScrollReset
+            })
+        }), [router]), basename = router.basename || "/", dataRouterContext = React.useMemo(() => ({
+            router,
+            navigator: navigator2,
+            static: !1,
+            basename
+        }), [router, navigator2, basename]);
+        return /* @__PURE__ */ React.createElement(React.Fragment, null, /* @__PURE__ */ React.createElement(DataRouterContext.Provider, {
+            value: dataRouterContext
+        }, /* @__PURE__ */ React.createElement(DataRouterStateContext.Provider, {
+            value: state
+        }, /* @__PURE__ */ React.createElement(Router, {
+            basename: router.basename,
+            location: router.state.location,
+            navigationType: router.state.historyAction,
+            navigator: navigator2
+        }, router.state.initialized ? /* @__PURE__ */ React.createElement(Routes, null) : fallbackElement))), null);
+    }
+
+    function Navigate(_ref3) {
         let {
             to,
             replace,
-            state
-        } = _ref2;
+            state,
+            relative
+        } = _ref3;
         useInRouterContext() || invariant(!1);
-        let navigate = useNavigate();
-        return (0, import_react.useEffect)(() => {
-            navigate(to, {
+        let dataRouterState = React.useContext(DataRouterStateContext),
+            navigate = useNavigate();
+        return React.useEffect(() => {
+            dataRouterState && dataRouterState.navigation.state !== "idle" || navigate(to, {
                 replace,
-                state
+                state,
+                relative
             });
         }), null;
     }
 
-    function Router(_ref3) {
+    function Route(_props) {
+        invariant(!1);
+    }
+
+    function Router(_ref4) {
         let {
             basename: basenameProp = "/",
             children = null,
             location: locationProp,
             navigationType = Action.Pop,
             navigator: navigator2,
             static: staticProp = !1
-        } = _ref3;
+        } = _ref4;
         useInRouterContext() && invariant(!1);
-        let basename = normalizePathname(basenameProp),
-            navigationContext = (0, import_react.useMemo)(() => ({
+        let basename = basenameProp.replace(/^\/*/, "/"),
+            navigationContext = React.useMemo(() => ({
                 basename,
                 navigator: navigator2,
                 static: staticProp
             }), [basename, navigator2, staticProp]);
         typeof locationProp == "string" && (locationProp = parsePath(locationProp));
         let {
             pathname = "/",
                 search = "",
                 hash = "",
                 state = null,
                 key = "default"
-        } = locationProp, location = (0, import_react.useMemo)(() => {
+        } = locationProp, locationContext = React.useMemo(() => {
             let trailingPathname = stripBasename(pathname, basename);
             return trailingPathname == null ? null : {
-                pathname: trailingPathname,
-                search,
-                hash,
-                state,
-                key
+                location: {
+                    pathname: trailingPathname,
+                    search,
+                    hash,
+                    state,
+                    key
+                },
+                navigationType
             };
-        }, [basename, pathname, search, hash, state, key]);
-        return location == null ? null : /* @__PURE__ */ (0, import_react.createElement)(NavigationContext.Provider, {
+        }, [basename, pathname, search, hash, state, key, navigationType]);
+        return locationContext == null ? null : /* @__PURE__ */ React.createElement(NavigationContext.Provider, {
             value: navigationContext
-        }, /* @__PURE__ */ (0, import_react.createElement)(LocationContext.Provider, {
+        }, /* @__PURE__ */ React.createElement(LocationContext.Provider, {
             children,
-            value: {
-                location,
-                navigationType
-            }
+            value: locationContext
         }));
     }
 
-    // node_modules/react-router-dom/index.js
-    function _extends2() {
-        return _extends2 = Object.assign || function(target) {
+    function Routes(_ref5) {
+        let {
+            children,
+            location
+        } = _ref5, dataRouterContext = React.useContext(DataRouterContext), routes = dataRouterContext && !children ? dataRouterContext.router.routes : createRoutesFromChildren(children);
+        return useRoutes(routes, location);
+    }
+    var AwaitRenderStatus;
+    (function(AwaitRenderStatus2) {
+        AwaitRenderStatus2[AwaitRenderStatus2.pending = 0] = "pending", AwaitRenderStatus2[AwaitRenderStatus2.success = 1] = "success", AwaitRenderStatus2[AwaitRenderStatus2.error = 2] = "error";
+    })(AwaitRenderStatus || (AwaitRenderStatus = {}));
+    var neverSettledPromise = new Promise(() => {});
+
+    function createRoutesFromChildren(children, parentPath) {
+        parentPath === void 0 && (parentPath = []);
+        let routes = [];
+        return React.Children.forEach(children, (element, index) => {
+            if (! /* @__PURE__ */ React.isValidElement(element))
+                return;
+            let treePath = [...parentPath, index];
+            if (element.type === React.Fragment) {
+                routes.push.apply(routes, createRoutesFromChildren(element.props.children, treePath));
+                return;
+            }
+            element.type !== Route && invariant(!1), !element.props.index || !element.props.children || invariant(!1);
+            let route = {
+                id: element.props.id || treePath.join("-"),
+                caseSensitive: element.props.caseSensitive,
+                element: element.props.element,
+                Component: element.props.Component,
+                index: element.props.index,
+                path: element.props.path,
+                loader: element.props.loader,
+                action: element.props.action,
+                errorElement: element.props.errorElement,
+                ErrorBoundary: element.props.ErrorBoundary,
+                hasErrorBoundary: element.props.ErrorBoundary != null || element.props.errorElement != null,
+                shouldRevalidate: element.props.shouldRevalidate,
+                handle: element.props.handle,
+                lazy: element.props.lazy
+            };
+            element.props.children && (route.children = createRoutesFromChildren(element.props.children, treePath)), routes.push(route);
+        }), routes;
+    }
+
+    function detectErrorBoundary(route) {
+        return !!route.ErrorBoundary || !!route.errorElement;
+    }
+
+    // node_modules/react-router-dom/dist/index.js
+    function _extends3() {
+        return _extends3 = Object.assign ? Object.assign.bind() : function(target) {
             for (var i = 1; i < arguments.length; i++) {
                 var source = arguments[i];
                 for (var key in source)
                     Object.prototype.hasOwnProperty.call(source, key) && (target[key] = source[key]);
             }
             return target;
-        }, _extends2.apply(this, arguments);
+        }, _extends3.apply(this, arguments);
     }
 
     function _objectWithoutPropertiesLoose(source, excluded) {
         if (source == null)
             return {};
         var target = {},
             sourceKeys = Object.keys(source),
             key, i;
         for (i = 0; i < sourceKeys.length; i++)
             key = sourceKeys[i], !(excluded.indexOf(key) >= 0) && (target[key] = source[key]);
         return target;
     }
-    var _excluded = ["onClick", "reloadDocument", "replace", "state", "target", "to"],
-        _excluded2 = ["aria-current", "caseSensitive", "className", "end", "style", "to", "children"];
-
-    function BrowserRouter(_ref) {
-        let {
-            basename,
-            children,
-            window: window2
-        } = _ref, historyRef = (0, import_react2.useRef)();
-        historyRef.current == null && (historyRef.current = createBrowserHistory({
-            window: window2
-        }));
-        let history = historyRef.current,
-            [state, setState] = (0, import_react2.useState)({
-                action: history.action,
-                location: history.location
-            });
-        return (0, import_react2.useLayoutEffect)(() => history.listen(setState), [history]), /* @__PURE__ */ (0, import_react2.createElement)(Router, {
-            basename,
-            children,
-            location: state.location,
-            navigationType: state.action,
-            navigator: history
-        });
-    }
 
     function isModifiedEvent(event) {
         return !!(event.metaKey || event.altKey || event.ctrlKey || event.shiftKey);
     }
-    var Link = /* @__PURE__ */ (0, import_react2.forwardRef)(function(_ref4, ref) {
+
+    function shouldProcessLinkClick(event, target) {
+        return event.button === 0 && // Ignore everything but left clicks
+            (!target || target === "_self") && // Let browser handle "target=_blank" etc.
+            !isModifiedEvent(event);
+    }
+    var _excluded = ["onClick", "relative", "reloadDocument", "replace", "state", "target", "to", "preventScrollReset"],
+        _excluded2 = ["aria-current", "caseSensitive", "className", "end", "style", "to", "children"];
+
+    function createBrowserRouter(routes, opts) {
+        return createRouter({
+            basename: opts?.basename,
+            future: opts?.future,
+            history: createBrowserHistory({
+                window: opts?.window
+            }),
+            hydrationData: opts?.hydrationData || parseHydrationData(),
+            routes,
+            detectErrorBoundary
+        }).initialize();
+    }
+
+    function parseHydrationData() {
+        var _window;
+        let state = (_window = window) == null ? void 0 : _window.__staticRouterHydrationData;
+        return state && state.errors && (state = _extends3({}, state, {
+            errors: deserializeErrors(state.errors)
+        })), state;
+    }
+
+    function deserializeErrors(errors) {
+        if (!errors)
+            return null;
+        let entries = Object.entries(errors),
+            serialized = {};
+        for (let [key, val] of entries)
+            if (val && val.__type === "RouteErrorResponse")
+                serialized[key] = new ErrorResponse(val.status, val.statusText, val.data, val.internal === !0);
+            else if (val && val.__type === "Error") {
+            let error = new Error(val.message);
+            error.stack = "", serialized[key] = error;
+        } else
+            serialized[key] = val;
+        return serialized;
+    }
+    var isBrowser2 = typeof window < "u" && typeof window.document < "u" && typeof window.document.createElement < "u",
+        ABSOLUTE_URL_REGEX2 = /^(?:[a-z][a-z0-9+.-]*:|\/\/)/i,
+        Link = /* @__PURE__ */ React2.forwardRef(function(_ref4, ref) {
             let {
                 onClick,
+                relative,
                 reloadDocument,
-                replace = !1,
-                state,
-                target,
-                to
-            } = _ref4, rest = _objectWithoutPropertiesLoose(_ref4, _excluded), href = useHref(to), internalOnClick = useLinkClickHandler(to, {
                 replace,
                 state,
-                target
-            });
+                target,
+                to,
+                preventScrollReset
+            } = _ref4, rest = _objectWithoutPropertiesLoose(_ref4, _excluded), {
+                basename
+            } = React2.useContext(NavigationContext), absoluteHref, isExternal = !1;
+            if (typeof to == "string" && ABSOLUTE_URL_REGEX2.test(to) && (absoluteHref = to, isBrowser2)) {
+                let currentUrl = new URL(window.location.href),
+                    targetUrl = to.startsWith("//") ? new URL(currentUrl.protocol + to) : new URL(to),
+                    path = stripBasename(targetUrl.pathname, basename);
+                targetUrl.origin === currentUrl.origin && path != null ? to = path + targetUrl.search + targetUrl.hash : isExternal = !0;
+            }
+            let href = useHref(to, {
+                    relative
+                }),
+                internalOnClick = useLinkClickHandler(to, {
+                    replace,
+                    state,
+                    target,
+                    preventScrollReset,
+                    relative
+                });
 
             function handleClick(event) {
-                onClick && onClick(event), !event.defaultPrevented && !reloadDocument && internalOnClick(event);
+                onClick && onClick(event), event.defaultPrevented || internalOnClick(event);
             }
-            return /* @__PURE__ */ (0, import_react2.createElement)("a", _extends2({}, rest, {
-                href,
-                onClick: handleClick,
-                ref,
-                target
-            }));
+            return (
+                // eslint-disable-next-line jsx-a11y/anchor-has-content
+                /* @__PURE__ */
+                React2.createElement("a", _extends3({}, rest, {
+                    href: absoluteHref || href,
+                    onClick: isExternal || reloadDocument ? onClick : handleClick,
+                    ref,
+                    target
+                }))
+            );
         }),
-        NavLink = /* @__PURE__ */ (0, import_react2.forwardRef)(function(_ref5, ref) {
+        NavLink = /* @__PURE__ */ React2.forwardRef(function(_ref5, ref) {
             let {
                 "aria-current": ariaCurrentProp = "page",
                 caseSensitive = !1,
                 className: classNameProp = "",
                 end = !1,
                 style: styleProp,
                 to,
                 children
-            } = _ref5, rest = _objectWithoutPropertiesLoose(_ref5, _excluded2), location = useLocation(), path = useResolvedPath(to), locationPathname = location.pathname, toPathname = path.pathname;
-            caseSensitive || (locationPathname = locationPathname.toLowerCase(), toPathname = toPathname.toLowerCase());
+            } = _ref5, rest = _objectWithoutPropertiesLoose(_ref5, _excluded2), path = useResolvedPath(to, {
+                relative: rest.relative
+            }), location = useLocation(), routerState = React2.useContext(DataRouterStateContext), {
+                navigator: navigator2
+            } = React2.useContext(NavigationContext), toPathname = navigator2.encodeLocation ? navigator2.encodeLocation(path).pathname : path.pathname, locationPathname = location.pathname, nextLocationPathname = routerState && routerState.navigation && routerState.navigation.location ? routerState.navigation.location.pathname : null;
+            caseSensitive || (locationPathname = locationPathname.toLowerCase(), nextLocationPathname = nextLocationPathname ? nextLocationPathname.toLowerCase() : null, toPathname = toPathname.toLowerCase());
             let isActive = locationPathname === toPathname || !end && locationPathname.startsWith(toPathname) && locationPathname.charAt(toPathname.length) === "/",
+                isPending = nextLocationPathname != null && (nextLocationPathname === toPathname || !end && nextLocationPathname.startsWith(toPathname) && nextLocationPathname.charAt(toPathname.length) === "/"),
                 ariaCurrent = isActive ? ariaCurrentProp : void 0,
                 className;
             typeof classNameProp == "function" ? className = classNameProp({
-                isActive
-            }) : className = [classNameProp, isActive ? "active" : null].filter(Boolean).join(" ");
+                isActive,
+                isPending
+            }) : className = [classNameProp, isActive ? "active" : null, isPending ? "pending" : null].filter(Boolean).join(" ");
             let style = typeof styleProp == "function" ? styleProp({
-                isActive
+                isActive,
+                isPending
             }) : styleProp;
-            return /* @__PURE__ */ (0, import_react2.createElement)(Link, _extends2({}, rest, {
+            return /* @__PURE__ */ React2.createElement(Link, _extends3({}, rest, {
                 "aria-current": ariaCurrent,
                 className,
                 ref,
                 style,
                 to
             }), typeof children == "function" ? children({
-                isActive
+                isActive,
+                isPending
             }) : children);
         });
+    var DataRouterHook2;
+    (function(DataRouterHook3) {
+        DataRouterHook3.UseScrollRestoration = "useScrollRestoration", DataRouterHook3.UseSubmitImpl = "useSubmitImpl", DataRouterHook3.UseFetcher = "useFetcher";
+    })(DataRouterHook2 || (DataRouterHook2 = {}));
+    var DataRouterStateHook2;
+    (function(DataRouterStateHook3) {
+        DataRouterStateHook3.UseFetchers = "useFetchers", DataRouterStateHook3.UseScrollRestoration = "useScrollRestoration";
+    })(DataRouterStateHook2 || (DataRouterStateHook2 = {}));
 
     function useLinkClickHandler(to, _temp) {
         let {
             target,
             replace: replaceProp,
-            state
-        } = _temp === void 0 ? {} : _temp, navigate = useNavigate(), location = useLocation(), path = useResolvedPath(to);
-        return (0, import_react2.useCallback)((event) => {
-            if (event.button === 0 && (!target || target === "_self") && !isModifiedEvent(event)) {
+            state,
+            preventScrollReset,
+            relative
+        } = _temp === void 0 ? {} : _temp, navigate = useNavigate(), location = useLocation(), path = useResolvedPath(to, {
+            relative
+        });
+        return React2.useCallback((event) => {
+            if (shouldProcessLinkClick(event, target)) {
                 event.preventDefault();
-                let replace = !!replaceProp || createPath(location) === createPath(path);
+                let replace = replaceProp !== void 0 ? replaceProp : createPath(location) === createPath(path);
                 navigate(to, {
                     replace,
-                    state
+                    state,
+                    preventScrollReset,
+                    relative
                 });
             }
-        }, [location, navigate, path, replaceProp, state, target, to]);
+        }, [location, navigate, path, replaceProp, state, target, to, preventScrollReset, relative]);
+    }
+
+    function usePrompt(_ref8) {
+        let {
+            when,
+            message
+        } = _ref8, blocker = useBlocker(when);
+        React2.useEffect(() => {
+            blocker.state === "blocked" && !when && blocker.reset();
+        }, [blocker, when]), React2.useEffect(() => {
+            blocker.state === "blocked" && (window.confirm(message) ? setTimeout(blocker.proceed, 0) : blocker.reset());
+        }, [blocker, message]);
     }
 
     // ../lektor/translations/ca.json
     var ca_default = {
         RETURN_TO_WEBSITE: "Tornar al Lloc Web",
         UNLOAD_ACTIVE_TAB: "Hi ha informaci\xF3 sense desar, est\xE0 segur que vol abandonar aquesta p\xE0gina?",
         EDIT_METADATA: "Editar Metadades",
@@ -8633,15 +10651,22 @@
         FAILED_TO_OPEN_CONTENT_FILE: "Failed to open content file",
         OPEN_OTHER_PROJECT: "Open other Project",
         OPEN_OTHER_PROJECT_QUESTION: "Opening this file requires opening another project (%s). The current project will be closed. Do you want to continue?",
         COLLAPSE: "Collapse",
         EXPAND: "Expand",
         TRISTATE_CHECKBOX_TOOLTIP: "Tri-state checkbox: use <del> or <backspace> to revert to unset",
         AUTOSIZE_TEXTAREA: "Autosize textarea",
-        SHRINK_TEXTAREA: "Shrink textarea"
+        SHRINK_TEXTAREA: "Shrink textarea",
+        PREFERENCES: "Preferences",
+        RESET: "Reset",
+        RESET_TO_DEFAULTS: "Reset to defaults",
+        EDIT_SHORTCUT: "Edit",
+        SAVE_SHORTCUT: "Save",
+        PREVIEW_SHORTCUT: "(Save &) Preview",
+        SEARCH_SHORTCUT: "Search"
     };
 
     // ../lektor/translations/es.json
     var es_default = {
         RETURN_TO_WEBSITE: "Volver al Sitio Web",
         UNLOAD_ACTIVE_TAB: "Tiene informaci\xF3n sin guardar, est\xE1 seguro de que quiere abandonar esta p\xE1gina?",
         EDIT_METADATA: "Editar Metadatos",
@@ -9957,40 +11982,40 @@
     }
 
     function trans_format(key, replacement) {
         return trans(key).replace("%s", replacement);
     }
 
     // js/context/record-context.ts
-    var import_react3 = __toESM(require_react()),
-        RecordContext = (0, import_react3.createContext)({
+    var import_react = __toESM(require_react()),
+        RecordContext = (0, import_react.createContext)({
             path: "/",
             alt: "_primary"
         });
 
     function useRecord() {
-        return (0, import_react3.useContext)(RecordContext);
+        return (0, import_react.useContext)(RecordContext);
     }
 
     function useRecordAlt() {
         return useRecord().alt;
     }
 
     function useRecordPath() {
         return useRecord().path;
     }
 
     // js/views/App.tsx
     var import_react58 = __toESM(require_react());
 
     // js/header/Header.tsx
-    var import_react9 = __toESM(require_react());
+    var import_react7 = __toESM(require_react());
 
     // js/header/BreadCrumbs.tsx
-    var import_react7 = __toESM(require_react());
+    var import_react5 = __toESM(require_react());
 
     // js/fetch.ts
     var FetchError = class extends Error {
         constructor(code) {
             super();
             this.code = code;
         }
@@ -10002,23 +12027,23 @@
         return response.json();
     }
     var credentials = "same-origin",
         headers = {
             "Content-Type": "application/json"
         };
 
-    function fetchJSON(input, method, json) {
-        let init = json === void 0 ? {
+    function fetchJSON(input, method, json2) {
+        let init = json2 === void 0 ? {
             credentials,
             method
         } : {
             credentials,
             method,
             headers,
-            body: JSON.stringify(json)
+            body: JSON.stringify(json2)
         };
         return fetch(input, init).then(handleJSON);
     }
 
     function apiUrl(endpoint, params) {
         let url = `${$LEKTOR_CONFIG.admin_root}/api${endpoint}`;
         if (params) {
@@ -10031,22 +12056,22 @@
     }
 
     function get(endpoint, params) {
         let url = apiUrl(endpoint, params);
         return fetchJSON(url, "GET");
     }
 
-    function post(endpoint, params, json) {
+    function post(endpoint, params, json2) {
         let url = apiUrl(endpoint, params);
-        return fetchJSON(url, "POST", json);
+        return fetchJSON(url, "POST", json2);
     }
 
-    function put(endpoint, json) {
+    function put(endpoint, json2) {
         let url = apiUrl(endpoint);
-        return fetchJSON(url, "PUT", json);
+        return fetchJSON(url, "PUT", json2);
     }
 
     // js/events.ts
     function dispatch(type, detail) {
         document.dispatchEvent(new CustomEvent(type, {
             detail
         }));
@@ -10058,33 +12083,33 @@
 
     function unsubscribe(type, handler) {
         document.removeEventListener(type, handler);
     }
 
     // js/error-dialog.ts
     function showErrorDialog(error) {
-        error instanceof FetchError ? dispatch("lektor-error", error) : console.error("unknown error:", error);
+        throw error instanceof FetchError ? dispatch("lektor-error", error) : console.error("unknown error:", error), error;
     }
 
     // js/components/AdminLink.tsx
-    var import_react5 = __toESM(require_react());
+    var import_react3 = __toESM(require_react());
 
     // js/components/use-go-to-admin-page.ts
-    var import_react4 = __toESM(require_react());
+    var import_react2 = __toESM(require_react());
 
     function adminPath(page, path, alt) {
         let params = new URLSearchParams({
             path
         });
-        return alt !== "_primary" && params.set("alt", alt), `${$LEKTOR_CONFIG.admin_root}/${page}?${params}`;
+        return alt !== "_primary" && params.set("alt", alt), `/${page}?${params}`;
     }
 
     function useGoToAdminPage() {
         let navigate = useNavigate();
-        return (0, import_react4.useCallback)(
+        return (0, import_react2.useCallback)(
             (name, path, alt) => {
                 navigate(adminPath(name, path, alt));
             },
             [navigate]
         );
     }
 
@@ -10101,118 +12126,118 @@
                 "page",
                 "path",
                 "alt",
                 "children"
             ]);
         let current = useRecord(),
             recordMatches = path === current.path && alt === current.alt;
-        return /* @__PURE__ */ import_react5.default.createElement(
+        return /* @__PURE__ */ import_react3.default.createElement(
             NavLink,
             __spreadValues({
                 to: adminPath(page, path, alt),
                 className: ({
                     isActive
                 }) => isActive && recordMatches ? "active" : void 0
             }, otherProps),
             children
         );
     }
-    var AdminLink_default = (0, import_react5.memo)(AdminLink);
+    var AdminLink_default = (0, import_react3.memo)(AdminLink);
 
     // js/context/page-context.ts
-    var import_react6 = __toESM(require_react()),
+    var import_react4 = __toESM(require_react()),
         PAGE_NAMES = [
             "edit",
             "delete",
             "preview",
             "add-child",
             "upload"
         ];
 
     function isPageName(p) {
         return PAGE_NAMES.includes(p);
     }
-    var PageContext = (0, import_react6.createContext)("edit");
+    var PageContext = (0, import_react4.createContext)("edit");
 
     // js/header/BreadCrumbs.tsx
     function Crumb({
         alt,
         item,
         targetPage
     }) {
         let {
             path,
             exists
         } = item, label = exists ? trans_fallback(item.label_i18n, item.label) : item.id;
-        return /* @__PURE__ */ import_react7.default.createElement("li", {
+        return /* @__PURE__ */ import_react5.default.createElement("li", {
             className: exists ? "breadcrumb-item" : "breadcrumb-item missing-record-crumb"
-        }, /* @__PURE__ */ import_react7.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react5.default.createElement(AdminLink_default, {
             page: targetPage,
             path,
             alt
         }, label));
     }
 
     function AddNewPage({
         alt,
         item
     }) {
-        return item.can_have_children ? /* @__PURE__ */ import_react7.default.createElement("li", {
+        return item.can_have_children ? /* @__PURE__ */ import_react5.default.createElement("li", {
             className: "new-record-crumb"
-        }, /* @__PURE__ */ import_react7.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react5.default.createElement(AdminLink_default, {
             page: "add-child",
             path: item.path,
             alt
         }, "+")) : null;
     }
 
     function BreadCrumbs() {
-        let page = (0, import_react7.useContext)(PageContext),
+        let page = (0, import_react5.useContext)(PageContext),
             {
                 path,
                 alt
             } = useRecord(),
-            [segments, setSegments] = (0, import_react7.useState)(
+            [segments, setSegments] = (0, import_react5.useState)(
                 null
             );
-        if ((0, import_react7.useEffect)(() => {
+        if ((0, import_react5.useEffect)(() => {
                 let ignore = !1;
                 return get("/pathinfo", {
                     path
                 }).then((resp) => {
                     ignore || setSegments(resp.segments);
                 }, showErrorDialog), () => {
                     ignore = !0;
                 };
             }, [path]), !segments)
-            return /* @__PURE__ */ import_react7.default.createElement("ul", {
+            return /* @__PURE__ */ import_react5.default.createElement("ul", {
                 className: "breadcrumb"
-            }, /* @__PURE__ */ import_react7.default.createElement("li", null, /* @__PURE__ */ import_react7.default.createElement(AdminLink_default, {
+            }, /* @__PURE__ */ import_react5.default.createElement("li", null, /* @__PURE__ */ import_react5.default.createElement(AdminLink_default, {
                 page: "edit",
                 path: "/",
                 alt: "_primary"
             }, trans("BACK_TO_OVERVIEW"))));
         let target = page === "preview" ? "preview" : "edit",
             lastItem = segments[segments.length - 1];
-        return /* @__PURE__ */ import_react7.default.createElement("ul", {
+        return /* @__PURE__ */ import_react5.default.createElement("ul", {
             className: "breadcrumb"
-        }, segments.map((item) => /* @__PURE__ */ import_react7.default.createElement(Crumb, {
+        }, segments.map((item) => /* @__PURE__ */ import_react5.default.createElement(Crumb, {
             key: item.path,
             item,
             alt,
             targetPage: target
-        })), /* @__PURE__ */ import_react7.default.createElement(AddNewPage, {
+        })), /* @__PURE__ */ import_react5.default.createElement(AddNewPage, {
             item: lastItem,
             alt
         }));
     }
     var BreadCrumbs_default = BreadCrumbs;
 
     // js/header/GlobalActions.tsx
-    var import_react8 = __toESM(require_react());
+    var import_react6 = __toESM(require_react());
 
     // js/utils.ts
     function isValidUrl(url) {
         return !!url.match(/^([a-z0-9+.-]+):(\/\/)?[^/]\S+$/);
     }
 
     function trimLeadingSlashes(string) {
@@ -10231,387 +12256,434 @@
     }
 
     function getCanonicalUrl(localPath) {
         return `${trimTrailingSlashes($LEKTOR_CONFIG.site_root)}/${trimLeadingSlashes(localPath)}`;
     }
 
     function getPlatform() {
-        return navigator.appVersion.indexOf("Win") !== -1 ? "windows" : navigator.appVersion.indexOf("Mac") !== -1 ? "mac" : navigator.appVersion.indexOf("X11") !== -1 || navigator.appVersion.indexOf("Linux") !== -1 ? "linux" : "other";
+        try {
+            let appVersion = navigator == null ? void 0 : navigator.appVersion;
+            return appVersion != null && appVersion.match(/Win/) ? "windows" : appVersion != null && appVersion.match(/\bMac/) ? "mac" : appVersion != null && appVersion.match(/\b(X11|Linux)/) ? "linux" : null;
+        } catch (e) {
+            return null;
+        }
     }
 
-    function getKey(shortcut) {
-        return getPlatform() === "mac" && shortcut.mac ? shortcut.mac : shortcut.key;
+    function getParentPath(path) {
+        let match = /^(\/.*)\/[^/]*$/.exec(path);
+        return match ? match[1] : null;
     }
 
-    function keyboardShortcutHandler(shortcut, action) {
-        let key = getKey(shortcut);
-        return (ev) => {
-            let eventKey = ev.key;
-            ev.altKey && (eventKey = `Alt+${eventKey}`), ev.ctrlKey && (eventKey = `Control+${eventKey}`), ev.metaKey && (eventKey = `Meta+${eventKey}`), eventKey === key && (shortcut.preventDefault && ev.preventDefault(), action(ev));
-        };
+    // js/shortcut-keys.ts
+    var shortcutKeyRegexp = new RegExp(
+        [
+            "^",
+            "(?:Meta\\+)?(?:Control\\+)?(?:Alt\\+)?(?:Shift\\+)?",
+            "(?<=\\+)[A-Z]\\w*",
+            "$"
+        ].join("")
+    );
+
+    function isValidShortcutKey(value) {
+        return typeof value == "string" && shortcutKeyRegexp.test(value);
     }
 
-    function getParentPath(path) {
-        let match = /^(\/.*)\/[^/]*$/.exec(path);
-        return match ? match[1] : null;
+    function mod(key) {
+        return `${getPlatform() === "mac" ? "Meta" : "Control"}+${key}`;
+    }
+    var defaultShortcutKeyMap = /* @__PURE__ */ new Map([
+            ["EDIT_SHORTCUT" /* Edit */ , mod("E")],
+            ["PREVIEW_SHORTCUT" /* Preview */ , mod("S")],
+            ["SAVE_SHORTCUT" /* Save */ , null],
+            ["SEARCH_SHORTCUT" /* Search */ , mod("G")]
+        ]),
+        ignoredKeys = /* @__PURE__ */ new Set([
+            "Unidentified",
+            // Modifier Keys
+            "Alt",
+            "AltGraph",
+            "CapsLock",
+            "Control",
+            "Fn",
+            "FnLock",
+            "Meta",
+            "NumLock",
+            "ScrollLock",
+            "Shift",
+            "Symbol",
+            "SymbolLock",
+            "Hyper",
+            "Super",
+            // Legacy Modifier Keys
+            "Hyper",
+            "Super"
+        ]),
+        eraseHotkeyKeys = /* @__PURE__ */ new Set([
+            "Backspace",
+            "Delete",
+            " "
+            // space key
+        ]);
+
+    function isPrintingKey(key) {
+        return key.length === 1 || key == "Enter" || key == "Tab";
+    }
+    var modifierKeys = ["Meta", "Control", "Alt", "Shift"];
+
+    function getShortcutKey(event) {
+        if ((event instanceof Event ? event : event.nativeEvent).isComposing || ignoredKeys.has(event.key))
+            return null;
+        let activeMods = modifierKeys.filter((mod2) => event.getModifierState(mod2));
+        if (activeMods.length === 0 && eraseHotkeyKeys.has(event.key) || isPrintingKey(event.key) && !activeMods.some((mod2) => mod2 != "Shift"))
+            return null;
+        let key = event.key.length == 1 ? event.key.toUpperCase() : event.key;
+        return [...activeMods, key].join("+");
+    }
+    var shortcutHandlers = /* @__PURE__ */ new Map();
+
+    function setShortcutHandler(action, handler) {
+        let prevHandler = shortcutHandlers.get(action);
+        return shortcutHandlers.set(action, handler), () => prevHandler ? shortcutHandlers.set(action, prevHandler) : shortcutHandlers.delete(action);
+    }
+
+    function dispatchShortcut(action) {
+        let handler = shortcutHandlers.get(action);
+        handler && handler();
+    }
+
+    function installShortcutKeyListener(keymap) {
+        let actionForKey = new Map(
+                Array.from(keymap.entries()).filter(([, key]) => key).map(([action, key]) => [key, action])
+            ),
+            keydownListener = (event) => {
+                let key = getShortcutKey(event),
+                    action = key && actionForKey.get(key);
+                action && (event.preventDefault(), event.stopPropagation(), dispatchShortcut(action));
+            };
+        return window.addEventListener("keydown", keydownListener), () => window.removeEventListener("keydown", keydownListener);
+    }
+
+    function serializeShortcutKeyMap(keymap) {
+        return Object.fromEntries(
+            Array.from(keymap.entries()).filter(([, key]) => key)
+        );
+    }
+
+    function deserializeShortcutKeyMap(obj) {
+        let data = obj;
+        return new Map(
+            Array.from(defaultShortcutKeyMap.keys(), (action) => {
+                var _a2;
+                let key = (_a2 = data[action]) != null ? _a2 : null;
+                if (key !== null && !isValidShortcutKey(key))
+                    throw new Error("Invalid value for ShortcutKey in serialized keymap");
+                return [action, key];
+            })
+        );
     }
 
     // js/header/GlobalActions.tsx
     var findFiles = () => dispatch("lektor-dialog", {
             type: "find-files"
         }),
         refresh = () => dispatch("lektor-dialog", {
             type: "refresh"
         }),
         publish = () => dispatch("lektor-dialog", {
             type: "publish"
         }),
-        onKeyPress = keyboardShortcutHandler({
-                key: "Control+g",
-                mac: "Meta+g",
-                preventDefault: !0
-            },
-            findFiles
-        );
+        preferences = () => dispatch("lektor-dialog", {
+            type: "preferences"
+        });
 
     function GlobalActions() {
         let record = useRecord();
-        (0, import_react8.useEffect)(() => (window.addEventListener("keydown", onKeyPress), () => window.removeEventListener("keydown", onKeyPress)), []);
-        let returnToWebsite = (0, import_react8.useCallback)(() => {
+        (0, import_react6.useEffect)(() => setShortcutHandler("SEARCH_SHORTCUT" /* Search */ , findFiles), []);
+        let returnToWebsite = (0, import_react6.useCallback)(() => {
             get("/previewinfo", record).then(({
                 url
             }) => {
                 window.location.href = url === null ? getCanonicalUrl("/") : getCanonicalUrl(url);
             }, showErrorDialog);
         }, [record]);
-        return /* @__PURE__ */ import_react8.default.createElement("div", {
+        return /* @__PURE__ */ import_react6.default.createElement("div", {
             className: "btn-group"
-        }, /* @__PURE__ */ import_react8.default.createElement(
+        }, /* @__PURE__ */ import_react6.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary border",
                 onClick: findFiles,
                 title: trans("FIND_FILES")
             },
             /* @__PURE__ */
-            import_react8.default.createElement("i", {
+            import_react6.default.createElement("i", {
                 className: "fa fa-search fa-fw"
             })
-        ), /* @__PURE__ */ import_react8.default.createElement(
+        ), /* @__PURE__ */ import_react6.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary border",
                 onClick: publish,
                 title: trans("PUBLISH")
             },
             /* @__PURE__ */
-            import_react8.default.createElement("i", {
+            import_react6.default.createElement("i", {
                 className: "fa fa-cloud-upload fa-fw"
             })
-        ), /* @__PURE__ */ import_react8.default.createElement(
+        ), /* @__PURE__ */ import_react6.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary border",
                 onClick: refresh,
                 title: trans("REFRESH_BUILD")
             },
             /* @__PURE__ */
-            import_react8.default.createElement("i", {
+            import_react6.default.createElement("i", {
                 className: "fa fa-refresh fa-fw"
             })
-        ), /* @__PURE__ */ import_react8.default.createElement(
+        ), /* @__PURE__ */ import_react6.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary border",
                 onClick: returnToWebsite,
                 title: trans("RETURN_TO_WEBSITE")
             },
             /* @__PURE__ */
-            import_react8.default.createElement("i", {
+            import_react6.default.createElement("i", {
                 className: "fa fa-eye fa-fw"
             })
+        ), /* @__PURE__ */ import_react6.default.createElement(
+            "button", {
+                type: "button",
+                className: "btn btn-secondary border",
+                onClick: preferences,
+                title: trans("PREFERENCES")
+            },
+            /* @__PURE__ */
+            import_react6.default.createElement("i", {
+                className: "fa fa-gear fa-fw"
+            })
         ));
     }
 
     // js/header/Header.tsx
     function Header({
         sidebarIsActive,
         toggleSidebar
     }) {
-        return /* @__PURE__ */ import_react9.default.createElement("header", null, /* @__PURE__ */ import_react9.default.createElement("div", {
+        return /* @__PURE__ */ import_react7.default.createElement("header", null, /* @__PURE__ */ import_react7.default.createElement("div", {
             className: "container"
-        }, /* @__PURE__ */ import_react9.default.createElement(
+        }, /* @__PURE__ */ import_react7.default.createElement(
             "button", {
                 type: "button",
                 className: sidebarIsActive ? "fa fa-bars navbar-toggle active" : "fa fa-bars navbar-toggle",
                 onClick: toggleSidebar,
                 "aria-label": "Toggle navigation"
             }
-        ), /* @__PURE__ */ import_react9.default.createElement("div", {
+        ), /* @__PURE__ */ import_react7.default.createElement("div", {
             className: "d-flex justify-content-between"
-        }, /* @__PURE__ */ import_react9.default.createElement(BreadCrumbs_default, null), /* @__PURE__ */ import_react9.default.createElement("div", null, /* @__PURE__ */ import_react9.default.createElement(GlobalActions, null)))));
+        }, /* @__PURE__ */ import_react7.default.createElement(BreadCrumbs_default, null), /* @__PURE__ */ import_react7.default.createElement("div", null, /* @__PURE__ */ import_react7.default.createElement(GlobalActions, null)))));
     }
 
     // js/sidebar/Sidebar.tsx
-    var import_react16 = __toESM(require_react());
-
-    // js/sidebar/PageActions.tsx
-    var import_react11 = __toESM(require_react());
-
-    // js/components/AdminLinkWithHotkey.tsx
-    var import_react10 = __toESM(require_react());
-
-    function useKeyboardShortcut(key, action) {
-        (0, import_react10.useEffect)(() => {
-            let handler = keyboardShortcutHandler(key, action);
-            return window.addEventListener("keydown", handler), () => window.removeEventListener("keydown", handler);
-        }, [key, action]);
-    }
-
-    function useKeyboardShortcutRef(key) {
-        let el = (0, import_react10.useRef)(null),
-            handler = (0, import_react10.useCallback)(() => {
-                var _a2;
-                (_a2 = el.current) == null || _a2.click();
-            }, []);
-        return useKeyboardShortcut(key, handler), el;
-    }
-
-    function AdminLinkWithHotkey(_a2) {
-        var _b = _a2,
-            {
-                page,
-                path,
-                alt,
-                children,
-                shortcut
-            } = _b,
-            otherProps = __objRest(_b, [
-                "page",
-                "path",
-                "alt",
-                "children",
-                "shortcut"
-            ]);
-        let el = useKeyboardShortcutRef(shortcut),
-            current = useRecord(),
-            recordMatches = path === current.path && alt === current.alt;
-        return /* @__PURE__ */ import_react10.default.createElement(
-            NavLink,
-            __spreadValues({
-                to: adminPath(page, path, alt),
-                className: ({
-                    isActive
-                }) => isActive && recordMatches ? "active" : void 0,
-                ref: el
-            }, otherProps),
-            children
-        );
-    }
+    var import_react13 = __toESM(require_react());
 
     // js/sidebar/PageActions.tsx
+    var import_react8 = __toESM(require_react());
     var getBrowseButtonTitle = () => {
         let platform = getPlatform();
         return platform === "mac" ? trans("BROWSE_FS_MAC") : platform === "windows" ? trans("BROWSE_FS_WINDOWS") : trans("BROWSE_FS");
     };
 
     function BrowseFSLink() {
         let record = useRecord(),
-            fsOpen = (0, import_react11.useCallback)(
+            fsOpen = (0, import_react8.useCallback)(
                 (ev) => {
                     ev.preventDefault(), post("/browsefs", record).then(({
                         okay
                     }) => {
                         okay || alert(trans("ERROR_CANNOT_BROWSE_FS"));
                     }, showErrorDialog);
                 },
                 [record]
             );
-        return /* @__PURE__ */ import_react11.default.createElement("a", {
+        return /* @__PURE__ */ import_react8.default.createElement("a", {
             href: "#",
             onClick: fsOpen
         }, getBrowseButtonTitle());
     }
-    var editKey = {
-        key: "Control+e",
-        mac: "Meta+e",
-        preventDefault: !0
-    };
 
     function PageActions({
         recordInfo
     }) {
         let {
             path,
             alt
         } = useRecord();
-        return /* @__PURE__ */ import_react11.default.createElement(import_react11.default.Fragment, null, /* @__PURE__ */ import_react11.default.createElement("h3", null, recordInfo.is_attachment ? trans("ATTACHMENT_ACTIONS") : trans("PAGE_ACTIONS")), /* @__PURE__ */ import_react11.default.createElement("ul", {
+        return /* @__PURE__ */ import_react8.default.createElement(import_react8.default.Fragment, null, /* @__PURE__ */ import_react8.default.createElement("h3", null, recordInfo.is_attachment ? trans("ATTACHMENT_ACTIONS") : trans("PAGE_ACTIONS")), /* @__PURE__ */ import_react8.default.createElement("ul", {
             className: "nav"
-        }, /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "edit"
-        }, /* @__PURE__ */ import_react11.default.createElement(
-            AdminLinkWithHotkey, {
-                page: "edit",
-                path,
-                alt,
-                shortcut: editKey
-            },
-            recordInfo.is_attachment ? trans("EDIT_METADATA") : trans("EDIT")
-        )), recordInfo.can_be_deleted && /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, /* @__PURE__ */ import_react8.default.createElement(AdminLink_default, {
+            page: "edit",
+            path,
+            alt
+        }, recordInfo.is_attachment ? trans("EDIT_METADATA") : trans("EDIT"))), recordInfo.can_be_deleted && /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "delete"
-        }, /* @__PURE__ */ import_react11.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react8.default.createElement(AdminLink_default, {
             page: "delete",
             path,
             alt
-        }, trans("DELETE"))), /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, trans("DELETE"))), /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "preview"
-        }, /* @__PURE__ */ import_react11.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react8.default.createElement(AdminLink_default, {
             page: "preview",
             path,
             alt
-        }, trans("PREVIEW"))), recordInfo.exists && /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, trans("PREVIEW"))), recordInfo.exists && /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "fs-open"
-        }, /* @__PURE__ */ import_react11.default.createElement(BrowseFSLink, null)), recordInfo.can_have_children && /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, /* @__PURE__ */ import_react8.default.createElement(BrowseFSLink, null)), recordInfo.can_have_children && /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "add-child"
-        }, /* @__PURE__ */ import_react11.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react8.default.createElement(AdminLink_default, {
             page: "add-child",
             path,
             alt
-        }, trans("ADD_CHILD_PAGE"))), recordInfo.can_have_attachments && /* @__PURE__ */ import_react11.default.createElement("li", {
+        }, trans("ADD_CHILD_PAGE"))), recordInfo.can_have_attachments && /* @__PURE__ */ import_react8.default.createElement("li", {
             key: "add-attachment"
-        }, /* @__PURE__ */ import_react11.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react8.default.createElement(AdminLink_default, {
             page: "upload",
             path,
             alt
         }, trans("ADD_ATTACHMENT")))));
     }
-    var PageActions_default = (0, import_react11.memo)(PageActions);
+    var PageActions_default = (0, import_react8.memo)(PageActions);
 
     // js/sidebar/Alternatives.tsx
-    var import_react12 = __toESM(require_react());
+    var import_react9 = __toESM(require_react());
 
     function Alternatives({
         alts
     }) {
-        let page = (0, import_react12.useContext)(PageContext),
+        let page = (0, import_react9.useContext)(PageContext),
             path = useRecordPath();
         if (alts.length < 2)
             return null;
         let items = alts.map((item) => {
             let title = trans_obj(item.name_i18n);
             item.is_primary ? title += ` (${trans("PRIMARY_ALT")})` : item.primary_overlay && (title += ` (${trans("PRIMARY_OVERLAY")})`);
             let className = item.exists ? "alt" : "alt alt-missing";
-            return /* @__PURE__ */ import_react12.default.createElement("li", {
+            return /* @__PURE__ */ import_react9.default.createElement("li", {
                 key: item.alt,
                 className
-            }, /* @__PURE__ */ import_react12.default.createElement(AdminLink_default, {
+            }, /* @__PURE__ */ import_react9.default.createElement(AdminLink_default, {
                 page,
                 path,
                 alt: item.alt
             }, title));
         });
-        return /* @__PURE__ */ import_react12.default.createElement(import_react12.default.Fragment, null, /* @__PURE__ */ import_react12.default.createElement("h3", null, trans("ALTS")), /* @__PURE__ */ import_react12.default.createElement("ul", {
+        return /* @__PURE__ */ import_react9.default.createElement(import_react9.default.Fragment, null, /* @__PURE__ */ import_react9.default.createElement("h3", null, trans("ALTS")), /* @__PURE__ */ import_react9.default.createElement("ul", {
             className: "nav"
         }, items));
     }
-    var Alternatives_default = (0, import_react12.memo)(Alternatives);
+    var Alternatives_default = (0, import_react9.memo)(Alternatives);
 
     // js/sidebar/AttachmentActions.tsx
-    var import_react13 = __toESM(require_react());
+    var import_react10 = __toESM(require_react());
 
     function AttachmentActions({
         recordInfo
     }) {
         let alt = useRecordAlt(),
             attachments = recordInfo.attachments;
-        return /* @__PURE__ */ import_react13.default.createElement(import_react13.default.Fragment, null, /* @__PURE__ */ import_react13.default.createElement("h3", null, trans("ATTACHMENTS")), /* @__PURE__ */ import_react13.default.createElement("ul", {
+        return /* @__PURE__ */ import_react10.default.createElement(import_react10.default.Fragment, null, /* @__PURE__ */ import_react10.default.createElement("h3", null, trans("ATTACHMENTS")), /* @__PURE__ */ import_react10.default.createElement("ul", {
             className: "nav"
-        }, attachments.length > 0 ? attachments.map((atch) => /* @__PURE__ */ import_react13.default.createElement("li", {
+        }, attachments.length > 0 ? attachments.map((atch) => /* @__PURE__ */ import_react10.default.createElement("li", {
             key: atch.id
-        }, /* @__PURE__ */ import_react13.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react10.default.createElement(AdminLink_default, {
             page: "edit",
             path: atch.path,
             alt
-        }, atch.id, " (", atch.type, ")"))) : /* @__PURE__ */ import_react13.default.createElement("li", {
+        }, atch.id, " (", atch.type, ")"))) : /* @__PURE__ */ import_react10.default.createElement("li", {
             key: "_missing"
-        }, /* @__PURE__ */ import_react13.default.createElement("em", null, trans("NO_ATTACHMENTS")))));
+        }, /* @__PURE__ */ import_react10.default.createElement("em", null, trans("NO_ATTACHMENTS")))));
     }
-    var AttachmentActions_default = (0, import_react13.memo)(AttachmentActions);
+    var AttachmentActions_default = (0, import_react10.memo)(AttachmentActions);
 
     // js/sidebar/ChildActions.tsx
-    var import_react15 = __toESM(require_react());
+    var import_react12 = __toESM(require_react());
 
     // js/sidebar/ChildPagination.tsx
-    var import_react14 = __toESM(require_react());
+    var import_react11 = __toESM(require_react());
 
     function ChildPagination({
         page,
         numberOfChildren,
         setPage
     }) {
         let pages = Math.ceil(numberOfChildren / 15);
-        return pages <= 1 ? null : /* @__PURE__ */ import_react14.default.createElement("li", {
+        return pages <= 1 ? null : /* @__PURE__ */ import_react11.default.createElement("li", {
             className: "pagination"
-        }, page > 1 ? /* @__PURE__ */ import_react14.default.createElement(
+        }, page > 1 ? /* @__PURE__ */ import_react11.default.createElement(
             "a", {
                 href: "#",
                 onClick: (ev) => {
                     ev.preventDefault(), setPage(page - 1);
                 }
             },
             "\xAB"
-        ) : /* @__PURE__ */ import_react14.default.createElement("em", null, "\xAB"), /* @__PURE__ */ import_react14.default.createElement("span", {
+        ) : /* @__PURE__ */ import_react11.default.createElement("em", null, "\xAB"), /* @__PURE__ */ import_react11.default.createElement("span", {
             className: "page"
-        }, page + " / " + pages), page < pages ? /* @__PURE__ */ import_react14.default.createElement(
+        }, page + " / " + pages), page < pages ? /* @__PURE__ */ import_react11.default.createElement(
             "a", {
                 href: "#",
                 onClick: (ev) => {
                     ev.preventDefault(), setPage(page + 1);
                 }
             },
             "\xBB"
-        ) : /* @__PURE__ */ import_react14.default.createElement("em", null, "\xBB"));
+        ) : /* @__PURE__ */ import_react11.default.createElement("em", null, "\xBB"));
     }
 
     // js/sidebar/ChildActions.tsx
     function ChildActions({
         targetPage,
         allChildren,
         page,
         setPage
     }) {
         let alt = useRecordAlt(),
             shownChildren = allChildren.slice(
                 (page - 1) * 15,
                 page * 15
             );
-        return /* @__PURE__ */ import_react15.default.createElement(import_react15.default.Fragment, null, /* @__PURE__ */ import_react15.default.createElement("h3", null, trans("CHILD_PAGES")), /* @__PURE__ */ import_react15.default.createElement("ul", {
+        return /* @__PURE__ */ import_react12.default.createElement(import_react12.default.Fragment, null, /* @__PURE__ */ import_react12.default.createElement("h3", null, trans("CHILD_PAGES")), /* @__PURE__ */ import_react12.default.createElement("ul", {
             className: "nav"
-        }, /* @__PURE__ */ import_react15.default.createElement(
+        }, /* @__PURE__ */ import_react12.default.createElement(
             ChildPagination, {
                 numberOfChildren: allChildren.length,
                 page,
                 setPage
             }
-        ), shownChildren.length > 0 ? shownChildren.map((child) => /* @__PURE__ */ import_react15.default.createElement("li", {
+        ), shownChildren.length > 0 ? shownChildren.map((child) => /* @__PURE__ */ import_react12.default.createElement("li", {
             key: child.id
-        }, /* @__PURE__ */ import_react15.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react12.default.createElement(AdminLink_default, {
             page: targetPage,
             path: child.path,
             alt
-        }, trans_obj(child.label_i18n)))) : /* @__PURE__ */ import_react15.default.createElement("li", {
+        }, trans_obj(child.label_i18n)))) : /* @__PURE__ */ import_react12.default.createElement("li", {
             key: "_missing"
-        }, /* @__PURE__ */ import_react15.default.createElement("em", null, trans("NO_CHILD_PAGES")))));
+        }, /* @__PURE__ */ import_react12.default.createElement("em", null, trans("NO_CHILD_PAGES")))));
     }
 
     // js/sidebar/Sidebar.tsx
     var ChildPosCache = class {
             constructor() {
                 this.memo = [];
             }
+            /** Remember the page for a record. */
             rememberPosition(record, page) {
                 this.memo = this.memo.filter(([r]) => r !== record), this.memo.unshift([record, page]), this.memo.length > 5 && (this.memo.length = 5);
             }
             getPosition(record, childCount) {
                 var _a2;
                 let page = (_a2 = this.memo.find(([r]) => r === record)) == null ? void 0 : _a2[1];
                 return page ? Math.min(page, Math.ceil(childCount / 15)) : 1;
@@ -10620,133 +12692,133 @@
         compareAlternatives = (a, b) => {
             let nameA = (a.is_primary ? "A" : "B") + trans_obj(a.name_i18n),
                 nameB = (b.is_primary ? "A" : "B") + trans_obj(b.name_i18n);
             return nameA === nameB ? 0 : nameA < nameB ? -1 : 1;
         };
 
     function Sidebar() {
-        let page = (0, import_react16.useContext)(PageContext),
+        let page = (0, import_react13.useContext)(PageContext),
             path = useRecordPath(),
-            [recordInfo, setRecordInfo] = (0, import_react16.useState)(null),
-            [childrenPage, setChildrenPage] = (0, import_react16.useState)(1),
-            [childPosCache] = (0, import_react16.useState)(() => new ChildPosCache()),
-            [updateForced, forceUpdate] = (0, import_react16.useReducer)((x) => x + 1, 0);
-        return (0, import_react16.useEffect)(() => {
+            [recordInfo, setRecordInfo] = (0, import_react13.useState)(null),
+            [childrenPage, setChildrenPage] = (0, import_react13.useState)(1),
+            [childPosCache] = (0, import_react13.useState)(() => new ChildPosCache()),
+            [updateForced, forceUpdate] = (0, import_react13.useReducer)((x) => x + 1, 0);
+        return (0, import_react13.useEffect)(() => {
             let handler = ({
                 detail
             }) => {
                 detail === path && forceUpdate();
             };
             return subscribe("lektor-attachments-changed", handler), () => unsubscribe("lektor-attachments-changed", handler);
-        }, [path]), (0, import_react16.useEffect)(() => {
+        }, [path]), (0, import_react13.useEffect)(() => {
             let ignore = !1;
             return get("/recordinfo", {
                 path
             }).then((resp) => {
                 ignore || (setRecordInfo(__spreadProps(__spreadValues({}, resp), {
                     alts: resp.alts.sort(compareAlternatives)
                 })), setChildrenPage(childPosCache.getPosition(path, resp.children.length)));
             }, showErrorDialog), () => {
                 ignore = !0;
             };
-        }, [path, childPosCache, updateForced]), recordInfo ? /* @__PURE__ */ import_react16.default.createElement(import_react16.default.Fragment, null, /* @__PURE__ */ import_react16.default.createElement(PageActions_default, {
+        }, [path, childPosCache, updateForced]), recordInfo ? /* @__PURE__ */ import_react13.default.createElement(import_react13.default.Fragment, null, /* @__PURE__ */ import_react13.default.createElement(PageActions_default, {
             recordInfo
-        }), /* @__PURE__ */ import_react16.default.createElement(Alternatives_default, {
+        }), /* @__PURE__ */ import_react13.default.createElement(Alternatives_default, {
             alts: recordInfo.alts
-        }), recordInfo.can_have_children && /* @__PURE__ */ import_react16.default.createElement(
+        }), recordInfo.can_have_children && /* @__PURE__ */ import_react13.default.createElement(
             ChildActions, {
                 targetPage: page === "preview" ? "preview" : "edit",
                 allChildren: recordInfo.children,
                 page: childrenPage,
                 setPage: (page2) => {
                     childPosCache.rememberPosition(path, page2), setChildrenPage(page2);
                 }
             }
-        ), recordInfo.can_have_attachments && /* @__PURE__ */ import_react16.default.createElement(AttachmentActions_default, {
+        ), recordInfo.can_have_attachments && /* @__PURE__ */ import_react13.default.createElement(AttachmentActions_default, {
             recordInfo
         })) : null;
     }
     var Sidebar_default = Sidebar;
 
     // js/components/DialogSlot.tsx
-    var import_react22 = __toESM(require_react());
+    var import_react21 = __toESM(require_react());
 
     // js/dialogs/find-files/FindFiles.tsx
-    var import_react19 = __toESM(require_react());
+    var import_react16 = __toESM(require_react());
 
     // js/components/SlideDialog.tsx
-    var import_react17 = __toESM(require_react());
+    var import_react14 = __toESM(require_react());
 
     function SlideDialog({
         title,
         hasCloseButton,
         dismiss,
         children
     }) {
-        return (0, import_react17.useEffect)(() => {
+        return (0, import_react14.useEffect)(() => {
             let handler = (ev) => {
                 ev.key === "Escape" && (ev.preventDefault(), dismiss());
             };
             return window.addEventListener("keydown", handler), () => window.removeEventListener("keydown", handler);
-        }, [dismiss]), (0, import_react17.useEffect)(() => {
+        }, [dismiss]), (0, import_react14.useEffect)(() => {
             window.scrollTo(0, 0);
-        }, []), /* @__PURE__ */ import_react17.default.createElement("div", {
+        }, []), /* @__PURE__ */ import_react14.default.createElement("div", {
             className: "dialog-slot"
-        }, /* @__PURE__ */ import_react17.default.createElement("div", {
+        }, /* @__PURE__ */ import_react14.default.createElement("div", {
             className: "container"
-        }, /* @__PURE__ */ import_react17.default.createElement("div", {
+        }, /* @__PURE__ */ import_react14.default.createElement("div", {
             className: "sliding-panel col-md-6 offset-md-3"
-        }, hasCloseButton && /* @__PURE__ */ import_react17.default.createElement(
+        }, hasCloseButton && /* @__PURE__ */ import_react14.default.createElement(
             "a", {
                 href: "#",
                 className: "close-btn",
                 onClick: (ev) => {
                     ev.preventDefault(), dismiss();
                 }
             },
             trans("CLOSE")
-        ), /* @__PURE__ */ import_react17.default.createElement("h3", null, title), children)), /* @__PURE__ */ import_react17.default.createElement("div", {
+        ), /* @__PURE__ */ import_react14.default.createElement("h3", null, title), children)), /* @__PURE__ */ import_react14.default.createElement("div", {
             className: "interface-protector"
         }));
     }
 
     // js/dialogs/find-files/ResultRow.tsx
-    var import_react18 = __toESM(require_react());
+    var import_react15 = __toESM(require_react());
 
     function ResultRow({
         result,
         isActive,
         dismiss,
         alt,
         target
     }) {
-        return /* @__PURE__ */ import_react18.default.createElement("li", {
+        return /* @__PURE__ */ import_react15.default.createElement("li", {
             className: isActive ? "active" : ""
-        }, /* @__PURE__ */ import_react18.default.createElement(AdminLink_default, {
+        }, /* @__PURE__ */ import_react15.default.createElement(AdminLink_default, {
             page: target,
             path: result.path,
             alt,
             onClick: dismiss
-        }, result.parents.map((item) => /* @__PURE__ */ import_react18.default.createElement("span", {
+        }, result.parents.map((item) => /* @__PURE__ */ import_react15.default.createElement("span", {
             key: item.title
-        }, item.title)), /* @__PURE__ */ import_react18.default.createElement("strong", null, result.title)));
+        }, item.title)), /* @__PURE__ */ import_react15.default.createElement("strong", null, result.title)));
     }
 
     // js/dialogs/find-files/FindFiles.tsx
     function FindFiles({
         dismiss
     }) {
         let alt = useRecordAlt(),
-            page = (0, import_react19.useContext)(PageContext),
-            [query, setQuery] = (0, import_react19.useState)(""),
-            [results, setResults] = (0, import_react19.useState)([]),
-            [selected, setSelected] = (0, import_react19.useState)(-1),
+            page = (0, import_react16.useContext)(PageContext),
+            [query, setQuery] = (0, import_react16.useState)(""),
+            [results, setResults] = (0, import_react16.useState)([]),
+            [selected, setSelected] = (0, import_react16.useState)(-1),
             goToAdminPage = useGoToAdminPage(),
             target = page === "preview" ? "preview" : "edit";
-        (0, import_react19.useEffect)(() => {
+        (0, import_react16.useEffect)(() => {
             if (!query) {
                 setResults([]), setSelected(-1);
                 return;
             }
             let ignore = !1;
             return post("/find", {
                 q: query,
@@ -10759,259 +12831,431 @@
                     ignore || (setResults(results2), setSelected((selected2) => Math.min(selected2, results2.length - 1)));
                 },
                 showErrorDialog
             ), () => {
                 ignore = !0;
             };
         }, [alt, query]);
-        let onInputKey = (0, import_react19.useCallback)(
+        let onInputKey = (0, import_react16.useCallback)(
             (event) => {
                 if (event.key === "ArrowDown")
                     event.preventDefault(), setSelected((selected2) => (selected2 + 1) % results.length);
                 else if (event.key === "ArrowUp")
                     event.preventDefault(), setSelected(
                         (selected2) => (selected2 - 1 + results.length) % results.length
                     );
                 else if (event.key === "Enter") {
                     let item = results[selected];
                     item && (dismiss(), goToAdminPage(target, item.path, alt));
                 }
             },
             [alt, dismiss, goToAdminPage, results, selected, target]
         );
-        return /* @__PURE__ */ import_react19.default.createElement(SlideDialog, {
+        return /* @__PURE__ */ import_react16.default.createElement(SlideDialog, {
             dismiss,
             hasCloseButton: !0,
             title: trans("FIND_FILES")
-        }, /* @__PURE__ */ import_react19.default.createElement(
+        }, /* @__PURE__ */ import_react16.default.createElement(
             "input", {
                 type: "text",
                 autoFocus: !0,
                 className: "form-control",
                 value: query,
                 onChange: (ev) => setQuery(ev.target.value),
                 onKeyDown: onInputKey,
                 placeholder: trans("FIND_FILES_PLACEHOLDER")
             }
-        ), /* @__PURE__ */ import_react19.default.createElement("ul", {
+        ), /* @__PURE__ */ import_react16.default.createElement("ul", {
             className: "search-results"
-        }, results.map((result, idx) => /* @__PURE__ */ import_react19.default.createElement(
+        }, results.map((result, idx) => /* @__PURE__ */ import_react16.default.createElement(
             ResultRow, {
                 key: result.path,
                 result,
                 isActive: idx === selected,
                 dismiss,
                 alt,
                 target
             }
         ))));
     }
     var FindFiles_default = FindFiles;
 
+    // js/dialogs/Preferences.tsx
+    var import_react18 = __toESM(require_react());
+
+    // js/context/appsettings-context.ts
+    var import_react17 = __toESM(require_react());
+    var defaultAppSettings = {
+            shortcutKeyMap: defaultShortcutKeyMap
+        },
+        AppSettingsContext = (0, import_react17.createContext)(defaultAppSettings);
+
+    function useAppSettings() {
+        return (0, import_react17.useContext)(AppSettingsContext);
+    }
+
+    function serializeAppSettings(settings) {
+        return {
+            shortcutKeyMap: serializeShortcutKeyMap(settings.shortcutKeyMap)
+        };
+    }
+
+    function hasAttribute(obj, attr) {
+        return typeof obj == "object" && obj !== null && attr in obj;
+    }
+
+    function deserializeAppSettings(obj) {
+        if (!hasAttribute(obj, "shortcutKeyMap"))
+            throw new Error("Bad stored value for AppSettings");
+        return {
+            shortcutKeyMap: deserializeShortcutKeyMap(obj.shortcutKeyMap)
+        };
+    }
+    var appSettingsKey = "com.getlektor--appsettings";
+
+    function loadAppSettings() {
+        try {
+            let saved = localStorage.getItem(appSettingsKey);
+            if (saved)
+                return deserializeAppSettings(JSON.parse(saved));
+        } catch (e) {
+            console.log("Failed to load AppSettings from localStorage", e);
+        }
+        return defaultAppSettings;
+    }
+
+    function saveAppSettings(settings) {
+        localStorage.setItem(
+            appSettingsKey,
+            JSON.stringify(serializeAppSettings(settings))
+        );
+    }
+
+    // js/dialogs/Preferences.tsx
+    function Preferences({
+        setAppSettings,
+        dismiss
+    }) {
+        let appSettings = useAppSettings(),
+            [state, setState] = (0, import_react18.useState)(appSettings),
+            save = () => {
+                setAppSettings(state), dismiss();
+            },
+            setKeyMap = (0, import_react18.useCallback)((action) => {
+                setState((state2) => __spreadProps(__spreadValues({}, state2), {
+                    shortcutKeyMap: typeof action == "function" ? action(state2.shortcutKeyMap) : action
+                }));
+            }, []);
+        return /* @__PURE__ */ import_react18.default.createElement(
+            SlideDialog, {
+                dismiss,
+                hasCloseButton: !1,
+                title: trans("PREFERENCES")
+            },
+            /* @__PURE__ */
+            import_react18.default.createElement("form", null, /* @__PURE__ */ import_react18.default.createElement(ShortcutKeyPrefs, {
+                keyMap: state.shortcutKeyMap,
+                setKeyMap
+            }), /* @__PURE__ */ import_react18.default.createElement("div", {
+                className: "d-flex"
+            }, /* @__PURE__ */ import_react18.default.createElement(
+                "button", {
+                    type: "submit",
+                    disabled: state === appSettings,
+                    className: "btn btn-primary border me-2",
+                    onClick: save
+                },
+                trans("SAVE_CHANGES")
+            ), /* @__PURE__ */ import_react18.default.createElement(
+                "button", {
+                    type: "button",
+                    className: "btn btn-secondary border me-2",
+                    disabled: state === defaultAppSettings,
+                    onClick: () => setState(defaultAppSettings)
+                },
+                trans("RESET_TO_DEFAULTS")
+            ), /* @__PURE__ */ import_react18.default.createElement(
+                "button", {
+                    type: "button",
+                    className: "btn btn-secondary border",
+                    onClick: dismiss
+                },
+                trans("CANCEL")
+            )))
+        );
+    }
+
+    function ShortcutKeyPrefs({
+        keyMap,
+        setKeyMap
+    }) {
+        let setShortcut = (0, import_react18.useCallback)(
+            (action, key) => setKeyMap(
+                (keyMap2) => new Map(
+                    Array.from(keyMap2.entries(), ([a, k]) => [
+                        a,
+                        a === action ? key : k !== key ? k : null
+                    ])
+                )
+            ),
+            [setKeyMap]
+        );
+        return /* @__PURE__ */ import_react18.default.createElement("fieldset", {
+            className: "border border-dark p-2 mb-3"
+        }, /* @__PURE__ */ import_react18.default.createElement("legend", null, "Shortcut Keys"), Array.from(keyMap, ([action, key]) => /* @__PURE__ */ import_react18.default.createElement("div", {
+            className: "row mb-3",
+            key: action
+        }, /* @__PURE__ */ import_react18.default.createElement("label", {
+            htmlFor: action,
+            className: "col-sm-6 col-form-label text-end"
+        }, trans(action)), /* @__PURE__ */ import_react18.default.createElement("div", {
+            className: "col-sm-4"
+        }, /* @__PURE__ */ import_react18.default.createElement(
+            ShortcutKeyInputWidget, {
+                value: key,
+                onValueChange: (key2) => setShortcut(action, key2),
+                className: "form-control",
+                id: action
+            }
+        )))));
+    }
+
+    function ShortcutKeyInputWidget(_a2) {
+        var _b = _a2,
+            {
+                value,
+                onValueChange
+            } = _b,
+            props = __objRest(_b, [
+                "value",
+                "onValueChange"
+            ]);
+        return /* @__PURE__ */ import_react18.default.createElement(
+            "input",
+            __spreadValues({
+                type: "text",
+                value: value != null ? value : "",
+                onChange: () => null,
+                onKeyDown: (event) => {
+                    let key = getShortcutKey(event),
+                        doUnset = eraseHotkeyKeys.has(event.key);
+                    (key || doUnset) && (event.preventDefault(), event.stopPropagation(), onValueChange(key));
+                }
+            }, props)
+        );
+    }
+
     // js/dialogs/Publish.tsx
-    var import_react20 = __toESM(require_react());
+    var import_react19 = __toESM(require_react());
 
     function TargetServers({
         activeTarget,
         servers,
         setActiveTarget
     }) {
         function onChange(event) {
             setActiveTarget(event.target.value);
         }
-        let serverOptions = servers.map((server) => /* @__PURE__ */ import_react20.default.createElement("option", {
+        let serverOptions = servers.map((server) => /* @__PURE__ */ import_react19.default.createElement("option", {
             value: server.id,
             key: server.id
         }, trans_fallback(server.name_i18n, server.name) + " (" + server.short_target + ")"));
-        return /* @__PURE__ */ import_react20.default.createElement("dl", null, /* @__PURE__ */ import_react20.default.createElement("dt", null, trans("PUBLISH_SERVER")), /* @__PURE__ */ import_react20.default.createElement("dd", null, /* @__PURE__ */ import_react20.default.createElement("div", {
+        return /* @__PURE__ */ import_react19.default.createElement("dl", null, /* @__PURE__ */ import_react19.default.createElement("dt", null, trans("PUBLISH_SERVER")), /* @__PURE__ */ import_react19.default.createElement("dd", null, /* @__PURE__ */ import_react19.default.createElement("div", {
             className: "input-group"
-        }, /* @__PURE__ */ import_react20.default.createElement(
+        }, /* @__PURE__ */ import_react19.default.createElement(
             "select", {
                 value: activeTarget,
                 onChange,
                 className: "form-control"
             },
             serverOptions
         ))));
     }
 
     function BuildLog({
         log
     }) {
-        let buildLog = (0, import_react20.useRef)(null);
-        return (0, import_react20.useEffect)(() => {
+        let buildLog = (0, import_react19.useRef)(null);
+        return (0, import_react19.useEffect)(() => {
             let node = buildLog.current;
             node && (node.scrollTop = node.scrollHeight);
-        }, [log]), /* @__PURE__ */ import_react20.default.createElement("pre", {
+        }, [log]), /* @__PURE__ */ import_react19.default.createElement("pre", {
             ref: buildLog,
             className: "build-log"
         }, log.join(`
 `));
     }
 
     function Publish({
         dismiss,
         preventNavigation
     }) {
-        let [servers, setServers] = (0, import_react20.useState)([]), [activeTarget, setActiveTarget] = (0, import_react20.useState)(""), [log, setLog] = (0, import_react20.useState)([]), [state, setState] = (0, import_react20.useState)("IDLE");
-        (0, import_react20.useEffect)(() => {
+        let [servers, setServers] = (0, import_react19.useState)([]), [activeTarget, setActiveTarget] = (0, import_react19.useState)(""), [log, setLog] = (0, import_react19.useState)([]), [state, setState] = (0, import_react19.useState)("IDLE");
+        (0, import_react19.useEffect)(() => {
             get("/servers", null).then(({
                 servers: servers2
             }) => {
                 setServers(servers2), setActiveTarget(servers2.length ? servers2[0].id : "");
             }, showErrorDialog);
         }, []);
-        let onPublish = (0, import_react20.useCallback)(() => {
+        let onPublish = (0, import_react19.useCallback)(() => {
                 setLog([]), setState("BUILDING"), preventNavigation(!0), post("/build", null).then(() => {
                     setState("PUBLISH");
                     let eventSource = new EventSource(
                         apiUrl("/publish", {
                             server: activeTarget
                         })
                     );
                     eventSource.addEventListener("message", (event) => {
                         let data = JSON.parse(event.data);
                         data === null ? (setState("DONE"), preventNavigation(!1), eventSource.close()) : setLog((log2) => log2.concat(data.msg));
                     });
                 }, showErrorDialog);
             }, [activeTarget, preventNavigation]),
             isSafeToPublish = state === "IDLE" || state === "DONE";
-        return /* @__PURE__ */ import_react20.default.createElement(
+        return /* @__PURE__ */ import_react19.default.createElement(
             SlideDialog, {
                 dismiss,
                 hasCloseButton: !1,
                 title: trans("PUBLISH")
             },
             /* @__PURE__ */
-            import_react20.default.createElement("p", null, trans("PUBLISH_NOTE")),
+            import_react19.default.createElement("p", null, trans("PUBLISH_NOTE")),
             /* @__PURE__ */
-            import_react20.default.createElement(
+            import_react19.default.createElement(
                 TargetServers, {
                     activeTarget,
                     servers,
                     setActiveTarget
                 }
             ),
             /* @__PURE__ */
-            import_react20.default.createElement("p", null, /* @__PURE__ */ import_react20.default.createElement(
+            import_react19.default.createElement("p", null, /* @__PURE__ */ import_react19.default.createElement(
                 "button", {
                     type: "button",
                     className: "btn btn-primary",
                     disabled: !isSafeToPublish,
                     onClick: onPublish
                 },
                 trans("PUBLISH")
-            ), " ", /* @__PURE__ */ import_react20.default.createElement(
+            ), " ", /* @__PURE__ */ import_react19.default.createElement(
                 "button", {
                     type: "button",
                     className: "btn btn-secondary border",
                     disabled: !isSafeToPublish,
                     onClick: dismiss
                 },
                 trans(state === "DONE" ? "CLOSE" : "CANCEL")
             )),
-            state !== "IDLE" ? /* @__PURE__ */ import_react20.default.createElement(import_react20.default.Fragment, null, /* @__PURE__ */ import_react20.default.createElement("h3", null, state !== "DONE" ? trans("CURRENTLY_PUBLISHING") : trans("PUBLISH_DONE")), /* @__PURE__ */ import_react20.default.createElement("pre", null, trans("STATE") + ": " + trans(`PUBLISH_STATE_${state}`)), /* @__PURE__ */ import_react20.default.createElement(BuildLog, {
+            state !== "IDLE" ? /* @__PURE__ */ import_react19.default.createElement(import_react19.default.Fragment, null, /* @__PURE__ */ import_react19.default.createElement("h3", null, state !== "DONE" ? trans("CURRENTLY_PUBLISHING") : trans("PUBLISH_DONE")), /* @__PURE__ */ import_react19.default.createElement("pre", null, trans("STATE") + ": " + trans(`PUBLISH_STATE_${state}`)), /* @__PURE__ */ import_react19.default.createElement(BuildLog, {
                 log
             })) : null
         );
     }
     var Publish_default = Publish;
 
     // js/dialogs/Refresh.tsx
-    var import_react21 = __toESM(require_react());
+    var import_react20 = __toESM(require_react());
 
     function Refresh({
         dismiss,
         preventNavigation
     }) {
-        let [state, setState] = (0, import_react21.useState)("IDLE"), isSafeToNavigate = state === "IDLE" || state === "DONE", refresh2 = (0, import_react21.useCallback)(() => {
+        let [state, setState] = (0, import_react20.useState)("IDLE"), isSafeToNavigate = state === "IDLE" || state === "DONE", refresh2 = (0, import_react20.useCallback)(() => {
             setState("CLEANING"), post("/clean", null).then(() => {
                 setState("DONE");
             }, showErrorDialog);
         }, []);
-        return (0, import_react21.useEffect)(
+        return (0, import_react20.useEffect)(
             () => preventNavigation(!isSafeToNavigate),
             [preventNavigation, isSafeToNavigate]
-        ), /* @__PURE__ */ import_react21.default.createElement(
+        ), /* @__PURE__ */ import_react20.default.createElement(
             SlideDialog, {
                 dismiss,
                 hasCloseButton: !1,
                 title: trans("REFRESH_BUILD")
             },
             /* @__PURE__ */
-            import_react21.default.createElement("p", null, trans("REFRESH_BUILD_NOTE")),
+            import_react20.default.createElement("p", null, trans("REFRESH_BUILD_NOTE")),
             /* @__PURE__ */
-            import_react21.default.createElement("p", null, /* @__PURE__ */ import_react21.default.createElement(
+            import_react20.default.createElement("p", null, /* @__PURE__ */ import_react20.default.createElement(
                 "button", {
                     type: "button",
                     className: "btn btn-primary",
                     disabled: !isSafeToNavigate,
                     onClick: refresh2
                 },
                 trans("REFRESH_BUILD")
-            ), " ", /* @__PURE__ */ import_react21.default.createElement(
+            ), " ", /* @__PURE__ */ import_react20.default.createElement(
                 "button", {
                     type: "button",
                     className: "btn btn-secondary border",
                     disabled: !isSafeToNavigate,
                     onClick: dismiss
                 },
                 trans(state === "DONE" ? "CLOSE" : "CANCEL")
             )),
-            state !== "IDLE" && /* @__PURE__ */ import_react21.default.createElement("div", null, /* @__PURE__ */ import_react21.default.createElement("h3", null, state !== "DONE" ? trans("CURRENTLY_REFRESHING_BUILD") : trans("REFRESHING_BUILD_DONE")))
+            state !== "IDLE" && /* @__PURE__ */ import_react20.default.createElement("div", null, /* @__PURE__ */ import_react20.default.createElement("h3", null, state !== "DONE" ? trans("CURRENTLY_REFRESHING_BUILD") : trans("REFRESHING_BUILD_DONE")))
         );
     }
 
     // js/components/DialogSlot.tsx
-    function DialogSlot() {
-        let [dialog, setDialog] = (0, import_react22.useState)(null), dismiss = (0, import_react22.useCallback)(
+    function DialogSlot({
+        setAppSettings
+    }) {
+        let [dialog, setDialog] = (0, import_react21.useState)(null), dismiss = (0, import_react21.useCallback)(
             () => setDialog((c) => c != null && c.preventNavigation ? c : null),
             []
-        ), prevent = (0, import_react22.useCallback)(
+        ), prevent = (0, import_react21.useCallback)(
             (preventNavigation) => setDialog((d) => d ? __spreadProps(__spreadValues({}, d), {
                 preventNavigation
             }) : null),
             []
         );
-        if ((0, import_react22.useEffect)(() => {
+        if ((0, import_react21.useEffect)(() => {
                 let handler = ({
                     detail
                 }) => {
                     setDialog((current) => current != null ? current : detail);
                 };
                 return subscribe("lektor-dialog", handler), () => unsubscribe("lektor-dialog", handler);
             }, []), !dialog)
             return null;
         if (dialog.type === "find-files")
-            return /* @__PURE__ */ import_react22.default.createElement(FindFiles_default, {
+            return /* @__PURE__ */ import_react21.default.createElement(FindFiles_default, {
                 dismiss
             });
         if (dialog.type === "refresh")
-            return /* @__PURE__ */ import_react22.default.createElement(Refresh, {
+            return /* @__PURE__ */ import_react21.default.createElement(Refresh, {
                 dismiss,
                 preventNavigation: prevent
             });
         if (dialog.type === "publish")
-            return /* @__PURE__ */ import_react22.default.createElement(Publish_default, {
+            return /* @__PURE__ */ import_react21.default.createElement(Publish_default, {
                 dismiss,
                 preventNavigation: prevent
             });
+        if (dialog.type === "preferences")
+            return /* @__PURE__ */ import_react21.default.createElement(Preferences, {
+                setAppSettings,
+                dismiss
+            });
         let exhaustiveCheck = dialog.type;
         throw new Error(exhaustiveCheck);
     }
 
     // js/components/ServerStatus.tsx
-    var import_react23 = __toESM(require_react());
+    var import_react22 = __toESM(require_react());
 
     function ServerStatus() {
-        let [state, setState] = (0, import_react23.useState)({
+        let [state, setState] = (0, import_react22.useState)({
             serverIsUp: !0,
             projectId: null
         });
-        return (0, import_react23.useEffect)(() => {
+        return (0, import_react22.useEffect)(() => {
             let onInterval = () => {
                     get("/ping", null).then(
                         ({
                             project_id
                         }) => {
                             setState(
                                 ({
@@ -11030,75 +13274,75 @@
                                 serverIsUp: !1
                             }));
                         }
                     );
                 },
                 id = window.setInterval(onInterval, 2e3);
             return () => window.clearInterval(id);
-        }, []), state.serverIsUp ? null : /* @__PURE__ */ import_react23.default.createElement("div", {
+        }, []), state.serverIsUp ? null : /* @__PURE__ */ import_react22.default.createElement("div", {
             className: "interface-protector server-down-panel"
-        }, /* @__PURE__ */ import_react23.default.createElement("div", {
+        }, /* @__PURE__ */ import_react22.default.createElement("div", {
             className: "server-down-dialog"
-        }, /* @__PURE__ */ import_react23.default.createElement("h3", null, trans("ERROR_SERVER_UNAVAILABLE")), /* @__PURE__ */ import_react23.default.createElement("p", null, trans("ERROR_SERVER_UNAVAILABLE_MESSAGE"))));
+        }, /* @__PURE__ */ import_react22.default.createElement("h3", null, trans("ERROR_SERVER_UNAVAILABLE")), /* @__PURE__ */ import_react22.default.createElement("p", null, trans("ERROR_SERVER_UNAVAILABLE_MESSAGE"))));
     }
 
     // js/components/ErrorDialog.tsx
-    var import_react24 = __toESM(require_react());
+    var import_react23 = __toESM(require_react());
 
     function ErrorDialog() {
-        let [error, setError] = (0, import_react24.useState)(null), dismiss = (0, import_react24.useCallback)(() => setError(null), []);
-        return (0, import_react24.useEffect)(() => {
+        let [error, setError] = (0, import_react23.useState)(null), dismiss = (0, import_react23.useCallback)(() => setError(null), []);
+        return (0, import_react23.useEffect)(() => {
             let handler = ({
                 detail
             }) => setError(detail);
             return subscribe("lektor-error", handler), () => unsubscribe("lektor-error", handler);
-        }, []), error ? /* @__PURE__ */ import_react24.default.createElement(
+        }, []), error ? /* @__PURE__ */ import_react23.default.createElement(
             SlideDialog, {
                 dismiss,
                 hasCloseButton: !1,
                 title: trans("ERROR")
             },
             /* @__PURE__ */
-            import_react24.default.createElement("p", null, trans("ERROR_OCURRED"), ": ", trans("ERROR_" + error.code)),
+            import_react23.default.createElement("p", null, trans("ERROR_OCURRED"), ": ", trans("ERROR_" + error.code)),
             /* @__PURE__ */
-            import_react24.default.createElement("p", null, /* @__PURE__ */ import_react24.default.createElement("button", {
+            import_react23.default.createElement("p", null, /* @__PURE__ */ import_react23.default.createElement("button", {
                 type: "button",
                 className: "btn btn-primary",
                 onClick: dismiss
             }, trans("CLOSE")))
         ) : null;
     }
 
     // js/views/edit/EditPage.tsx
     var import_react44 = __toESM(require_react());
 
     // js/widgets.tsx
-    var import_react41 = __toESM(require_react());
+    var import_react40 = __toESM(require_react());
 
     // js/widgets/IntegerInputWidget.tsx
-    var import_react27 = __toESM(require_react());
+    var import_react26 = __toESM(require_react());
 
     // js/widgets/InputWidgetBase.tsx
-    var import_react26 = __toESM(require_react());
+    var import_react25 = __toESM(require_react());
 
     // js/userLabel.tsx
-    var import_react25 = __toESM(require_react());
+    var import_react24 = __toESM(require_react());
 
     function formatUserLabel(inputConfig) {
         let label = typeof inputConfig == "string" ? inputConfig : trans_obj(inputConfig);
         if (!label)
-            return /* @__PURE__ */ import_react25.default.createElement("span", null);
+            return /* @__PURE__ */ import_react24.default.createElement("span", null);
         let iconData = label.match(/^\[\[\s*(.*?)\s*(;\s*(.*?))?\s*\]\]$/);
         if (iconData) {
             let className = "fa fa-" + iconData[1];
-            return (iconData[3] || "").match(/90|180|270/) && (className += " fa-rotate-" + iconData[3]), /* @__PURE__ */ import_react25.default.createElement("i", {
+            return (iconData[3] || "").match(/90|180|270/) && (className += " fa-rotate-" + iconData[3]), /* @__PURE__ */ import_react24.default.createElement("i", {
                 className
             });
         }
-        return /* @__PURE__ */ import_react25.default.createElement("span", null, label);
+        return /* @__PURE__ */ import_react24.default.createElement("span", null, label);
     }
 
     // js/widgets/types.ts
     function getInputClass(type) {
         return type.size === "small" ? "form-control form-control-sm" : type.size === "large" ? "form-control form-control-lg" : "form-control";
     }
 
@@ -11110,77 +13354,88 @@
         postprocessValue,
         inputAddon: inputAddon5,
         inputType,
         validate,
         disabled,
         placeholder
     }) {
-        let onChangeHandler = (0, import_react26.useCallback)(
+        let onChangeHandler = (0, import_react25.useCallback)(
                 (event) => {
                     let value2 = event.target.value;
                     postprocessValue && (value2 = postprocessValue(value2)), onChange(value2);
                 },
                 [onChange, postprocessValue]
             ),
             failure = validate ? validate(value) : null,
             setValidity = (el) => {
                 el == null || el.setCustomValidity(failure != null ? failure : "");
             },
             configuredAddon = type.addon_label_i18n,
             addon = configuredAddon ? formatUserLabel(configuredAddon) : inputAddon5;
-        return /* @__PURE__ */ import_react26.default.createElement(import_react26.default.Fragment, null, /* @__PURE__ */ import_react26.default.createElement("div", {
+        return /* @__PURE__ */ import_react25.default.createElement(import_react25.default.Fragment, null, /* @__PURE__ */ import_react25.default.createElement("div", {
             className: "input-group"
-        }, /* @__PURE__ */ import_react26.default.createElement(
+        }, /* @__PURE__ */ import_react25.default.createElement(
             "input", {
                 ref: setValidity,
                 type: inputType,
                 disabled,
                 placeholder,
                 className: getInputClass(type),
                 onChange: onChangeHandler,
                 value: value || ""
             }
-        ), /* @__PURE__ */ import_react26.default.createElement("span", {
+        ), /* @__PURE__ */ import_react25.default.createElement("span", {
             className: "input-group-text"
-        }, addon)), failure !== null && /* @__PURE__ */ import_react26.default.createElement("div", {
+        }, addon)), failure !== null && /* @__PURE__ */ import_react25.default.createElement("div", {
             className: "validation-block validation-block-error"
         }, failure));
     }
 
     // js/widgets/IntegerInputWidget.tsx
     function postprocessInteger(value) {
         return value.trim();
     }
 
     function validateInteger(value) {
         return value && !value.match(/^-?\d+$/) ? trans("ERROR_INVALID_NUMBER") : null;
     }
 
     function IntegerInputWidget(props) {
-        return /* @__PURE__ */ import_react27.default.createElement(
+        return /* @__PURE__ */ import_react26.default.createElement(
             InputWidgetBase,
             __spreadValues({
                 inputType: "text",
                 inputAddon: "0",
                 postprocessValue: postprocessInteger,
                 validate: validateInteger
             }, props)
         );
     }
 
     // js/widgets/MultiLineTextInputWidget.tsx
-    var import_react28 = __toESM(require_react());
+    var import_react27 = __toESM(require_react());
     var config = {
+        // On initial render, if the natural height of the textarea is less than
+        // than maxInitialHeight, the textarea will start in autosize mode.
+        // Otherwise, it will start with a static height of defaultStaticHeight.
+        // (Both of these are relative to windowHeight.)
         maxInitialHeight: 0.6,
         defaultStaticHeight: 0.4,
+        // The maximum target height for the "shrink" button, relative to windowHeight.
         maxTargetHeight: 0.8,
+        // The minimum target height for the "shrink" button, in lines.
         minTargetLines: 5,
+        // Default shrink factor, if remembered height is not viable
         fallbackShrinkFactor: 0.5,
+        // When textarea is manually resized, if the new size larger than the
+        // largest of (extraLines * lineHeight) or (maxResizeHeight * windowHeight),
+        // the textarea will be switched to autosize mode.
         extraLines: 2,
         maxResizeHeight: 0.8,
+        // When window is narrower than this, textareas are always autosized
         minWindowWidth: 576
     };
 
     function _pixels(dimension) {
         return Number(dimension.replace(/px/, ""));
     }
 
@@ -11274,18 +13529,18 @@
     function MultiLineTextInputWidget({
         type,
         value,
         placeholder,
         disabled,
         onChange: onChangeProp
     }) {
-        let textareaRef = (0, import_react28.useRef)(null),
-            replicaRef = (0, import_react28.useRef)(null),
-            [state, dispatch2] = (0, import_react28.useReducer)(reduceState, null, initState);
-        (0, import_react28.useEffect)(() => {
+        let textareaRef = (0, import_react27.useRef)(null),
+            replicaRef = (0, import_react27.useRef)(null),
+            [state, dispatch2] = (0, import_react27.useReducer)(reduceState, null, initState);
+        (0, import_react27.useEffect)(() => {
             let textarea = deref(textareaRef),
                 replica = deref(replicaRef);
             dispatch2({
                 type: "initialize",
                 textarea,
                 replica
             });
@@ -11297,15 +13552,15 @@
                 });
             };
             window.addEventListener("resize", windowResizeListener);
             let disconnectResizeWatcher = textareaResizeWatcher(textarea);
             return () => {
                 disconnectResizeWatcher(), window.removeEventListener("resize", windowResizeListener);
             };
-        }, []), (0, import_react28.useEffect)(() => {
+        }, []), (0, import_react27.useEffect)(() => {
             if (state.resizeable) {
                 let textarea = deref(textareaRef),
                     replica = deref(replicaRef),
                     observer = new MutationObserver(() => {
                         textarea.style.height && (replica.style.maxHeight = "0px");
                     });
                 observer.observe(textarea, {
@@ -11325,40 +13580,40 @@
                 };
             }
         }, [state.resizeable]);
         let getNaturalHeight = () => {
             let replica = replicaRef.current;
             return replica ? (replica.innerText = value, replica.scrollHeight + state.borderHeight) : 0;
         };
-        (0, import_react28.useEffect)(() => {
+        (0, import_react27.useEffect)(() => {
             if (!state.autosized) {
                 let reasonableHeight = Math.max(
                     getNaturalHeight() + state.lineHeight * config.extraLines,
                     window.innerHeight * config.maxResizeHeight
                 );
                 state.height > reasonableHeight && dispatch2({
                     type: "autosize"
                 });
             }
         });
         let onChange = (event) => {
             onChangeProp(event.target.value);
         };
-        return /* @__PURE__ */ import_react28.default.createElement("div", {
+        return /* @__PURE__ */ import_react27.default.createElement("div", {
             className: "text-widget"
-        }, /* @__PURE__ */ import_react28.default.createElement(
+        }, /* @__PURE__ */ import_react27.default.createElement(
             "div", {
                 style: {
                     maxHeight: state.autosized ? "" : "0px"
                 },
                 ref: replicaRef,
                 className: "text-widget__replica"
             },
             value
-        ), /* @__PURE__ */ import_react28.default.createElement(
+        ), /* @__PURE__ */ import_react27.default.createElement(
             "textarea", {
                 style: {
                     height: state.autosized ? "" : `${state.height}px`
                 },
                 ref: textareaRef,
                 className: [
                     "text-widget__textarea",
@@ -11367,15 +13622,15 @@
                     getInputClass(type)
                 ].filter(Boolean).join(" "),
                 onChange,
                 value,
                 disabled,
                 placeholder
             }
-        ), /* @__PURE__ */ import_react28.default.createElement(
+        ), /* @__PURE__ */ import_react27.default.createElement(
             ToggleButton, {
                 state,
                 dispatch: dispatch2,
                 naturalHeight: getNaturalHeight()
             }
         ));
     }
@@ -11390,20 +13645,20 @@
             return null;
         let {
             title,
             icon
         } = toggleButtonLabels[action.type], onClick = (event) => {
             event.preventDefault(), dispatch2(action);
         }, className = "position-absolute top-0 start-100 translate-middle bg-light border rounded-circle";
-        return /* @__PURE__ */ import_react28.default.createElement("a", {
+        return /* @__PURE__ */ import_react27.default.createElement("a", {
             href: "#",
             title: trans(title),
             onClick,
             className
-        }, /* @__PURE__ */ import_react28.default.createElement("i", {
+        }, /* @__PURE__ */ import_react27.default.createElement("i", {
             className: `fa fa-${icon} fa-fw`
         }));
     }
     var toggleButtonLabels = {
         autosize: {
             title: "AUTOSIZE_TEXTAREA",
             icon: "expand"
@@ -11419,14 +13674,15 @@
             return null;
         if (!state.autosized)
             return {
                 type: "autosize"
             };
         let targetHeight = Math.min(
             state.height,
+            // last manually set height
             Math.ceil(window.innerHeight * config.maxTargetHeight)
         );
         if (targetHeight < naturalHeight)
             return {
                 type: "set-height",
                 height: targetHeight
             };
@@ -11443,30 +13699,30 @@
         return fallbackHeight < naturalHeight ? {
             type: "set-height",
             height: fallbackHeight
         } : null;
     }
 
     // js/widgets/BooleanInputWidget.tsx
-    var import_react29 = __toESM(require_react());
+    var import_react28 = __toESM(require_react());
     var isTrue = (value) => value === "true" || value === "yes" || value === "1",
         isDeleteOrBackspace = (event) => event.altKey || event.metaKey || event.shiftKey && !event.ctrlKey ? !1 : event.key === "Delete" || event.key === "Backspace";
 
     function BooleanInputWidget({
         type,
         value,
         disabled,
         placeholder,
         onChange
     }) {
-        return /* @__PURE__ */ import_react29.default.createElement("div", {
+        return /* @__PURE__ */ import_react28.default.createElement("div", {
             className: "form-check"
-        }, /* @__PURE__ */ import_react29.default.createElement("label", {
+        }, /* @__PURE__ */ import_react28.default.createElement("label", {
             className: "form-check-label"
-        }, /* @__PURE__ */ import_react29.default.createElement(
+        }, /* @__PURE__ */ import_react28.default.createElement(
             "input", {
                 type: "checkbox",
                 className: [
                     "form-check-input",
                     `form-check-input--default-${placeholder ? "true" : "false"}`
                 ].join(" "),
                 disabled,
@@ -11482,15 +13738,15 @@
                 },
                 title: trans("TRISTATE_CHECKBOX_TOOLTIP")
             }
         ), type.checkbox_label_i18n ? trans_obj(type.checkbox_label_i18n) : null));
     }
 
     // js/widgets/DateInputWidget.tsx
-    var import_react30 = __toESM(require_react());
+    var import_react29 = __toESM(require_react());
     var parseInteger = (s) => Number.parseInt(s, 10);
 
     function isValidDate(year, month, day) {
         let date = new Date(year, month - 1, day);
         return date.getFullYear() === year && date.getMonth() === month - 1 && date.getDate() === day;
     }
     var DATE_RE = new RegExp("^\\s*(?<year>\\d{4})-(?<month>\\d{1,2})-(?<day>\\d{1,2})\\s*$");
@@ -11516,110 +13772,110 @@
         if (groups) {
             let day = parseInteger(groups.day),
                 month = parseInteger(groups.month);
             return `${parseInteger(groups.year)}-${pad(month)}-${pad(day)}`;
         }
         return value;
     }
-    var inputAddon = /* @__PURE__ */ import_react30.default.createElement("i", {
+    var inputAddon = /* @__PURE__ */ import_react29.default.createElement("i", {
         className: "fa fa-calendar"
     });
 
     function DateInputWidget(props) {
-        return /* @__PURE__ */ import_react30.default.createElement(
+        return /* @__PURE__ */ import_react29.default.createElement(
             InputWidgetBase,
             __spreadValues({
                 inputType: "date",
                 inputAddon,
                 postprocessValue: postprocessDate,
                 validate: validateDate
             }, props)
         );
     }
 
     // js/widgets/FloatInputWidget.tsx
-    var import_react31 = __toESM(require_react());
+    var import_react30 = __toESM(require_react());
 
     function postprocessFloat(value) {
         return value.trim();
     }
 
     function validateFloat(value) {
         return value && !value.match(/^[+,-]?\d+[.]\d+$/) ? trans("ERROR_INVALID_NUMBER") : null;
     }
 
     function FloatInputWidget(props) {
-        return /* @__PURE__ */ import_react31.default.createElement(
+        return /* @__PURE__ */ import_react30.default.createElement(
             InputWidgetBase,
             __spreadValues({
                 inputType: "text",
                 inputAddon: "0.0",
                 postprocessValue: postprocessFloat,
                 validate: validateFloat
             }, props)
         );
     }
 
     // js/widgets/UrlInputWidget.tsx
-    var import_react32 = __toESM(require_react());
+    var import_react31 = __toESM(require_react());
 
     function validateUrl(value) {
         return value && !isValidUrl(value) ? trans("ERROR_INVALID_URL") : null;
     }
-    var inputAddon2 = /* @__PURE__ */ import_react32.default.createElement("i", {
+    var inputAddon2 = /* @__PURE__ */ import_react31.default.createElement("i", {
         className: "fa fa-external-link"
     });
 
     function UrlInputWidget(props) {
-        return /* @__PURE__ */ import_react32.default.createElement(
+        return /* @__PURE__ */ import_react31.default.createElement(
             InputWidgetBase,
             __spreadValues({
                 inputType: "text",
                 inputAddon: inputAddon2,
                 validate: validateUrl
             }, props)
         );
     }
 
     // js/widgets/SlugInputWidget.tsx
-    var import_react33 = __toESM(require_react());
+    var import_react32 = __toESM(require_react());
 
     function postprocessSlug(value) {
         return value.replace(/\s+/g, "-");
     }
-    var inputAddon3 = /* @__PURE__ */ import_react33.default.createElement("i", {
+    var inputAddon3 = /* @__PURE__ */ import_react32.default.createElement("i", {
         className: "fa fa-link"
     });
 
     function SlugInputWidget(props) {
-        return /* @__PURE__ */ import_react33.default.createElement(
+        return /* @__PURE__ */ import_react32.default.createElement(
             InputWidgetBase,
             __spreadValues({
                 inputType: "text",
                 inputAddon: inputAddon3,
                 postprocessValue: postprocessSlug
             }, props)
         );
     }
 
     // js/widgets/SingleLineTextInputWidget.tsx
-    var import_react34 = __toESM(require_react());
-    var inputAddon4 = /* @__PURE__ */ import_react34.default.createElement("i", {
+    var import_react33 = __toESM(require_react());
+    var inputAddon4 = /* @__PURE__ */ import_react33.default.createElement("i", {
         className: "fa fa-paragraph"
     });
 
     function SingleLineTextInputWidget(props) {
-        return /* @__PURE__ */ import_react34.default.createElement(InputWidgetBase, __spreadValues({
+        return /* @__PURE__ */ import_react33.default.createElement(InputWidgetBase, __spreadValues({
             inputType: "text",
             inputAddon: inputAddon4
         }, props));
     }
 
     // js/widgets/CheckboxesInputWidget.tsx
-    var import_react35 = __toESM(require_react());
+    var import_react34 = __toESM(require_react());
     var checkboxIsActive = (field, value) => value !== null && value.includes(field),
         flipSetValue = (set, value, isActive) => isActive ? set.includes(value) ? set : [...set, value] : set.filter((v) => v !== value),
         deserialize = (value) => {
             if (!value)
                 return null;
             let rv = value.split(",").map((x) => x.trim());
             return rv.length === 1 && rv[0] === "" && (rv = []), rv;
@@ -11631,22 +13887,22 @@
         onChange,
         value,
         placeholder
     }) {
         var _a2;
         let deserializedValue = deserialize(value),
             deserializedPlaceholder = deserialize(placeholder);
-        return /* @__PURE__ */ import_react35.default.createElement("div", {
+        return /* @__PURE__ */ import_react34.default.createElement("div", {
             className: "checkboxes-widget"
-        }, (_a2 = type.choices) == null ? void 0 : _a2.map(([key, description]) => /* @__PURE__ */ import_react35.default.createElement("div", {
+        }, (_a2 = type.choices) == null ? void 0 : _a2.map(([key, description]) => /* @__PURE__ */ import_react34.default.createElement("div", {
             className: "form-check",
             key
-        }, /* @__PURE__ */ import_react35.default.createElement("label", {
+        }, /* @__PURE__ */ import_react34.default.createElement("label", {
             className: "form-check-label"
-        }, /* @__PURE__ */ import_react35.default.createElement(
+        }, /* @__PURE__ */ import_react34.default.createElement(
             "input", {
                 className: "form-check-input",
                 type: "checkbox",
                 disabled,
                 checked: checkboxIsActive(
                     key,
                     deserializedValue != null ? deserializedValue : deserializedPlaceholder
@@ -11660,46 +13916,46 @@
                     onChange(newValue.join(", "));
                 }
             }
         ), trans_obj(description)))));
     }
 
     // js/widgets/SelectInputWidget.tsx
-    var import_react36 = __toESM(require_react());
+    var import_react35 = __toESM(require_react());
 
     function SelectInputWidget(props) {
         var _a2;
         let {
             type,
             value,
             placeholder,
             onChange,
             disabled
-        } = props, choices = (_a2 = type.choices) == null ? void 0 : _a2.map((item) => /* @__PURE__ */ import_react36.default.createElement("option", {
+        } = props, choices = (_a2 = type.choices) == null ? void 0 : _a2.map((item) => /* @__PURE__ */ import_react35.default.createElement("option", {
             key: item[0],
             value: item[0]
         }, trans_obj(item[1])));
-        return /* @__PURE__ */ import_react36.default.createElement("div", null, /* @__PURE__ */ import_react36.default.createElement(
+        return /* @__PURE__ */ import_react35.default.createElement("div", null, /* @__PURE__ */ import_react35.default.createElement(
             "select", {
                 className: getInputClass(type),
                 value: value || placeholder || "",
                 onChange: (e) => onChange(e.target.value),
                 disabled
             },
             /* @__PURE__ */
-            import_react36.default.createElement("option", {
+            import_react35.default.createElement("option", {
                 key: "",
                 value: ""
             }, "----"),
             choices
         ));
     }
 
     // js/widgets/flow/FlowWidget.tsx
-    var import_react39 = __toESM(require_react());
+    var import_react38 = __toESM(require_react());
 
     // js/widgets/flow/metaformat.tsx
     function lineIsDashes(rawLine) {
         let line = rawLine.trim();
         return line.length >= 3 && line.match(/[^-]/) === null;
     }
 
@@ -11768,102 +14024,102 @@
             } else
                 rv.push(key + ": " + value + `
 `);
         }), rv;
     }
 
     // js/widgets/flow/FlowBlock.tsx
-    var import_react37 = __toESM(require_react());
-    var FlowBlock_default = (0, import_react37.memo)(function({
+    var import_react36 = __toESM(require_react());
+    var FlowBlock_default = (0, import_react36.memo)(function({
         block,
         moveBlock,
         renderFormField,
         removeBlock,
         idx,
         length
     }) {
-        let [collapsed, toggle] = (0, import_react37.useReducer)((s) => !s, !1);
-        return /* @__PURE__ */ import_react37.default.createElement("div", {
+        let [collapsed, toggle] = (0, import_react36.useReducer)((s) => !s, !1);
+        return /* @__PURE__ */ import_react36.default.createElement("div", {
             className: "flow-block"
-        }, /* @__PURE__ */ import_react37.default.createElement("div", {
+        }, /* @__PURE__ */ import_react36.default.createElement("div", {
             className: "d-flex justify-content-between"
-        }, /* @__PURE__ */ import_react37.default.createElement("h4", {
+        }, /* @__PURE__ */ import_react36.default.createElement("h4", {
             className: "block-name"
-        }, formatUserLabel(block.model.name_i18n)), /* @__PURE__ */ import_react37.default.createElement("div", {
+        }, formatUserLabel(block.model.name_i18n)), /* @__PURE__ */ import_react36.default.createElement("div", {
             className: "btn-group action-bar"
-        }, /* @__PURE__ */ import_react37.default.createElement(
+        }, /* @__PURE__ */ import_react36.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary btn-sm border",
                 title: collapsed ? trans("EXPAND") : trans("COLLAPSE"),
                 onClick: toggle
             },
             /* @__PURE__ */
-            import_react37.default.createElement("i", {
+            import_react36.default.createElement("i", {
                 className: collapsed ? "fa fa-expand" : "fa fa-compress"
             })
-        ), /* @__PURE__ */ import_react37.default.createElement(
+        ), /* @__PURE__ */ import_react36.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary btn-sm border",
                 title: trans("UP"),
                 disabled: idx === 0,
                 onClick: () => moveBlock(idx, -1)
             },
             /* @__PURE__ */
-            import_react37.default.createElement("i", {
+            import_react36.default.createElement("i", {
                 className: "fa fa-fw fa-chevron-up"
             })
-        ), /* @__PURE__ */ import_react37.default.createElement(
+        ), /* @__PURE__ */ import_react36.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary btn-sm border",
                 title: trans("DOWN"),
                 disabled: idx === length - 1,
                 onClick: () => moveBlock(idx, 1)
             },
             /* @__PURE__ */
-            import_react37.default.createElement("i", {
+            import_react36.default.createElement("i", {
                 className: "fa fa-fw fa-chevron-down"
             })
-        ), /* @__PURE__ */ import_react37.default.createElement(
+        ), /* @__PURE__ */ import_react36.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary btn-sm border",
                 title: trans("REMOVE"),
                 onClick: () => removeBlock(idx)
             },
             /* @__PURE__ */
-            import_react37.default.createElement("i", {
+            import_react36.default.createElement("i", {
                 className: "fa fa-fw fa-times"
             })
-        ))), collapsed ? null : /* @__PURE__ */ import_react37.default.createElement(
+        ))), collapsed ? null : /* @__PURE__ */ import_react36.default.createElement(
             FieldRows, {
                 fields: block.model.fields,
                 renderFunc: renderFormField.bind(void 0, block)
             }
         ));
     });
 
     // js/widgets/flow/AddFlowBlockButtons.tsx
-    var import_react38 = __toESM(require_react());
+    var import_react37 = __toESM(require_react());
 
     function AddFlowBlockButtons({
         flowblock_order,
         flowblocks,
         addBlock
     }) {
         let models = flowblock_order.map((key) => flowblocks[key]);
-        return /* @__PURE__ */ import_react38.default.createElement("div", {
+        return /* @__PURE__ */ import_react37.default.createElement("div", {
             className: "add-flow-block"
-        }, /* @__PURE__ */ import_react38.default.createElement("label", null, `${trans("ADD_FLOWBLOCK")}: `), /* @__PURE__ */ import_react38.default.createElement("div", {
+        }, /* @__PURE__ */ import_react37.default.createElement("label", null, `${trans("ADD_FLOWBLOCK")}: `), /* @__PURE__ */ import_react37.default.createElement("div", {
             className: "btn-group"
         }, models.map((model) => {
             let label = model.button_label ? formatUserLabel(model.button_label) : formatUserLabel(model.name_i18n);
-            return /* @__PURE__ */ import_react38.default.createElement(
+            return /* @__PURE__ */ import_react37.default.createElement(
                 "button", {
                     type: "button",
                     className: "btn btn-secondary border",
                     onClick: () => addBlock(model),
                     title: trans_obj(model.name_i18n),
                     key: model.id
                 },
@@ -11935,43 +14191,43 @@
         }), serialize(rv);
     }
 
     function FlowWidget(props) {
         let {
             value,
             onChange
-        } = props, moveBlock = (0, import_react39.useCallback)(
+        } = props, moveBlock = (0, import_react38.useCallback)(
             (idx, offset) => {
                 onChange((prevValue) => {
                     let newIndex = idx + offset;
                     if (newIndex < 0 || newIndex >= prevValue.length)
                         return prevValue;
                     let newValue = [...prevValue];
                     return newValue[newIndex] = prevValue[idx], newValue[idx] = prevValue[newIndex], newValue;
                 });
             },
             [onChange]
-        ), removeBlock = (0, import_react39.useCallback)(
+        ), removeBlock = (0, import_react38.useCallback)(
             (idx) => {
                 confirm(trans("REMOVE_FLOWBLOCK_PROMPT")) && onChange((v) => v.filter((item, i) => i !== idx));
             },
             [onChange]
-        ), addNewBlock = (0, import_react39.useCallback)(
+        ), addNewBlock = (0, import_react38.useCallback)(
             (flowBlockModel) => {
                 onChange((prevValue) => {
                     prevValue != null || (prevValue = []);
                     let newBlockId = Math.max(0, ...prevValue.map(({
                             localId
                         }) => localId)) + 1,
                         newBlock = deserializeFlowBlock(flowBlockModel, [], newBlockId);
                     return [...prevValue, newBlock];
                 });
             },
             [onChange]
-        ), renderFormField = (0, import_react39.useCallback)(
+        ), renderFormField = (0, import_react38.useCallback)(
             (block, field) => {
                 let fieldValue = block.data[field.name],
                     placeholder = field.default,
                     Widget = getWidgetComponentWithFallback(field.type);
                 Widget.deserializeValue && placeholder != null && (placeholder = Widget.deserializeValue(placeholder, field.type));
                 let setFieldValue = (fieldName, v) => {
                     onChange((prevValue) => {
@@ -11981,42 +14237,42 @@
                                 [fieldName]: typeof v == "function" ? v(block.data[fieldName]) : v
                             });
                         return newValue[idx] = __spreadProps(__spreadValues({}, block), {
                             data
                         }), newValue;
                     });
                 };
-                return /* @__PURE__ */ import_react39.default.createElement(
+                return /* @__PURE__ */ import_react38.default.createElement(
                     FieldBox, {
                         key: field.name,
                         value: fieldValue,
                         placeholder,
                         field,
                         setFieldValue
                     }
                 );
             },
             [onChange]
         ), {
             flowblock_order,
             flowblocks
         } = props.type;
-        return /* @__PURE__ */ import_react39.default.createElement("div", {
+        return /* @__PURE__ */ import_react38.default.createElement("div", {
             className: "flow-widget"
-        }, value.map((block, idx) => /* @__PURE__ */ import_react39.default.createElement(
+        }, value.map((block, idx) => /* @__PURE__ */ import_react38.default.createElement(
             FlowBlock_default, {
                 key: block.localId,
                 block,
                 moveBlock,
                 renderFormField,
                 removeBlock,
                 length: value.length,
                 idx
             }
-        )), /* @__PURE__ */ import_react39.default.createElement(
+        )), /* @__PURE__ */ import_react38.default.createElement(
             AddFlowBlockButtons, {
                 flowblock_order,
                 flowblocks,
                 addBlock: addNewBlock
             }
         ));
     }
@@ -12037,39 +14293,39 @@
         }) => [
             flowBlockModel.id,
             serializeFlowBlock(flowBlockModel, data)
         ])
     );
 
     // js/widgets/fakeWidgets.tsx
-    var import_react40 = __toESM(require_react());
+    var import_react39 = __toESM(require_react());
 
     function LineWidget() {
-        return /* @__PURE__ */ import_react40.default.createElement("hr", null);
+        return /* @__PURE__ */ import_react39.default.createElement("hr", null);
     }
     LineWidget.isFakeWidget = !0;
 
     function SpacingWidget() {
-        return /* @__PURE__ */ import_react40.default.createElement("div", {
+        return /* @__PURE__ */ import_react39.default.createElement("div", {
             className: "spacing-widget"
         });
     }
     SpacingWidget.isFakeWidget = !0;
 
     function InfoWidget(props) {
         let label = trans_obj(props.field.label_i18n);
-        return /* @__PURE__ */ import_react40.default.createElement("div", {
+        return /* @__PURE__ */ import_react39.default.createElement("div", {
             className: "info-widget"
-        }, /* @__PURE__ */ import_react40.default.createElement("p", null, label ? /* @__PURE__ */ import_react40.default.createElement("strong", null, label + ": ") : null, trans_obj(props.field.description_i18n)));
+        }, /* @__PURE__ */ import_react39.default.createElement("p", null, label ? /* @__PURE__ */ import_react39.default.createElement("strong", null, label + ": ") : null, trans_obj(props.field.description_i18n)));
     }
     InfoWidget.isFakeWidget = !0;
 
     function HeadingWidget(props) {
         var _a2;
-        return /* @__PURE__ */ import_react40.default.createElement("h3", null, trans_obj((_a2 = props.field.type.heading_i18n) != null ? _a2 : {}));
+        return /* @__PURE__ */ import_react39.default.createElement("h3", null, trans_obj((_a2 = props.field.type.heading_i18n) != null ? _a2 : {}));
     }
     HeadingWidget.isFakeWidget = !0;
 
     // js/widgets.tsx
     var widgetComponents = {
         "singleline-text": SingleLineTextInputWidget,
         "multiline-text": MultiLineTextInputWidget,
@@ -12085,44 +14341,44 @@
         "f-line": LineWidget,
         "f-spacing": SpacingWidget,
         "f-info": InfoWidget,
         "f-heading": HeadingWidget
     };
 
     function FallbackWidget(props) {
-        return /* @__PURE__ */ import_react41.default.createElement("div", null, /* @__PURE__ */ import_react41.default.createElement("em", null, `Widget "${props.type.widget}" not implemented`, ` (used by type "${props.type.name}")`));
+        return /* @__PURE__ */ import_react40.default.createElement("div", null, /* @__PURE__ */ import_react40.default.createElement("em", null, `Widget "${props.type.widget}" not implemented`, ` (used by type "${props.type.name}")`));
     }
-    var FieldBox = import_react41.default.memo(function(props) {
+    var FieldBox = import_react40.default.memo(function(props) {
         let {
             field,
             value,
             placeholder,
             disabled,
             setFieldValue
-        } = props, onChange = (0, import_react41.useCallback)(
+        } = props, onChange = (0, import_react40.useCallback)(
             (value2) => setFieldValue(field.name, value2),
             [field, setFieldValue]
         ), className = `col-md-${getFieldColumns(field)}`, Widget = getWidgetComponentWithFallback(field.type);
         if (Widget.isFakeWidget)
-            return /* @__PURE__ */ import_react41.default.createElement("div", {
+            return /* @__PURE__ */ import_react40.default.createElement("div", {
                 className,
                 key: field.name
-            }, /* @__PURE__ */ import_react41.default.createElement(Widget, {
+            }, /* @__PURE__ */ import_react40.default.createElement(Widget, {
                 key: field.name,
                 field
             }));
-        let description = field.description_i18n ? /* @__PURE__ */ import_react41.default.createElement("div", {
+        let description = field.description_i18n ? /* @__PURE__ */ import_react40.default.createElement("div", {
             className: "help-text"
         }, trans_obj(field.description_i18n)) : null;
-        return /* @__PURE__ */ import_react41.default.createElement("div", {
+        return /* @__PURE__ */ import_react40.default.createElement("div", {
             className,
             key: field.name
-        }, /* @__PURE__ */ import_react41.default.createElement("dl", {
+        }, /* @__PURE__ */ import_react40.default.createElement("dl", {
             className: "field"
-        }, field.hide_label ? null : /* @__PURE__ */ import_react41.default.createElement("dt", null, trans_obj(field.label_i18n)), /* @__PURE__ */ import_react41.default.createElement("dd", null, description, /* @__PURE__ */ import_react41.default.createElement(
+        }, field.hide_label ? null : /* @__PURE__ */ import_react40.default.createElement("dt", null, trans_obj(field.label_i18n)), /* @__PURE__ */ import_react40.default.createElement("dd", null, description, /* @__PURE__ */ import_react40.default.createElement(
             Widget, {
                 value,
                 onChange,
                 type: field.type,
                 placeholder: placeholder != null ? placeholder : void 0,
                 disabled
             }
@@ -12161,80 +14417,117 @@
         }), [normalFields, systemFields];
     }
 
     function FieldRows({
         fields,
         renderFunc
     }) {
-        let rows = (0, import_react41.useMemo)(() => processFields(fields), [fields]);
-        return /* @__PURE__ */ import_react41.default.createElement(import_react41.default.Fragment, null, rows.map((row, idx) => /* @__PURE__ */ import_react41.default.createElement("div", {
+        let rows = (0, import_react40.useMemo)(() => processFields(fields), [fields]);
+        return /* @__PURE__ */ import_react40.default.createElement(import_react40.default.Fragment, null, rows.map((row, idx) => /* @__PURE__ */ import_react40.default.createElement("div", {
             key: idx,
             className: "row field-row"
         }, row.map(renderFunc))));
     }
 
     // js/views/edit/EditPageActions.tsx
-    var import_react42 = __toESM(require_react());
+    var import_react41 = __toESM(require_react());
 
     function EditPageActions({
         recordInfo,
         hasPendingChanges
     }) {
         let {
             path,
             alt
-        } = useRecord(), goToAdminPage = useGoToAdminPage(), deleteRecord = (0, import_react42.useCallback)(() => {
+        } = useRecord(), goToAdminPage = useGoToAdminPage(), deleteRecord = (0, import_react41.useCallback)(() => {
             goToAdminPage("delete", path, alt);
         }, [alt, goToAdminPage, path]);
-        return /* @__PURE__ */ import_react42.default.createElement("div", {
+        return /* @__PURE__ */ import_react41.default.createElement("div", {
             className: "actions"
-        }, /* @__PURE__ */ import_react42.default.createElement(
+        }, /* @__PURE__ */ import_react41.default.createElement(
             "button", {
                 type: "submit",
                 disabled: !hasPendingChanges,
                 className: "btn btn-primary"
             },
             trans("SAVE_CHANGES")
-        ), recordInfo.can_be_deleted ? /* @__PURE__ */ import_react42.default.createElement(
+        ), recordInfo.can_be_deleted ? /* @__PURE__ */ import_react41.default.createElement(
             "button", {
                 type: "button",
                 className: "btn btn-secondary border",
                 onClick: deleteRecord
             },
             trans("DELETE")
         ) : null);
     }
 
     // js/components/ToggleGroup.tsx
-    var import_react43 = __toESM(require_react());
+    var import_react42 = __toESM(require_react());
 
     function ToggleGroup({
         className = "",
         groupTitle,
         children
     }) {
-        let [open, setOpen] = (0, import_react43.useState)(!1), toggle = (0, import_react43.useCallback)((event) => {
+        let [open, setOpen] = (0, import_react42.useState)(!1), toggle = (0, import_react42.useCallback)((event) => {
             event.preventDefault(), setOpen((v) => !v);
         }, []);
-        return /* @__PURE__ */ import_react43.default.createElement(
+        return /* @__PURE__ */ import_react42.default.createElement(
             "div", {
                 className: open ? `${className} toggle-group` : `${className} toggle-group closed`
             },
             /* @__PURE__ */
-            import_react43.default.createElement("h4", {
+            import_react42.default.createElement("h4", {
                 className: "toggle-group-header",
                 onClick: toggle
             }, groupTitle),
             /* @__PURE__ */
-            import_react43.default.createElement("div", {
+            import_react42.default.createElement("div", {
                 className: "toggle-group-content"
             }, children)
         );
     }
 
+    // js/components/use-changed-flag.ts
+    var import_react43 = __toESM(require_react()),
+        import_react_dom = __toESM(require_react_dom());
+
+    function reducer(state, flushed) {
+        return flushed !== null ? __spreadProps(__spreadValues({}, state), {
+            flushed
+        }) : __spreadProps(__spreadValues({}, state), {
+            changes: state.changes + 1
+        });
+    }
+
+    function useChangedFlag() {
+        let [state, setFlushed] = (0, import_react43.useReducer)(reducer, {
+            changes: 0,
+            flushed: 0
+        }), changesRef = (0, import_react43.useRef)(state.changes);
+        (0, import_react43.useEffect)(() => {
+            changesRef.current = state.changes;
+        }, [state]);
+        let hasPendingChanges = state.changes != state.flushed,
+            setDirty = (0, import_react43.useCallback)(() => {
+                setFlushed(null);
+            }, [setFlushed]),
+            setClean = (0, import_react43.useCallback)(
+                (arg, options) => __async(this, null, function*() {
+                    let cb = typeof arg == "function" ? arg : () => arg,
+                        changes = changesRef.current,
+                        update = () => setFlushed(changes),
+                        result = yield cb();
+                    return options != null && options.sync ? (0, import_react_dom.flushSync)(update) : update(), result;
+                }),
+                [setFlushed]
+            );
+        return [hasPendingChanges, setDirty, setClean];
+    }
+
     // js/views/edit/EditPage.tsx
     function legalFields(recordDataModel, recordInfo) {
         function isLegalField(field) {
             switch (field.name) {
                 case "_id":
                 case "_path":
                 case "_gid":
@@ -12256,14 +14549,27 @@
     }
 
     function getValueForField(recordData, Widget, field) {
         let value = recordData[field.name];
         return value === void 0 && (value = "", Widget.deserializeValue && (value = Widget.deserializeValue(value, field.type))), value;
     }
 
+    function getRecordData({
+        data,
+        datamodel,
+        record_info
+    }) {
+        let recordData = {};
+        return legalFields(datamodel, record_info).forEach((field) => {
+            let Widget = getWidgetComponentWithFallback(field.type),
+                value = data[field.name];
+            value !== void 0 && (Widget.deserializeValue && (value = Widget.deserializeValue(value, field.type)), recordData[field.name] = value);
+        }), recordData;
+    }
+
     function getValues({
         recordDataModel,
         recordInfo,
         recordData
     }) {
         let rv = {};
         return !recordDataModel || !recordInfo || legalFields(recordDataModel, recordInfo).forEach((field) => {
@@ -12273,153 +14579,141 @@
                 Widget.serializeValue && (value = Widget.serializeValue(value, field.type));
             } else
                 value = null;
             rv[field.name] = value;
         }), rv;
     }
 
-    function useBlockNavigation(hasPendingChanges, pendingChanges) {
-        let {
-            navigator: navigator2
-        } = (0, import_react44.useContext)(NavigationContext), blockNavigator = navigator2;
-        (0, import_react44.useEffect)(() => {
-            if (!hasPendingChanges)
-                return;
-            let unblock = blockNavigator.block((tx) => {
-                (!pendingChanges.current || window.confirm(trans("UNLOAD_ACTIVE_TAB"))) && (unblock(), tx.retry());
-            });
-            return unblock;
-        }, [blockNavigator, hasPendingChanges, pendingChanges]);
-    }
-
     function EditPage() {
         let {
             path,
             alt
-        } = useRecord(), form = (0, import_react44.useRef)(null), [recordData, setRecordData] = (0, import_react44.useState)({}), [recordDataModel, setRecordDataModel] = (0, import_react44.useState)(null), [recordInfo, setRecordnfo] = (0, import_react44.useState)(null), pendingChanges = (0, import_react44.useRef)(!1), [hasPendingChanges, rawSetHasPendingChanges] = (0, import_react44.useState)(!1), setHasPendingChanges = (0, import_react44.useCallback)((v) => {
-            rawSetHasPendingChanges(v), pendingChanges.current = v;
-        }, []), goToAdminPage = useGoToAdminPage();
-        useBlockNavigation(hasPendingChanges, pendingChanges), (0, import_react44.useEffect)(() => {
+        } = useRecord(), form = (0, import_react44.useRef)(null), [recordData, setRecordData] = (0, import_react44.useState)({}), [recordDataModel, setRecordDataModel] = (0, import_react44.useState)(null), [recordInfo, setRecordInfo] = (0, import_react44.useState)(null), [hasPendingChanges, setDirty, setClean] = useChangedFlag(), goToAdminPage = useGoToAdminPage();
+        usePrompt({
+            when: hasPendingChanges,
+            message: trans("UNLOAD_ACTIVE_TAB")
+        }), (0, import_react44.useEffect)(() => {
             let ignore = !1;
-            return get("/rawrecord", {
-                path,
-                alt
-            }).then(
-                ({
-                    datamodel,
-                    data,
-                    record_info
-                }) => {
-                    if (!ignore) {
-                        let recordData2 = {};
-                        legalFields(datamodel, record_info).forEach((field) => {
-                            let Widget = getWidgetComponentWithFallback(field.type),
-                                value = data[field.name];
-                            value !== void 0 && (Widget.deserializeValue && (value = Widget.deserializeValue(value, field.type)), recordData2[field.name] = value);
-                        }), setRecordData(recordData2), setRecordDataModel(datamodel), setRecordnfo(record_info), setHasPendingChanges(!1);
-                    }
-                },
-                showErrorDialog
+            return setClean(
+                () => __async(this, null, function*() {
+                    let rawrecord = yield get("/rawrecord", {
+                        path,
+                        alt
+                    }).catch(
+                        showErrorDialog
+                    );
+                    ignore || (setRecordData(getRecordData(rawrecord)), setRecordDataModel(rawrecord.datamodel), setRecordInfo(rawrecord.record_info));
+                }), {
+                    sync: !0
+                }
             ), () => {
                 ignore = !0;
             };
-        }, [alt, path, setHasPendingChanges]), (0, import_react44.useEffect)(() => {
-            let onKeyPress2 = keyboardShortcutHandler({
-                    key: "Control+s",
-                    mac: "Meta+s",
-                    preventDefault: !0
-                },
-                () => {
-                    var _a2;
-                    hasPendingChanges ? (_a2 = form.current) == null || _a2.requestSubmit() : goToAdminPage("preview", path, alt);
-                }
-            );
-            return window.addEventListener("keydown", onKeyPress2), () => window.removeEventListener("keydown", onKeyPress2);
-        }, [hasPendingChanges, goToAdminPage, path, alt]);
+        }, [alt, path, setClean]);
         let setFieldValue = (0, import_react44.useCallback)(
                 (fieldName, value) => {
                     setRecordData((r) => __spreadProps(__spreadValues({}, r), {
                         [fieldName]: typeof value == "function" ? value(r[fieldName]) : value
-                    })), setHasPendingChanges(!0);
+                    })), setDirty();
                 },
-                [setHasPendingChanges]
-            ),
-            saveChanges = (0, import_react44.useCallback)(
-                (ev) => {
-                    ev.preventDefault();
-                    let data = getValues({
-                        recordDataModel,
-                        recordInfo,
-                        recordData
-                    });
-                    put("/rawrecord", {
-                        data,
-                        path,
-                        alt
-                    }).then(() => {
-                        setHasPendingChanges(!1), goToAdminPage("preview", path, alt);
-                    }, showErrorDialog);
-                },
-                [
-                    alt,
-                    goToAdminPage,
-                    path,
-                    recordData,
-                    recordDataModel,
-                    recordInfo,
-                    setHasPendingChanges
-                ]
+                [setDirty]
             ),
-            renderFormField = (0, import_react44.useCallback)(
-                (field) => {
-                    let Widget = getWidgetComponentWithFallback(field.type);
-                    if (!recordInfo)
-                        return null;
-                    let disabled = !(field.alts_enabled === null || field.alts_enabled !== (recordInfo.alt === "_primary"));
-                    return /* @__PURE__ */ import_react44.default.createElement(
-                        FieldBox, {
-                            key: field.name,
-                            value: getValueForField(recordData, Widget, field),
-                            placeholder: getPlaceholderForField(recordInfo, Widget, field),
-                            field,
-                            setFieldValue,
-                            disabled
+            maybeSaveChanges = (0, import_react44.useCallback)(() => __async(this, null, function*() {
+                if (hasPendingChanges)
+                    return setClean(
+                        () => __async(this, null, function*() {
+                            let data = getValues({
+                                recordDataModel,
+                                recordInfo,
+                                recordData
+                            });
+                            yield put("/rawrecord", {
+                                data,
+                                path,
+                                alt
+                            }).catch(showErrorDialog);
+                        }), {
+                            sync: !0
                         }
                     );
-                },
-                [recordData, recordInfo, setFieldValue]
-            );
+            }), [
+                path,
+                alt,
+                hasPendingChanges,
+                setClean,
+                recordData,
+                recordDataModel,
+                recordInfo
+            ]);
+        (0, import_react44.useEffect)(() => {
+            let saveAndPreview = () => __async(this, null, function*() {
+                    yield maybeSaveChanges(), goToAdminPage("preview", path, alt);
+                }),
+                cleanup = [
+                    setShortcutHandler("SAVE_SHORTCUT" /* Save */ , maybeSaveChanges),
+                    setShortcutHandler("PREVIEW_SHORTCUT" /* Preview */ , saveAndPreview)
+                ];
+            return () => cleanup.forEach((cb) => cb());
+        }, [maybeSaveChanges, path, alt, goToAdminPage]);
+        let renderFormField = (0, import_react44.useCallback)(
+            (field) => {
+                let Widget = getWidgetComponentWithFallback(field.type);
+                if (!recordInfo)
+                    return null;
+                let disabled = !(field.alts_enabled === null || field.alts_enabled !== (recordInfo.alt === "_primary"));
+                return /* @__PURE__ */ import_react44.default.createElement(
+                    FieldBox, {
+                        key: field.name,
+                        value: getValueForField(recordData, Widget, field),
+                        placeholder: getPlaceholderForField(recordInfo, Widget, field),
+                        field,
+                        setFieldValue,
+                        disabled
+                    }
+                );
+            },
+            [recordData, recordInfo, setFieldValue]
+        );
         if (!recordInfo || !recordDataModel)
             return null;
         let label = trans_fallback(recordInfo.label_i18n, recordInfo.label),
             title = recordInfo.is_attachment ? trans_format("EDIT_ATTACHMENT_METADATA_OF", label) : trans_format("EDIT_PAGE_NAME", label),
             fields = legalFields(recordDataModel, recordInfo),
             [normalFields, systemFields] = splitFields(fields);
-        return /* @__PURE__ */ import_react44.default.createElement(import_react44.default.Fragment, null, /* @__PURE__ */ import_react44.default.createElement("h2", null, title), /* @__PURE__ */ import_react44.default.createElement("form", {
-            ref: form,
-            onSubmit: saveChanges
-        }, /* @__PURE__ */ import_react44.default.createElement(FieldRows, {
-            fields: normalFields,
-            renderFunc: renderFormField
-        }), systemFields.length > 0 && /* @__PURE__ */ import_react44.default.createElement(
-            ToggleGroup, {
-                groupTitle: trans("SYSTEM_FIELDS"),
-                className: "system-fields"
+        return /* @__PURE__ */ import_react44.default.createElement(import_react44.default.Fragment, null, /* @__PURE__ */ import_react44.default.createElement("h2", null, title), /* @__PURE__ */ import_react44.default.createElement(
+            "form", {
+                ref: form,
+                onSubmit: (e) => {
+                    e.preventDefault(), maybeSaveChanges();
+                }
             },
             /* @__PURE__ */
             import_react44.default.createElement(FieldRows, {
-                fields: systemFields,
+                fields: normalFields,
                 renderFunc: renderFormField
-            })
-        ), /* @__PURE__ */ import_react44.default.createElement(
-            EditPageActions, {
-                recordInfo,
-                hasPendingChanges
-            }
-        )));
+            }),
+            systemFields.length > 0 && /* @__PURE__ */ import_react44.default.createElement(
+                ToggleGroup, {
+                    groupTitle: trans("SYSTEM_FIELDS"),
+                    className: "system-fields"
+                },
+                /* @__PURE__ */
+                import_react44.default.createElement(FieldRows, {
+                    fields: systemFields,
+                    renderFunc: renderFormField
+                })
+            ),
+            /* @__PURE__ */
+            import_react44.default.createElement(
+                EditPageActions, {
+                    recordInfo,
+                    hasPendingChanges
+                }
+            )
+        ));
     }
     var EditPage_default = EditPage;
 
     // js/views/delete/DeletePage.tsx
     var import_react51 = __toESM(require_react());
 
     // js/views/delete/DeletableAttachments.tsx
@@ -12654,14 +14948,15 @@
     }
 
     // js/views/add-child-page/AddChildPage.tsx
     var import_react56 = __toESM(require_react());
 
     // js/slugify.ts
     var charmap = {
+            // latin
             \u00C0: "A",
             \u00C1: "A",
             \u00C2: "A",
             \u00C3: "A",
             \u00C4: "Ae",
             \u00C5: "A",
             \u00C6: "AE",
@@ -12721,14 +15016,15 @@
             \u00FB: "u",
             \u00FC: "ue",
             \u0171: "u",
             \u00FD: "y",
             \u00FE: "th",
             \u00FF: "y",
             "\u1E9E": "SS",
+            // greek
             \u03B1: "a",
             \u03B2: "b",
             \u03B3: "g",
             \u03B4: "d",
             \u03B5: "e",
             \u03B6: "z",
             \u03B7: "h",
@@ -12790,20 +15086,22 @@
             \u038A: "I",
             \u038C: "O",
             \u038E: "Y",
             \u0389: "H",
             \u038F: "W",
             \u03AA: "I",
             \u03AB: "Y",
+            // turkish
             \u015F: "s",
             \u015E: "S",
             \u0131: "i",
             \u0130: "I",
             \u011F: "g",
             \u011E: "G",
+            // russian
             \u0430: "a",
             \u0431: "b",
             \u0432: "v",
             \u0433: "g",
             \u0434: "d",
             \u0435: "e",
             \u0451: "yo",
@@ -12862,22 +15160,24 @@
             \u0429: "Sh",
             \u042A: "U",
             \u042B: "Y",
             \u042C: "",
             \u042D: "E",
             \u042E: "Yu",
             \u042F: "Ya",
+            // ukranian
             \u0404: "Ye",
             \u0406: "I",
             \u0407: "Yi",
             \u0490: "G",
             \u0454: "ye",
             \u0456: "i",
             \u0457: "yi",
             \u0491: "g",
+            // czech
             \u010D: "c",
             \u010F: "d",
             \u011B: "e",
             \u0148: "n",
             \u0159: "r",
             \u0161: "s",
             \u0165: "t",
@@ -12888,14 +15188,15 @@
             \u011A: "E",
             \u0147: "N",
             \u0158: "R",
             \u0160: "S",
             \u0164: "T",
             \u016E: "U",
             \u017D: "Z",
+            // polish
             \u0105: "a",
             \u0107: "c",
             \u0119: "e",
             \u0142: "l",
             \u0144: "n",
             \u015B: "s",
             \u017A: "z",
@@ -12904,14 +15205,15 @@
             \u0106: "C",
             \u0118: "E",
             \u0141: "L",
             \u0143: "N",
             \u015A: "S",
             \u0179: "Z",
             \u017B: "Z",
+            // latvian
             \u0101: "a",
             \u0113: "e",
             \u0123: "g",
             \u012B: "i",
             \u0137: "k",
             \u013C: "l",
             \u0146: "n",
@@ -12920,28 +15222,31 @@
             \u0112: "E",
             \u0122: "G",
             \u012A: "I",
             \u0136: "K",
             \u013B: "L",
             \u0145: "N",
             \u016A: "U",
+            // lithuanian
             \u0117: "e",
             \u012F: "i",
             \u0173: "u",
             \u0116: "E",
             \u012E: "I",
             \u0172: "U",
+            // romanian
             \u021B: "t",
             \u021A: "T",
             \u0163: "t",
             \u0162: "T",
             \u0219: "s",
             \u0218: "S",
             \u0103: "a",
             \u0102: "A",
+            // currency
             "\u20AC": "euro",
             "\u20A2": "cruzeiro",
             "\u20A3": "french franc",
             "\xA3": "pound",
             "\u20A4": "lira",
             "\u20A5": "mill",
             "\u20A6": "naira",
@@ -12965,14 +15270,15 @@
             \u5186: "yen",
             "\uFDFC": "rial",
             "\u20A0": "ecu",
             "\xA4": "currency",
             "\u0E3F": "baht",
             $: "dollar",
             "\u20B9": "indian rupee",
+            // symbols
             "\xA9": "(c)",
             \u0153: "oe",
             \u0152: "OE",
             "\u2211": "sum",
             "\xAE": "(r)",
             "\u2020": "+",
             "\u201C": '"',
@@ -13278,19 +15584,45 @@
         "add-child": AddChildPage_default,
         upload: AddAttachmentPage_default
     };
 
     function App() {
         let page = (0, import_react58.useContext)(PageContext),
             [sidebarIsActive, toggleSidebar] = (0, import_react58.useReducer)((v) => !v, !1),
+            [appSettings, setAppSettings] = (0, import_react58.useState)(loadAppSettings()),
+            {
+                path,
+                alt
+            } = useRecord(),
+            goToAdminPage = useGoToAdminPage(),
             MainComponent = mainComponentForPage[page];
-        return /* @__PURE__ */ import_react58.default.createElement(import_react58.default.Fragment, null, /* @__PURE__ */ import_react58.default.createElement(Header, {
+        return (0, import_react58.useEffect)(() => (saveAppSettings(appSettings), installShortcutKeyListener(appSettings.shortcutKeyMap)), [appSettings]), (0, import_react58.useEffect)(() => {
+            let cleanup = [{
+                action: "EDIT_SHORTCUT" /* Edit */ ,
+                target: "edit"
+            }, {
+                action: "PREVIEW_SHORTCUT" /* Preview */ ,
+                target: "preview"
+            }].filter(({
+                target
+            }) => target != page).map(
+                ({
+                    action,
+                    target
+                }) => setShortcutHandler(action, () => goToAdminPage(target, path, alt))
+            );
+            return () => cleanup.forEach((cb) => cb());
+        }, [page, path, alt, goToAdminPage]), /* @__PURE__ */ import_react58.default.createElement(AppSettingsContext.Provider, {
+            value: appSettings
+        }, /* @__PURE__ */ import_react58.default.createElement(Header, {
             sidebarIsActive,
             toggleSidebar
-        }), /* @__PURE__ */ import_react58.default.createElement(ErrorDialog, null), /* @__PURE__ */ import_react58.default.createElement(DialogSlot, null), /* @__PURE__ */ import_react58.default.createElement("div", {
+        }), /* @__PURE__ */ import_react58.default.createElement(ErrorDialog, null), /* @__PURE__ */ import_react58.default.createElement(DialogSlot, {
+            setAppSettings
+        }), /* @__PURE__ */ import_react58.default.createElement("div", {
             className: "container"
         }, /* @__PURE__ */ import_react58.default.createElement(
             "div", {
                 className: sidebarIsActive ? "block-offcanvas row active" : "block-offcanvas row"
             },
             /* @__PURE__ */
             import_react58.default.createElement("nav", {
@@ -13322,22 +15654,111 @@
         }, /* @__PURE__ */ import_react59.default.createElement(RecordContext.Provider, {
             value: record
         }, /* @__PURE__ */ import_react59.default.createElement(App, null)));
     }
 
     function Main() {
         var _a2;
-        let root = $LEKTOR_CONFIG.admin_root,
-            page = (_a2 = useMatch(`${root}/:page`)) == null ? void 0 : _a2.params.page;
+        let page = (_a2 = useMatch(":page")) == null ? void 0 : _a2.params.page;
         return isPageName(page) ? /* @__PURE__ */ import_react59.default.createElement(Page, {
             page
         }) : /* @__PURE__ */ import_react59.default.createElement(Navigate, {
             to: adminPath("edit", "/", "_primary")
         });
     }
     var dash = document.getElementById("dash");
-    dash && (setCurrentLanguage($LEKTOR_CONFIG.lang), (0, import_client.createRoot)(dash).render(
-        /* @__PURE__ */
-        import_react59.default.createElement(import_react59.StrictMode, null, /* @__PURE__ */ import_react59.default.createElement(BrowserRouter, null, /* @__PURE__ */ import_react59.default.createElement(Main, null)))
-    ));
+    if (dash) {
+        setCurrentLanguage($LEKTOR_CONFIG.lang);
+        let root = (0, import_client.createRoot)(dash),
+            router = createBrowserRouter(
+                [{
+                    path: "/",
+                    element: /* @__PURE__ */ import_react59.default.createElement(Navigate, {
+                        to: adminPath("edit", "/", "_primary")
+                    })
+                }, {
+                    path: "/:page",
+                    element: /* @__PURE__ */ import_react59.default.createElement(Main, null)
+                }], {
+                    basename: $LEKTOR_CONFIG.admin_root
+                }
+            );
+        root.render(
+            /* @__PURE__ */
+            import_react59.default.createElement(import_react59.StrictMode, null, /* @__PURE__ */ import_react59.default.createElement(RouterProvider, {
+                router
+            }))
+        );
+    }
 })();
+/*! Bundled license information:
+
+react/cjs/react.production.min.js:
+  (**
+   * @license React
+   * react.production.min.js
+   *
+   * Copyright (c) Facebook, Inc. and its affiliates.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE file in the root directory of this source tree.
+   *)
+
+scheduler/cjs/scheduler.production.min.js:
+  (**
+   * @license React
+   * scheduler.production.min.js
+   *
+   * Copyright (c) Facebook, Inc. and its affiliates.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE file in the root directory of this source tree.
+   *)
+
+react-dom/cjs/react-dom.production.min.js:
+  (**
+   * @license React
+   * react-dom.production.min.js
+   *
+   * Copyright (c) Facebook, Inc. and its affiliates.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE file in the root directory of this source tree.
+   *)
+
+@remix-run/router/dist/router.js:
+  (**
+   * @remix-run/router v1.5.0
+   *
+   * Copyright (c) Remix Software Inc.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE.md file in the root directory of this source tree.
+   *
+   * @license MIT
+   *)
+
+react-router/dist/index.js:
+  (**
+   * React Router v6.10.0
+   *
+   * Copyright (c) Remix Software Inc.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE.md file in the root directory of this source tree.
+   *
+   * @license MIT
+   *)
+
+react-router-dom/dist/index.js:
+  (**
+   * React Router DOM v6.10.0
+   *
+   * Copyright (c) Remix Software Inc.
+   *
+   * This source code is licensed under the MIT license found in the
+   * LICENSE.md file in the root directory of this source tree.
+   *
+   * @license MIT
+   *)
+*/
 //# sourceMappingURL=app.js.map
```

### Comparing `lektor-3.4.0b5/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2` & `lektor-3.4.0b6/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/templates/dash.html` & `lektor-3.4.0b6/lektor/admin/templates/dash.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/templates/edit-button.html` & `lektor-3.4.0b6/lektor/admin/templates/edit-button.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/templates/livereload-worker.js` & `lektor-3.4.0b6/lektor/admin/templates/livereload-worker.js`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/admin/templates/livereload.html` & `lektor-3.4.0b6/lektor/admin/templates/livereload.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/environment/__init__.py` & `lektor-3.4.0b6/lektor/environment/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import fnmatch
 import os
 import uuid
 from functools import update_wrapper
 from typing import TYPE_CHECKING
 
+import babel.dates
 import jinja2
-from babel import dates
 from jinja2.loaders import split_template_path
 
 from lektor.constants import PRIMARY_ALT
 from lektor.context import config_proxy
 from lektor.context import get_asset_url
 from lektor.context import get_ctx
 from lektor.context import get_locale
@@ -30,35 +30,101 @@
 from lektor.utils import tojson_filter
 
 
 if TYPE_CHECKING:
     from typing import Literal
 
 
-def _pass_locale(func):
-    def new_func(*args, **kwargs):
-        if kwargs.get("locale", None) is None:
+def _prevent_inlining(wrapped):
+    """Ensure wrapped jinja filter does not get inlined by the template compiler.
+
+    The jinja compiler normally assumes that filters are pure functions (whose
+    result depends only on their parameters) and will inline filter calls that
+    are applied to compile-time constants.
+
+    E.g.
+
+        'say {{ "foo" | upper }}'
+
+    will be compiled to
+
+        "say Foo"
+
+    Many of our filters depend on global state (e..g the Lektor build context).
+
+    Applying this decorator to them will ensure they are not inlined.
+    """
+    # the use of @pass_context will prevent inlining
+    @jinja2.pass_context
+    def wrapper(_jinja_ctx, *args, **kwargs):
+        return wrapped(*args, **kwargs)
+
+    return update_wrapper(wrapper, wrapped)
+
+
+def _dates_filter(name, wrapped):
+    """Wrap one of the babel.dates.format_* functions for use as a jinja filter.
+
+    This will create a jinja filter that will:
+
+    - Check for *undefined* date/time input (and, in that case, return an empty string).
+
+    - Check that the ``format`` and ``locale`` parameters, if provided, have the correct
+      types, otherwise raising ``TypeError``.
+
+    - Raise ``TypeError`` with a somewhat informative message if the wrapped formatting
+      function raises an unexpected exception.  Such an exception is most likely due to
+      being passed an unsupported date/time time.  (The Babel formatting functions
+      accept a fairly wide range of input types — and that range might potentially vary
+      between releases — so we do not explicitly check the input type before passing it
+      on to Babel.)
+
+    If `locale` is not specified, we fill it in based on the current *alt*.
+
+    """
+
+    @_prevent_inlining
+    def wrapper(arg, format="medium", **kwargs):
+        if isinstance(arg, jinja2.Undefined):
+            # This will typically return an empty string, though it depends on the
+            # specific type of undefined instance.  E.g. if arg is a DebugUndefined, it
+            # will return a more descriptive message, and if arg is a StrictUndefined,
+            # an UndefinedError will be raised.
+            return str(arg)
+
+        if not isinstance(format, str):
+            raise TypeError(
+                f"The 'format' parameter to '{name}' should be a str, not {format!r}"
+            )
+
+        locale = kwargs.get("locale")
+        if locale is None:
             kwargs["locale"] = get_locale("en_US")
-        return func(*args, **kwargs)
 
-    return update_wrapper(new_func, func)
+        try:
+            return wrapped(arg, format, **kwargs)
+        except (TypeError, ValueError):
+            raise
+        except Exception as exc:
+            raise TypeError(
+                f"While evaluating filter '{name}', an unexpected exception was raised. "
+                "This is likely caused by an input or parameter of an unsupported type."
+            ) from exc
+
+    return update_wrapper(wrapper, wrapped)
 
 
-@jinja2.pass_context
+@_prevent_inlining
 def _markdown_filter(
-    _jinja_context: jinja2.runtime.Context,
     source: str,
     *,
     resolve_links: "Literal['always', 'never', 'when-possible', None]" = None,
-    **kw: str
+    **kw: str,
 ) -> Markdown:
     """A jinja filter that converts markdown text to HTML."""
-    # By default Jinja treats filters as pure functions, and will memoize
-    # their results. Since here we depend on global context, we mark the filter
-    # as a "context filter" to prevent memoization.
     ctx = get_ctx()
     source_obj = ctx.source if ctx is not None else None
     return Markdown(
         source, source_obj, field_options={**kw, "resolve_links": resolve_links}
     )
 
 
@@ -150,34 +216,31 @@
         from lektor.db import F, get_alts  # pylint: disable=import-outside-toplevel
 
         self.jinja_env.filters.update(
             tojson=tojson_filter,
             latformat=lambda x, secs=True: format_lat_long(lat=x, secs=secs),
             longformat=lambda x, secs=True: format_lat_long(long=x, secs=secs),
             latlongformat=lambda x, secs=True: format_lat_long(secs=secs, *x),
-            # By default filters need to be side-effect free.  This is not
-            # the case for this one, so we need to make it as a dummy
-            # context filter so that jinja2 will not inline it.
-            url=jinja2.pass_context(lambda ctx, *a, **kw: url_to(*a, **kw)),
-            asseturl=jinja2.pass_context(lambda ctx, *a, **kw: get_asset_url(*a, **kw)),
+            url=_prevent_inlining(url_to),
+            asseturl=_prevent_inlining(get_asset_url),
             markdown=_markdown_filter,
         )
         self.jinja_env.globals.update(
             F=F,
             url_to=url_to,
             site=site_proxy,
             config=config_proxy,
             bag=lookup_from_bag,
             get_alts=get_alts,
             get_random_id=lambda: uuid.uuid4().hex,
         )
         self.jinja_env.filters.update(
-            datetimeformat=_pass_locale(dates.format_datetime),
-            dateformat=_pass_locale(dates.format_date),
-            timeformat=_pass_locale(dates.format_time),
+            dateformat=_dates_filter("dateformat", babel.dates.format_date),
+            datetimeformat=_dates_filter("datetimeformat", babel.dates.format_datetime),
+            timeformat=_dates_filter("timeformat", babel.dates.format_time),
         )
 
         # pylint: disable=import-outside-toplevel
         from lektor.types import builtin_types
 
         self.types = builtin_types.copy()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lektor-3.4.0b5/lektor/environment/config.py` & `lektor-3.4.0b6/lektor/environment/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import copy
 import os
 import re
 from collections import OrderedDict
+from urllib.parse import urlsplit
 
 from inifile import IniFile
-from werkzeug.urls import url_parse
 from werkzeug.utils import cached_property
 
 from lektor.constants import PRIMARY_ALT
 from lektor.i18n import get_i18n_block
 from lektor.utils import bool_from_string
 from lektor.utils import secure_url
 
 
 DEFAULT_CONFIG = {
-    "IMAGEMAGICK_EXECUTABLE": None,
     "EPHEMERAL_RECORD_CACHE_SIZE": 500,
     "ATTACHMENT_TYPES": {
         # Only enable image formats here that we can handle in imagetools.
-        # Right now this is limited to jpg, png and gif because this is
-        # the only thing we compile into imagemagick on OS X distributions
-        # as those are what browsers also support.  Thers is no point in
-        # adding others here as we do not force convert images (yet?) but
-        # only use it for thumbnailing.  However an image should be
-        # visible even without thumbnailing.
+        # Right now this is limited to jpg, png and gif.
         ".jpg": "image",
         ".jpeg": "image",
         ".png": "image",
         ".gif": "image",
         ".svg": "image",
         ".avi": "video",
         ".mpg": "video",
@@ -57,23 +51,14 @@
     "ALTERNATIVES": OrderedDict(),
     "PRIMARY_ALTERNATIVE": None,
     "SERVERS": {},
 }
 
 
 def update_config_from_ini(config, inifile):
-    def set_simple(target, source_path):
-        rv = config.get(source_path)
-        if rv is not None:
-            config[target] = rv
-
-    set_simple(
-        target="IMAGEMAGICK_EXECUTABLE", source_path="env.imagemagick_executable"
-    )
-
     for section_name in ("ATTACHMENT_TYPES", "PROJECT", "PACKAGES", "THEME_SETTINGS"):
         section_config = inifile.section_as_dict(section_name.lower())
         config[section_name].update(section_config)
 
     for sect in inifile.sections():
         if sect.startswith("servers."):
             server_id = sect.split(".")[1]
@@ -268,24 +253,24 @@
         """The identifier that acts as primary alternative."""
         return self.values["PRIMARY_ALTERNATIVE"]
 
     @cached_property
     def base_url(self):
         """The external base URL."""
         url = self.values["PROJECT"].get("url")
-        if url and url_parse(url).scheme:
+        if url and urlsplit(url).scheme:
             return url.rstrip("/") + "/"
         return None
 
     @cached_property
     def base_path(self):
         """The base path of the URL."""
         url = self.values["PROJECT"].get("url")
         if url:
-            return url_parse(url).path.rstrip("/") + "/"
+            return urlsplit(url).path.rstrip("/") + "/"
         return "/"
 
     @cached_property
     def url_style(self):
         """The intended URL style."""
         style = self.values["PROJECT"].get("url_style")
         if style in ("relative", "absolute", "external"):
```

### Comparing `lektor-3.4.0b5/lektor/environment/expressions.py` & `lektor-3.4.0b6/lektor/environment/expressions.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/markdown/__init__.py` & `lektor-3.4.0b6/lektor/markdown/mistune0.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,79 @@
-from typing import Any
-from typing import Dict
-from typing import Hashable
+"""MarkdownController implementation for mistune 0.x"""
+import threading
+from typing import ClassVar
+from typing import List
 from typing import Optional
-from typing import Type
-from typing import TYPE_CHECKING
-from weakref import ref as weakref
-
-from markupsafe import Markup
-
-from lektor.compat import importlib_metadata as metadata
-from lektor.markdown.controller import ControllerCache
-from lektor.markdown.controller import FieldOptions
+
+import mistune  # type: ignore[import]
+
 from lektor.markdown.controller import MarkdownController
-from lektor.markdown.controller import Meta
-from lektor.markdown.controller import RenderResult
+from lektor.markdown.controller import Meta  # FIXME: move this?
+from lektor.markdown.controller import RendererHelper
 from lektor.sourceobj import SourceObject
 from lektor.utils import deprecated
 
-if TYPE_CHECKING:  # pragma: no cover
-    from lektor.environment import Environment
-
-
-controller_class: Type[MarkdownController]
-
-MISTUNE_VERSION = metadata.version("mistune")
-if MISTUNE_VERSION.startswith("0."):
-    from lektor.markdown.mistune0 import MarkdownController0 as controller_class
-elif MISTUNE_VERSION.startswith("2."):
-    from lektor.markdown.mistune2 import MarkdownController2 as controller_class
-else:  # pragma: no cover
-    raise ImportError("Unsupported version of mistune")
-
-
-get_controller = ControllerCache(controller_class)
-
 
-@deprecated(version="3.4.0")
-def make_markdown(env: "Environment") -> Any:  # (Environment) -> mistune.Markdown
-    return get_controller(env).make_parser()
+def escape(text: str) -> str:
+    return mistune.escape(text, quote=True)
 
 
-@deprecated(version="3.4.0")
-def markdown_to_html(
-    text: str, record: SourceObject, field_options: FieldOptions
-) -> RenderResult:
-    return get_controller().render(text, record, field_options)
+class ImprovedRenderer(
+    # pylint: disable=no-member
+    mistune.Renderer  # type: ignore[misc]
+):
+    lektor: ClassVar = RendererHelper()
 
-
-class Markdown:
-    def __init__(
-        self, source: str, record: Optional[SourceObject], field_options: FieldOptions
-    ) -> None:
-        self.source = source
-        self.__record = weakref(record) if record is not None else None
-        self.__field_options = field_options
-        self.__cache: Dict[Hashable, RenderResult] = {}
-
-    def __bool__(self) -> bool:
-        return bool(self.source)
-
-    __nonzero__ = __bool__
-
-    @property
+    @property  # type: ignore[misc] # https://github.com/python/mypy/issues/1362
+    @deprecated("Use ImprovedRenderer.lektor.record instead.", version="3.4.0")
     def record(self) -> SourceObject:
-        ref = self.__record
-        if ref is None:
-            return None
-        record = ref()
-        if record is None:
-            raise RuntimeError("Record has gone away")
-        return record
-
-    def __render(self) -> RenderResult:
-        # When the markdown instance is attached to a cached object we
-        # can end up in the situation where, e.g., the base_url has
-        # changed from the time we were put into the cache to the time
-        # where we got referenced by something elsewhere.  Since this
-        # affects the processing of relative links, in that case we
-        # need to re-process our markdown.
-        controller = get_controller()
-        key = controller.get_cache_key()
-        result = self.__cache.get(key) if key is not None else None
-        if result is None:
-            result = controller.render(self.source, self.record, self.__field_options)
-            if key is not None:
-                self.__cache[key] = result
-        return result
+        return self.lektor.record
 
-    @property
+    @property  # type: ignore[misc]
+    @deprecated("Use ImprovedRenderer.lektor.meta instead.", version="3.4.0")
     def meta(self) -> Meta:
-        return self.__render().meta
-
-    @property
-    def html(self) -> Markup:
-        return Markup(self.__render().html)
-
-    def __getitem__(self, name: str) -> Any:
-        return self.meta[name]
-
-    def __str__(self) -> str:
-        return self.__render().html
+        return self.lektor.meta
 
-    def __html__(self) -> Markup:
-        return self.html
+    def link(self, link: str, title: Optional[str], text: str) -> str:
+        url = self.lektor.resolve_url(link)
+        if not title:
+            return f'<a href="{escape(url)}">{text}</a>'
+        return f'<a href="{escape(url)}" title="{escape(title)}">{text}</a>'
+
+    def image(self, src: str, title: Optional[str], text: str) -> str:
+        url = escape(self.lektor.resolve_url(src))
+        if not title:
+            return f'<img src="{url}" alt="{escape(text)}">'
+        return f'<img src="{url}" alt="{escape(text)}" title="{escape(title)}">'
+
+
+class MarkdownConfig:
+    def __init__(self) -> None:
+        self.options = {
+            "escape": False,
+        }
+        self.renderer_base = ImprovedRenderer
+        self.renderer_mixins: List[type] = []
+
+    def make_renderer(self) -> ImprovedRenderer:
+        bases = tuple(self.renderer_mixins) + (self.renderer_base,)
+        renderer_cls = type("renderer_cls", bases, {})
+        return renderer_cls(**self.options)
+
+
+class MarkdownController0(MarkdownController, threading.local):
+    # NB: making this a threading.local means the results in the
+    # cached_property MarkdownController.parser having a separate
+    # value in each thread.
+    #
+    # We need that since the mistune 0.x parser is not thread-safe.
+
+    def make_parser(self) -> mistune.Markdown:
+        env = self.env
+        cfg = MarkdownConfig()
+        env.plugin_controller.emit("markdown-config", config=cfg)
+        renderer = cfg.make_renderer()
+        env.plugin_controller.emit(
+            "markdown-lexer-config", config=cfg, renderer=renderer
+        )
+        # pylint: disable=unexpected-keyword-arg
+        return mistune.Markdown(renderer, **cfg.options)
```

### Comparing `lektor-3.4.0b5/lektor/markdown/controller.py` & `lektor-3.4.0b6/lektor/markdown/controller.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/markdown/mistune2.py` & `lektor-3.4.0b6/lektor/markdown/mistune2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,38 @@
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 
-import mistune  # type: ignore[import]
+import mistune.util
 
 from lektor.markdown.controller import MarkdownController
 from lektor.markdown.controller import RendererHelper
 from lektor.markdown.controller import UnknownPluginError
 from lektor.utils import unique_everseen
 
 
+def escape(text: str) -> str:
+    # This is only here to provide the implementation for the
+    # deprecated lektor.markdown.escape method.
+    #
+    # (We don't use it below and it can be deleted once access
+    # to lektor.markdown.escape is removed.)
+    return mistune.util.escape(text, quote=True)
+
+
 class ImprovedRenderer(mistune.HTMLRenderer):  # type: ignore[misc]
     lektor: ClassVar = RendererHelper()
 
+    # The deprecated .record and .meta attributes are not made available here, since old
+    # renderer mixins (written for Lektor<3.4 and mistune 0.x) are not going to work
+    # with mistune 2.x anyway.
+
     def link(
         self, link: str, text: Optional[str] = None, title: Optional[str] = None
     ) -> str:
         link = self.lektor.resolve_url(link)
         return super().link(link, text, title)
 
     def image(self, src: str, alt: str = "", title: Optional[str] = None) -> str:
```

### Comparing `lektor-3.4.0b5/lektor/quickstart-templates/plugin/setup.cfg.in` & `lektor-3.4.0b6/lektor/quickstart-templates/plugin/setup.cfg.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/quickstart-templates/project/assets/static/style.css.in` & `lektor-3.4.0b6/lektor/quickstart-templates/project/assets/static/style.css.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/quickstart-templates/project/templates/layout.html.in` & `lektor-3.4.0b6/lektor/quickstart-templates/project/templates/layout.html.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/quickstart-templates/project/templates/macros/blog.html.in` & `lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/blog.html.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/quickstart-templates/theme/images/homepage.png` & `lektor-3.4.0b6/lektor/quickstart-templates/theme/images/homepage.png`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/ca.json` & `lektor-3.4.0b6/lektor/translations/ca.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/de.json` & `lektor-3.4.0b6/lektor/translations/de.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/en.json` & `lektor-3.4.0b6/lektor/translations/en.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9485294117647058%*

 * *Differences: {"'EDIT_SHORTCUT'": "'Edit'",*

 * * "'PREFERENCES'": "'Preferences'",*

 * * "'PREVIEW_SHORTCUT'": "'(Save &) Preview'",*

 * * "'RESET'": "'Reset'",*

 * * "'RESET_TO_DEFAULTS'": "'Reset to defaults'",*

 * * "'SAVE_SHORTCUT'": "'Save'",*

 * * "'SEARCH_SHORTCUT'": "'Search'"}*

```diff
@@ -42,14 +42,15 @@
     "DELETE_PRIMARY_ALT_INFO": "Because this record is a primary alternative it can be deleted separately or together with all other contents.",
     "DELETE_RECORD": "Delete \u201c%s\u201d",
     "DOWN": "Down",
     "EDIT": "Edit",
     "EDIT_ATTACHMENT_METADATA_OF": "Edit Metadata of Attachment \u201c%s\u201d",
     "EDIT_METADATA": "Edit Metadata",
     "EDIT_PAGE_NAME": "Edit \u201c%s\u201d",
+    "EDIT_SHORTCUT": "Edit",
     "ERROR": "Error",
     "ERROR_CANNOT_BROWSE_FS": "Error: File does not exist yet.",
     "ERROR_INVALID_DATE": "Invalid date",
     "ERROR_INVALID_ID": "Invalid ID",
     "ERROR_INVALID_NUMBER": "Not a valid number",
     "ERROR_INVALID_URL": "Not a valid URL",
     "ERROR_NO_ID_PROVIDED": "No ID provided.",
@@ -87,15 +88,17 @@
     "OPEN_OTHER_PROJECT_QUESTION": "Opening this file requires opening another project (%s). The current project will be closed. Do you want to continue?",
     "OPEN_PROJECT": "Open Project",
     "OPERATION_SUCCESS": "Success",
     "PAGE_ACTIONS": "Page Actions",
     "PAGE_IS_DISCOVERABLE": "Page is discoverable",
     "PAGE_IS_DISCOVERABLE_EXPLANATION": "If this is enabled the page can be discovered, otherwise the URL has to be known.",
     "PASTE": "Paste",
+    "PREFERENCES": "Preferences",
     "PREVIEW": "Preview",
+    "PREVIEW_SHORTCUT": "(Save &) Preview",
     "PRIMARY_ALT": "Primary",
     "PRIMARY_OVERLAY": "Overlaid",
     "PROGRESS": "Progress",
     "PROJECT": "Project",
     "PUBLISH": "Publish",
     "PUBLISH_DONE": "Published",
     "PUBLISH_NOTE": "From here you can publish the current version of the website.",
@@ -107,16 +110,20 @@
     "QUIT_LEKTOR": "Quit Lektor",
     "REDO": "Redo",
     "REFRESHING_BUILD_DONE": "Done refreshing build!",
     "REFRESH_BUILD": "Refresh Build",
     "REFRESH_BUILD_NOTE": "This deletes all cached build results which triggers a rebuilt from scratch.  This is useful in certain situations where sync errors or mistakes in templates caused corrupted output.",
     "REMOVE": "Remove",
     "REMOVE_FLOWBLOCK_PROMPT": "Do you really want to remove this block?",
+    "RESET": "Reset",
+    "RESET_TO_DEFAULTS": "Reset to defaults",
     "RETURN_TO_WEBSITE": "Return to Website",
     "SAVE_CHANGES": "Save Changes",
+    "SAVE_SHORTCUT": "Save",
+    "SEARCH_SHORTCUT": "Search",
     "SELECT_ALL": "Select All",
     "SHRINK_TEXTAREA": "Shrink textarea",
     "STATE": "Status",
     "SYSTEM_FIELDS": "System Fields",
     "TEMPLATE": "Template",
     "TRISTATE_CHECKBOX_TOOLTIP": "Tri-state checkbox: use <del> or <backspace> to revert to unset",
     "UNDO": "Undo",
```

### Comparing `lektor-3.4.0b5/lektor/translations/es.json` & `lektor-3.4.0b6/lektor/translations/es.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/fr.json` & `lektor-3.4.0b6/lektor/translations/fr.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/it.json` & `lektor-3.4.0b6/lektor/translations/it.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/ja.json` & `lektor-3.4.0b6/lektor/translations/ja.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/ko.json` & `lektor-3.4.0b6/lektor/translations/ko.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/nl.json` & `lektor-3.4.0b6/lektor/translations/nl.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/pl.json` & `lektor-3.4.0b6/lektor/translations/pl.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/pt.json` & `lektor-3.4.0b6/lektor/translations/pt.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/ru.json` & `lektor-3.4.0b6/lektor/translations/ru.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/translations/zh.json` & `lektor-3.4.0b6/lektor/translations/zh.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/__init__.py` & `lektor-3.4.0b6/lektor/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/base.py` & `lektor-3.4.0b6/lektor/types/base.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/fake.py` & `lektor-3.4.0b6/lektor/types/fake.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/flow.py` & `lektor-3.4.0b6/lektor/types/flow.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/formats.py` & `lektor-3.4.0b6/lektor/types/formats.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/multi.py` & `lektor-3.4.0b6/lektor/types/multi.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/primitives.py` & `lektor-3.4.0b6/lektor/types/primitives.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/lektor/types/special.py` & `lektor-3.4.0b6/lektor/types/special.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 class UrlType(SingleInputType):
     widget = "url"
 
     def value_from_raw(self, raw):
         if raw.value is None:
             return raw.missing_value("Missing URL")
-        return Url(raw.value)
+        return Url.from_string(raw.value)
```

### Comparing `lektor-3.4.0b5/tests/conftest.py` & `lektor-3.4.0b6/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import os
 import shutil
 import sys
 import textwrap
+from contextlib import contextmanager
 from pathlib import Path
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 
 import lektor.project
 from lektor.builder import Builder
@@ -48,16 +49,16 @@
 
     mp = MonkeyPatch()
     mp.setattr(lektor.project, "get_cache_dir", get_cache_dir)
     yield cache_dir
     mp.undo()
 
 
-@pytest.fixture
-def save_sys_path(monkeypatch):
+@contextmanager
+def restore_import_state():
     """Save `sys.path`, and `sys.modules` state on test
     entry, restore after test completion.
 
     Any test which constructs a `lektor.environment.Environment` instance
     or which runs any of the Lektor CLI commands should use this fixture
     to ensure that alterations made to `sys.path` do not interfere with
     other tests.
@@ -67,27 +68,70 @@
     whenever a Lektor `Environment` is constructed (unless
     `load_plugins=False` is specified.)  Since all tests are run
     within an single invocation of the python interpreter, this can
     cause problems when different tests are using different private
     package caches.
 
     """
-    monkeypatch.setattr(sys, "path", sys.path.copy())
+    path = sys.path.copy()
+    meta_path = sys.meta_path.copy()
+    path_hooks = sys.path_hooks.copy()
+    modules = sys.modules.copy()
+
+    # Importlib_metadata, when it is imported, cripples the stdlib distribution finder
+    # by deleting its find_distributions method.
+    #
+    # https://github.com/python/importlib_metadata/blob/705a7571ec7c5abec4d4b008da3a58df7e5c94e7/importlib_metadata/_compat.py#L31
+    #
+    def clone_class(cls):
+        return type(cls)(cls.__name__, cls.__bases__, cls.__dict__.copy())
+
+    sys.meta_path[:] = [
+        clone_class(finder) if isinstance(finder, type) else finder
+        for finder in meta_path
+    ]
 
-    # Restoring `sys.modules` is an attempt to unload any
-    # modules loaded during the test so that they can be re-loaded for
-    # the next test.  This is not guaranteed to work, since there are
-    # numerous ways that a reference to a loaded module may still be held.
-    monkeypatch.setattr(sys, "modules", sys.modules.copy())
+    try:
+        yield
+    finally:
+        importlib.invalidate_caches()
 
-    # It's not clear that this is necessary, but it probably won't hurt.
-    importlib.invalidate_caches()
+        # NB: Restore sys.modules, sys.path, et. all. in place. (Some modules may hold
+        # references to these — e.g. pickle appears to hold a reference to sys.modules.)
+        for module in set(sys.modules).difference(modules):
+            del sys.modules[module]
+        sys.modules.update(modules)
+        sys.path[:] = path
+        sys.meta_path[:] = meta_path
+        sys.path_hooks[:] = path_hooks
+        sys.path_importer_cache.clear()
 
 
-@pytest.fixture(scope="function")
+_initial_path_key = object()
+
+
+@pytest.hookimpl(tryfirst=True)
+def pytest_runtest_setup(item):
+    item.stash[_initial_path_key] = sys.path.copy()
+
+
+@pytest.hookimpl(trylast=True)
+def pytest_runtest_teardown(item):
+    # Check that tests don't alter sys.path
+    initial_path = item.stash[_initial_path_key]
+    assert sys.path == initial_path
+
+
+@pytest.fixture
+def save_sys_path():
+    with restore_import_state():
+        yield
+
+
+@pytest.fixture(scope="session")
 def project(data_path):
     return Project.from_path(data_path / "demo-project")
 
 
 @pytest.fixture(scope="function")
 def scratch_project_data(tmp_path):
     base = tmp_path / "scratch-proj"
@@ -175,25 +219,35 @@
 @pytest.fixture(scope="function")
 def builder(tmp_path, pad):
     output_path = tmp_path / "output"
     output_path.mkdir()
     return Builder(pad, str(output_path))
 
 
+@pytest.fixture(scope="session")
+def built_demo(tmp_path_factory, project):
+    output_path = tmp_path_factory.mktemp("demo-output")
+    with restore_import_state():
+        env = Environment(project)
+        builder = Builder(env.new_pad(), os.fspath(output_path))
+        builder.build_all()
+    return output_path
+
+
 @pytest.fixture(scope="function")
 def scratch_builder(tmp_path, scratch_pad):
     output_path = tmp_path / "output"
     output_path.mkdir()
     return Builder(scratch_pad, str(output_path))
 
 
 # Builder for child-sources-test-project, a project to test that child sources
 # are built even if they're filtered out by a pagination query.
 @pytest.fixture(scope="function")
-def child_sources_test_project_builder(tmp_path, data_path):
+def child_sources_test_project_builder(tmp_path, data_path, save_sys_path):
     output_path = tmp_path / "output"
     output_path.mkdir()
     project = Project.from_path(data_path / "child-sources-test-project")
     pad = project.make_env().new_pad()
     return Builder(pad, str(output_path))
 
 
@@ -228,14 +282,14 @@
             shutil.copy2(entry_path, entry)
     return isolated_cli_runner
 
 
 @pytest.fixture
 def no_utils(monkeypatch):
     """Monkeypatch $PATH to hide any installed external utilities
-    (e.g. git, imagemagick)."""
+    (e.g. git, ffmpeg)."""
     monkeypatch.setitem(os.environ, "PATH", "/dev/null")
     locate_executable.cache_clear()
     try:
         yield
     finally:
         locate_executable.cache_clear()
```

### Comparing `lektor-3.4.0b5/tests/test_assets.py` & `lektor-3.4.0b6/tests/test_assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import inspect
+import os
 import shutil
 
 import pytest
 
 from lektor.project import Project
 
 
 def write_text(path, text):
     path.parent.mkdir(parents=True, exist_ok=True)
     path.write_text(inspect.cleandoc(text))
 
 
-def _fixme(*args):
-    return pytest.param(*args, marks=pytest.mark.xfail(reason="FIXME"))
-
-
 @pytest.fixture(scope="module")
 def project_path(tmp_path_factory, data_path):
     """Make our own private copy of the demo-project"""
     demo = data_path / "demo-project"
     path = tmp_path_factory.mktemp("test_serve") / "demo-project"
 
     shutil.copytree(demo, path)
 
     write_text(path / "assets/TEST.TXT", "Text file.\n")
     return path
 
 
 @pytest.fixture
-def pad(project_path):
+def pad(project_path, save_sys_path):
     return Project.from_path(project_path).make_env().new_pad()
 
 
 @pytest.fixture
 def asset(pad, asset_path):
     return pad.get_asset(asset_path)
 
@@ -102,24 +99,31 @@
 def test_asset_get_child(asset, name, from_url, child_name):
     if child_name is None:
         assert asset.get_child(name, from_url) is None
     else:
         assert asset.get_child(name, from_url).name == child_name
 
 
+fs_ignores_case = all(os.path.exists(fn) for fn in (__file__.upper(), __file__.lower()))
+xfail_if_fs_cs = pytest.mark.xfail(
+    not fs_ignores_case,
+    reason="FIXME: fails on case-sensitive filesystems",
+)
+
+
 @pytest.mark.parametrize(
     "asset_path, url_path, expected",
     [
         ("/", ("static",), "/static"),
         ("/", ("static", "demo.css"), "/static/demo.css"),
         ("/", ("missing", "demo.css"), None),
         ("/", ("foo-prefix-makes-me-excluded",), None),
         ("/", ("foo-prefix-makes-me-excluded", "static"), None),
         ("/static", ("demo.css",), "/static/demo.css"),
-        _fixme("/", ("TEST.txt",), "/TEST.txt"),
+        pytest.param("/", ("TEST.txt",), "/TEST.txt", marks=xfail_if_fs_cs),
     ],
 )
 def test_resolve_url_path(asset, url_path, expected):
     if expected is None:
         assert asset.resolve_url_path(url_path) is None
     else:
         assert asset.resolve_url_path(url_path).artifact_name == expected
```

### Comparing `lektor-3.4.0b5/tests/test_build_frontend.py` & `lektor-3.4.0b6/tests/test_build_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     with pytest.raises(SystemExit) as exc_info:
         frontend_build_hook.initialize("standard", build_data={})
     assert exc_info.value.args[0] == 1
 
 
 @pytest.mark.skipif(shutil.which("npm") is None, reason="npm not installed")
 @pytest.mark.requiresinternet
+@pytest.mark.slowtest
 @pytest.mark.usefixtures("frontend_src")
 def test_initialize_builds_frontend(frontend_build_hook, tmp_root):
     frontend_build_hook.initialize("standard", build_data={})
     app_js = tmp_root / "lektor/admin/static/app.js"
     assert app_js.stat().st_size > 1024
```

### Comparing `lektor-3.4.0b5/tests/test_builder.py` & `lektor-3.4.0b6/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from pathlib import Path
 
 import pytest
-from markers import imagemagick
 
 from lektor.reporter import NullReporter
 
 
 def get_child_sources(prog):
     return sorted(list(prog.iter_child_sources()), key=lambda x: x["_id"])
 
 
-@imagemagick
 def test_basic_build(pad, builder):
     root = pad.root
 
     prog, build_state = builder.build(root)
     assert prog.source is root
     assert build_state.failed_artifacts == []
```

### Comparing `lektor-3.4.0b5/tests/test_buildfailures.py` & `lektor-3.4.0b6/tests/test_buildfailures.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_datamodel.py` & `lektor-3.4.0b6/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_db.py` & `lektor-3.4.0b6/tests/test_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -532,7 +532,34 @@
         "hello.txt",  # Attachment
     ],
 )
 def test_Record_contents_is_deprecated(pad, path):
     with pytest.deprecated_call(match=r"contents") as warnings:
         assert isinstance(pad.get(path).contents, FileContents)
     assert all(w.filename == __file__ for w in warnings)
+
+
+@pytest.mark.parametrize(
+    "url, base_url, absolute, external, project_url, expected",
+    [
+        ("/a/b.html", "/a/", None, None, None, "b.html"),
+        ("/a/b/", "/a/", None, None, None, "b/"),
+        ("/a/b/", "/a", None, None, None, "a/b/"),
+        ("/a/b/", "/a", True, None, None, "/a/b/"),
+        ("/a/b/", "/a", True, None, "https://example.net/pfx/", "/pfx/a/b/"),
+        ("/a/b/", "/a", None, True, "https://example.org", "https://example.org/a/b/"),
+    ],
+)
+def test_Pad_make_url(url, base_url, absolute, external, project_url, expected, pad):
+    if project_url is not None:
+        pad.db.config.values["PROJECT"]["url"] = project_url
+    assert pad.make_url(url, base_url, absolute, external) == expected
+
+
+def test_Pad_make_url_raises_runtime_error_if_no_project_url(pad):
+    with pytest.raises(RuntimeError, match="(?i)configure the url in the project"):
+        pad.make_url("/a/b", external=True)
+
+
+def test_Pad_make_url_raises_runtime_error_if_no_base_url(pad):
+    with pytest.raises(RuntimeError, match="(?i)no base url"):
+        pad.make_url("/a/b")
```

### Comparing `lektor-3.4.0b5/tests/test_deploy.py` & `lektor-3.4.0b6/tests/test_deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from os.path import dirname
 from os.path import join
 
 import pytest
-from werkzeug.urls import url_parse
 
 from lektor.publisher import RsyncPublisher
 
 
 def test_get_server(env):
     server = env.load_config().get_server("production")
     assert server.name == "Production"
@@ -14,15 +13,15 @@
     assert server.target == "rsync://myserver.com/path/to/website"
     assert server.extra == {"extra_field": "extra_value"}
 
 
 def test_rsync_command_credentials(tmpdir, mocker, env):
     output_path = tmpdir.mkdir("output")
     publisher = RsyncPublisher(env, str(output_path))
-    target_url = url_parse("http://example.com")
+    target_url = "http://example.com"
     credentials = {
         "username": "fakeuser",
         "password": "fakepass",
     }
     mock_popen = mocker.patch("lektor.publisher.portable_popen")
     with publisher.get_command(target_url, credentials):
         assert mock_popen.called
@@ -155,12 +154,11 @@
                 "/path/to/directory/",
             ],
         ),
     ],
 )
 def test_rsync_publisher(target_url, called_command, tmpdir, mocker, env):
     publisher = RsyncPublisher(env, str(output_path))
-    target_url = url_parse(target_url)
     mock_popen = mocker.patch("lektor.publisher.portable_popen")
     with publisher.get_command(target_url, credentials=None):
         assert mock_popen.called
         assert mock_popen.call_args[0] == (called_command,)
```

### Comparing `lektor-3.4.0b5/tests/test_devcli.py` & `lektor-3.4.0b6/tests/test_devcli.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_editor.py` & `lektor-3.4.0b6/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_imports.py` & `lektor-3.4.0b6/tests/test_imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,10 +30,11 @@
 
 
 @pytest.fixture(params=iter_lektor_modules())
 def module(request):
     return request.param
 
 
+@pytest.mark.slowtest
 def test_import(module):
     python = sys.executable
     assert run([python, "-c", f"import {module}"], check=False).returncode == 0
```

### Comparing `lektor-3.4.0b5/tests/test_issue_410.py` & `lektor-3.4.0b6/tests/test_issue_410.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_markdown.py` & `lektor-3.4.0b6/tests/test_markdown.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import threading
 from typing import Union
 
 import pytest
 from markupsafe import Markup
 
+import lektor.markdown
 from lektor.context import Context
 from lektor.markdown import controller_class
 from lektor.markdown import get_controller
 from lektor.markdown import make_markdown
 from lektor.markdown import Markdown
 from lektor.markdown import markdown_to_html
 from lektor.markdown import MISTUNE_VERSION
@@ -220,33 +221,14 @@
     if MISTUNE_VERSION.startswith("2."):
         from lektor.markdown.mistune2 import ImprovedRenderer
     else:
         from lektor.markdown.mistune0 import ImprovedRenderer
     return ImprovedRenderer()
 
 
-@pytest.mark.skipif(not MISTUNE_VERSION.startswith("0."), reason="not mistune0")
-@pytest.mark.usefixtures("renderer_context")
-def test_ImprovedRenderer_record(record, improved_renderer):
-    with pytest.deprecated_call(
-        match=r"Use .*Renderer\.lektor.record instead"
-    ) as warnings:
-        assert improved_renderer.record is record
-    assert all(w.filename == __file__ for w in warnings)
-
-
-@pytest.mark.skipif(not MISTUNE_VERSION.startswith("0."), reason="not mistune0")
-def test_ImprovedRenderer_meta(renderer_context, improved_renderer):
-    with pytest.deprecated_call(
-        match=r"Use .*Renderer\.lektor.meta instead"
-    ) as warnings:
-        assert improved_renderer.meta is renderer_context.meta
-    assert all(w.filename == __file__ for w in warnings)
-
-
 @pytest.mark.parametrize(
     "link, title, text, expected",
     [
         # NB: Mistune 0.x and mistune 2.x behave differently with
         # respect to how much HTML escaping of the ``link`` the
         # renderer is expected to do.  Do not put HTML-escaping tests
         # here.  Put them in the ``test_integration`` test later in
@@ -287,29 +269,14 @@
     if MISTUNE_VERSION.startswith("2."):
         result = improved_renderer.image(src, alt, title)
     else:
         result = improved_renderer.image(src, title, alt)
     assert re.match(expected, result.rstrip())
 
 
-def test_make_markdown(env):
-    with pytest.deprecated_call() as warnings:
-        md = make_markdown(env)
-    assert all(w.filename == __file__ for w in warnings)
-    assert md("foo").strip() == "<p>foo</p>"
-
-
-@pytest.mark.usefixtures("context")
-def test_markdown_to_html(record, field_options):
-    with pytest.deprecated_call() as warnings:
-        result = markdown_to_html("goober", record, field_options)
-    assert all(w.filename == __file__ for w in warnings)
-    assert result.html.rstrip() == "<p>goober</p>"
-
-
 def plugin_linkcount(md):
     """A test mistune2 plugin.
 
     This replaces ``[link-count]`` in text with the current link count
     wrapped in a <code> element.
     """
 
@@ -492,7 +459,148 @@
 @pytest.mark.usefixtures("context", "link_counter_plugin")
 def test_field_options_integration(record, field_options):
     # tests that we can pass field options to a custom renderer mixin
     field_options = dict(field_options, multiplier="11")
     two_links = "[one](x.html), [two](y.html)"
     markdown = Markdown(two_links, record, field_options)
     assert markdown.meta["nlinks"] == 22
+
+
+################################################################
+#
+# Tests for the bits that are provided for backward compatibility
+# with plugins written for Lektor < 3.4.
+#
+def test_deprecated_ImprovedRenderer(improved_renderer):
+    with pytest.deprecated_call(
+        match=r"lektor\.markdown\.ImprovedRenderer\b.* deprecated"
+    ) as warnings:
+        # pylint: disable-next=import-outside-toplevel,no-name-in-module
+        from lektor.markdown import ImprovedRenderer
+    assert all(w.filename == __file__ for w in warnings)
+    assert ImprovedRenderer is type(improved_renderer)
+
+
+@pytest.mark.skipif(not MISTUNE_VERSION.startswith("0."), reason="not mistune0")
+@pytest.mark.usefixtures("renderer_context")
+def test_deprecated_ImprovedRenderer_record(record):
+    with pytest.deprecated_call():
+        # pylint: disable-next=import-outside-toplevel,no-name-in-module
+        from lektor.markdown import ImprovedRenderer
+    improved_renderer = ImprovedRenderer()
+
+    with pytest.deprecated_call(
+        match=r"Use .*Renderer\.lektor\.record instead"
+    ) as warnings:
+        assert improved_renderer.record is record
+    assert all(w.filename == __file__ for w in warnings)
+
+
+@pytest.mark.skipif(not MISTUNE_VERSION.startswith("0."), reason="not mistune0")
+def test_deprecated_ImprovedRenderer_meta(renderer_context):
+    with pytest.deprecated_call():
+        # pylint: disable-next=import-outside-toplevel,no-name-in-module
+        from lektor.markdown import ImprovedRenderer
+    improved_renderer = ImprovedRenderer()
+
+    with pytest.deprecated_call(
+        match=r"Use .*Renderer\.lektor\.meta instead"
+    ) as warnings:
+        assert improved_renderer.meta is renderer_context.meta
+    assert all(w.filename == __file__ for w in warnings)
+
+
+def test_deprecated_MarkdownConfig(improved_renderer):
+    with pytest.deprecated_call(
+        match=r"lektor\.markdown\.MarkdownConfig\b.* deprecated"
+    ) as warnings:
+        config = lektor.markdown.MarkdownConfig()
+    assert all(w.filename == __file__ for w in warnings)
+    assert config.renderer_base is type(improved_renderer)
+
+
+def test_deprecated_escape(improved_renderer):
+    with pytest.deprecated_call(
+        match=r"lektor\.markdown\.escape\b.* deprecated"
+    ) as warnings:
+        assert lektor.markdown.escape("<") == "&lt;"
+    assert all(w.filename == __file__ for w in warnings)
+
+
+def test_getattr_raises():
+    with pytest.raises(AttributeError, match="no attribute 'goober'"):
+        lektor.markdown.goober  # pylint: disable=pointless-statement
+
+
+def test_dir():
+    expected = {
+        "MISTUNE_VERSION",
+        "Markdown",
+        "get_controller",
+        "escape",
+        "ImprovedRenderer",
+        "MarkdownConfig",
+        "make_markdown",
+        "markdown_to_html",
+    }
+    assert expected.issubset(dir(lektor.markdown))
+
+
+def test_deprecated_make_markdown(env):
+    with pytest.deprecated_call() as warnings:
+        md = make_markdown(env)
+    assert all(w.filename == __file__ for w in warnings)
+    assert md("foo").strip() == "<p>foo</p>"
+
+
+@pytest.mark.usefixtures("context")
+def test_deprecated_markdown_to_html(record, field_options):
+    with pytest.deprecated_call() as warnings:
+        result = markdown_to_html("goober", record, field_options)
+    assert all(w.filename == __file__ for w in warnings)
+    assert result.html.rstrip() == "<p>goober</p>"
+
+
+@pytest.mark.skipif(
+    not MISTUNE_VERSION.startswith("0."),
+    reason="Legacy renderer mixins will only work with mistune 0.x",
+)
+@pytest.mark.usefixtures("context")
+def test_legacy_plugin(env, record, field_options):
+    # Test that Lektor<3.4 style plugin works
+
+    class LegacyPlugin(Plugin):
+        """A legacy, Lektor<3.4, mistune 0.x style plugin."""
+
+        name = "legacy-plugin"
+
+        def on_markdown_config(self, config, **extra):
+            # pylint: disable-next=import-outside-toplevel,no-name-in-module
+            from lektor.markdown import escape
+
+            class LegacyRendererMixin:
+                def link(self, link, title, text):
+                    self.meta["links"].append(link)
+                    self.meta["record"] = self.record
+                    return f'<a href="{escape(link)}">{text}</a>'
+
+            config.renderer_mixins.append(LegacyRendererMixin)
+
+        @staticmethod
+        def on_markdown_meta_init(meta, **extra):
+            meta["links"] = []
+
+        @staticmethod
+        def on_markdown_meta_postprocess(meta, **extra):
+            meta["nlinks"] = len(meta["links"])
+
+    env.plugin_controller.instanciate_plugin("legacy-plugin", LegacyPlugin)
+
+    source = "[`foo`](https://example.org/)"
+    markdown = Markdown(source, record, field_options)
+
+    with pytest.deprecated_call():
+        assert markdown["record"] is record
+    assert markdown["links"] == ["https://example.org/"]
+    assert markdown["nlinks"] == 1
+    html = markdown.__html__().rstrip()
+    assert html == '<p><a href="https://example.org/"><code>foo</code></a></p>'
```

### Comparing `lektor-3.4.0b5/tests/test_packages.py` & `lektor-3.4.0b6/tests/test_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 def test_VirtualEnv_addsitedir(nested_venv: VirtualEnv) -> None:
     # check that we can run pytest (presumably from our site-packages)
     proc = run((nested_venv.executable, "-m", "pytest", "--version"), check=False)
     assert proc.returncode == 0
 
 
 @pytest.mark.requiresinternet
+@pytest.mark.slowtest
 def test_VirtualEnv_run_pip_install(tmp_path: Path) -> None:
     # XXX: slow test
     venv = VirtualEnv(tmp_path)
     venv.create()
 
     # install a dummy plugin
     plugin_path = Path(__file__).parent / "pep660-dummy-plugin"
```

### Comparing `lektor-3.4.0b5/tests/test_pagination.py` & `lektor-3.4.0b6/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_pluginsystem.py` & `lektor-3.4.0b6/tests/test_pluginsystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,25 @@
         return None
 
     def find_distributions(self, context=metadata.DistributionFinder.Context()):
         return [self.distribution]
 
 
 @pytest.fixture
-def dummy_plugin_distribution(save_sys_path, monkeypatch):
+def dummy_plugin_distribution(save_sys_path):
     """Add a dummy plugin distribution to the current working_set."""
     dist = DummyDistribution(
         {
             "Name": "lektor-dummy-plugin",
             "Version": "1.23",
         }
     )
     finder = DummyPluginFinder(__name__, dist)
-    monkeypatch.setattr("sys.meta_path", [finder] + sys.meta_path)
+    # The save_sys_path fixture will restore meta_path at end of test
+    sys.meta_path.insert(0, finder)
     return dist
 
 
 @pytest.fixture
 def dummy_plugin(env, dummy_plugin_distribution):
     """Instantiate and register a dummy plugin in env"""
     env.plugin_controller.instanciate_plugin(
@@ -193,14 +194,15 @@
         plugin = env.plugins["dummy-plugin"]
         assert plugin.version is None
 
     def test_path(self, dummy_plugin):
         assert dummy_plugin.path == str(Path(__file__).parent)
 
     @pytest.mark.requiresinternet
+    @pytest.mark.slowtest
     @pytest.mark.usefixtures("save_sys_path")
     def test_path_installed_plugin_is_none(self, scratch_project):
         # XXX: this test is slow and fragile. (It won't run
         # without an internet connection.)
         add_package_to_project(scratch_project, "webpack-support")
         env = scratch_project.make_env()
         plugin = get_plugin("webpack-support", env)
```

### Comparing `lektor-3.4.0b5/tests/test_prev_next_sibling.py` & `lektor-3.4.0b6/tests/test_prev_next_sibling.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     src = data_path / "dependency-test-project"
     tmp_project = tmp_path / "project"
     shutil.copytree(src, tmp_project)
     return Project.from_path(tmp_project)
 
 
 @pytest.fixture
-def pntest_env(pntest_project):
+def pntest_env(pntest_project, save_sys_path):
     return Environment(pntest_project)
 
 
 @pytest.fixture
 def pntest_pad(pntest_env):
     return Database(pntest_env).new_pad()
```

### Comparing `lektor-3.4.0b5/tests/test_publisher.py` & `lektor-3.4.0b6/tests/test_publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 from shutil import which
 from subprocess import CalledProcessError
 from subprocess import DEVNULL
 from subprocess import PIPE
 from subprocess import run
 
 import pytest
-from werkzeug.urls import url_parse
 
+from lektor.publisher import _CompatURLStr
 from lektor.publisher import _ssh_command
 from lektor.publisher import _ssh_key_file
 from lektor.publisher import Command
 from lektor.publisher import GithubPagesPublisher
 from lektor.publisher import GitRepo
 from lektor.publisher import publish
+from lektor.publisher import Publisher
 from lektor.publisher import PublishError
 from lektor.utils import locate_executable
 
 
 def test_ssh_key_file():
     credentials = {"key_file": "/some/id", "key": "rsa:ignored"}
     with _ssh_key_file(credentials) as key_file:
@@ -466,19 +467,18 @@
     ghp_publisher, output_path, mocker, target_url, publish_args, warns
 ):
     GitRepo = mocker.patch("lektor.publisher.GitRepo", spec_set=True)
     repo = mocker.Mock(spec_set=dir(GitRepo))
     repo.publish_ghpages.return_value = iter(["Published!"])
     GitRepo.return_value.__enter__.return_value = repo
 
-    url = url_parse(target_url)
     with ExitStack() as stack:
         if warns:
             stack.enter_context(pytest.deprecated_call())
-        output = list(ghp_publisher.publish(url))
+        output = list(ghp_publisher.publish(target_url))
 
     GitRepo.assert_called_once_with(output_path)
     if "+https:" in target_url:
         repo.set_https_credentials.assert_called_once_with({})
     else:
         repo.set_ssh_credentials.assert_called_once_with({})
     repo.publish_ghpages.assert_called_once_with(*publish_args)
@@ -486,17 +486,17 @@
         assert "WARNING" in " ".join(output)
         output = output[-1:]
     assert output == ["Published!"]
 
 
 @pytest.mark.usefixtures("no_utils")
 def test_GithubPagesPublisher_publish_fails_if_no_git(ghp_publisher):
-    url = url_parse("ghpages://owner/project")
+    target_url = "ghpages://owner/project"
     with pytest.raises(PublishError) as exc_info:
-        list(ghp_publisher.publish(url))
+        list(ghp_publisher.publish(target_url))
     assert re.search(r"git.*not found", str(exc_info.value))
 
 
 @pytest.mark.parametrize(
     "target_url, expected",
     [
         (
@@ -540,23 +540,22 @@
         (
             "ghpages+https://own:443/proj",
             ("https://github.com/own/proj.git", "gh-pages", None, True, []),
         ),
     ],
 )
 def test_GithubPagesPublisher_parse_url(ghp_publisher, target_url, expected):
-    url = url_parse(target_url)
-    assert ghp_publisher._parse_url(url) == expected
+    assert ghp_publisher._parse_url(target_url) == expected
 
 
 def test_GithubPagesPublisher_parse_url_warns_on_default_master_branch(ghp_publisher):
-    url = url_parse("ghpages://owner/owner.github.io")
+    target_url = "ghpages://owner/owner.github.io"
     with pytest.deprecated_call():
         push_url, branch, cname, preserve_history, warnings = ghp_publisher._parse_url(
-            url
+            target_url
         )
     assert (push_url, branch, cname, preserve_history) == (
         "ssh://git@github.com/owner/owner.github.io.git",
         "master",
         None,
         True,
     )
@@ -570,17 +569,16 @@
         ("ghpages:///project", "owner missing"),
         ("ghpages://owner", "project missing"),
         ("ghpages://owner:2222/project", "non-standard port"),
         ("ghpages+https://owner:4430/project", "non-standard port"),
     ],
 )
 def test_GithubPagesPublisher_parse_url_failures(ghp_publisher, target_url, expected):
-    url = url_parse(target_url)
     with pytest.raises(PublishError) as exc_info:
-        ghp_publisher._parse_url(url)
+        ghp_publisher._parse_url(target_url)
     assert expected in str(exc_info.value)
 
 
 @pytest.mark.parametrize(
     "target_url, credentials, expected",
     [
         ("ghpages://owner/proj", None, {}),
@@ -602,28 +600,61 @@
             {"username": "user", "password": "secret"},
         ),
     ],
 )
 def test_GithubPagesPublisher_parse_credentials(
     ghp_publisher, credentials, target_url, expected
 ):
-    url = url_parse(target_url)
-    assert ghp_publisher._parse_credentials(credentials, url) == expected
+    assert ghp_publisher._parse_credentials(credentials, target_url) == expected
 
 
 def test_publish(env, output_path, mocker):
     Publisher = mocker.Mock()
     env.add_publisher("publishtest", Publisher)
     credentials = {"foo": "bar"}
     rv = publish(env, "publishtest://host/path", output_path, credentials)
-    url = url_parse("publishtest://host/path")
+    target_url = "publishtest://host/path"
     assert Publisher.mock_calls == [
         mocker.call(env, output_path),
-        mocker.call().publish(url, credentials),
+        mocker.call().publish(target_url, credentials),
     ]
     assert rv is Publisher.return_value.publish.return_value
 
 
 def test_publish_unknown_scheme(env, output_path):
     with pytest.raises(PublishError) as exc_info:
         publish(env, "unknownscheme://host/path", output_path)
     assert "unknown scheme" in str(exc_info.value)
+
+
+def test_publish_old_plugin(env, output_path, mocker):
+    target_url = "publishtest://Bücher.example/?foo=bar"
+
+    class OldPublisher(Publisher):
+        # pylint: disable=signature-differs
+        def publish(self, target_url, credentials, **extra):
+            return target_url
+
+    env.add_publisher("publishtest", OldPublisher)
+    compat_url = publish(env, target_url, output_path, credentials={})
+
+    assert isinstance(compat_url, _CompatURLStr)
+
+
+def test_CompatURLStr_is_str():
+    url = _CompatURLStr(" scheme://example.org/ ")
+    assert isinstance(url, str)
+    assert str(url) == " scheme://example.org/ "
+
+
+def test_CompatURLStr_raises_attribute_error():
+    url = _CompatURLStr("scheme://example.org/")
+    with pytest.raises(AttributeError):
+        url._replace()
+
+
+def test_CompatURLStr_works_as_URL():
+    url = _CompatURLStr("scheme:///path?foo=bar")
+    with pytest.deprecated_call() as w:
+        warnings.filterwarnings("ignore", "'werkzeug", DeprecationWarning)
+        assert dict(url.decode_query()) == {"foo": "bar"}
+    assert w[0].filename == __file__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lektor-3.4.0b5/tests/test_quickstart.py` & `lektor-3.4.0b6/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_sourceobj.py` & `lektor-3.4.0b6/tests/test_sourceobj.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_themes.py` & `lektor-3.4.0b6/tests/test_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
     lektorfile = theme_project_tmpdir / "themes.lektorproject"
     lektorfile.write_text(lektorfile_text, "utf8")
     return Project.from_path(theme_project_tmpdir)
 
 
 @pytest.fixture(scope="function")
-def theme_env(theme_project):
+def theme_env(theme_project, save_sys_path):
 
     return Environment(theme_project)
 
 
 @pytest.fixture(scope="function")
 def theme_pad(theme_env):
```

### Comparing `lektor-3.4.0b5/tests/test_tree.py` & `lektor-3.4.0b6/tests/test_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 import pytest
 
 from lektor.constants import PRIMARY_ALT
 from lektor.db import Tree
 from lektor.project import Project
 
+# pylint: disable-next=wrong-import-order
+from conftest import restore_import_state  # noreorder
+
 
 @pytest.fixture(scope="session")
 def no_alt_pad(tmp_path_factory, data_path):
     no_alt_project = tmp_path_factory.mktemp("no-alts") / "demo-project"
     demo_project = data_path / "demo-project"
     shutil.copytree(demo_project, no_alt_project)
 
@@ -25,15 +28,16 @@
         for child in dirs.pop().iterdir():
             if child.is_dir():
                 dirs.append(child)
             elif child.match("contents+*.lr"):
                 child.unlink()
 
     project = Project.from_path(no_alt_project)
-    return project.make_env().new_pad()
+    with restore_import_state():
+        return project.make_env().new_pad()
 
 
 @pytest.fixture(params=[False, True])
 def disable_alternatives(request):
     return request.param
 
 
@@ -212,15 +216,15 @@
     children = item.get_children(offset, limit, order_by=order_by)
     assert list(child.id for child in children) == expect
 
 
 @pytest.mark.parametrize(
     "disable_alternatives, path, order_by, expect",
     [
-        (False, "/", None, ["blog", "extra", "projects"]),
+        (False, "/", None, ["blog", "colorspace-test", "extra", "projects"]),
         (False, "/blog", ("-pub_date",), ["post2", "post1", "dummy.xml"]),
         (
             False,
             "/projects",
             ("seq",),
             [
                 "zaun",
@@ -248,15 +252,15 @@
                 "postage",
                 "secret",
                 "slave",
                 "wolf",
                 "zaun",
             ],
         ),
-        (True, "/", None, ["blog", "extra", "projects"]),
+        (True, "/", None, ["blog", "colorspace-test", "extra", "projects"]),
         (True, "/blog", ("-pub_date",), ["post2", "post1", "dummy.xml"]),
     ],
 )
 def test_tree_item_iter_subpages(tree, path, order_by, expect):
     item = tree.get(path)
     assert list(child.id for child in item.iter_subpages(order_by)) == expect
```

### Comparing `lektor-3.4.0b5/tests/test_types.py` & `lektor-3.4.0b6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/test_unicode.py` & `lektor-3.4.0b6/tests/test_unicode.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from lektor.build_programs import BuildError
 from lektor.builder import Builder
 from lektor.project import Project
 from lektor.reporter import BufferReporter
 
 
 @pytest.fixture
-def pad(data_path):
+def pad(data_path, save_sys_path):
     proj = Project.from_path(data_path / "ünicöde-project")
     return proj.make_env().new_pad()
 
 
 @pytest.fixture
 def builder(pad, tmp_path):
     output_path = tmp_path / "output"
```

### Comparing `lektor-3.4.0b5/tests/test_urls.py` & `lektor-3.4.0b6/tests/test_urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 import re
 
 import pytest
 
 from lektor.context import _ctx_stack
 from lektor.context import Context
+from lektor.environment import Environment
+from lektor.reporter import BufferReporter
+from lektor.sourceobj import VirtualSourceObject
 from lektor.utils import cleanup_path
 from lektor.utils import cleanup_url_path
 
+# noreorder
+from conftest import restore_import_state  # pylint: disable=wrong-import-order
+
+
+@pytest.fixture(scope="module")
+def pad(project):
+    # Use a module-scoped pad to speed tests
+    with restore_import_state():
+        return Environment(project).new_pad()
+
+
+@pytest.fixture
+def config(pad, monkeypatch):
+    """Patch a function-scoped config into our session-scoped pad.
+
+    (For those tests/fixtures that want to mangle the config.)
+    """
+    config = pad.db.env.load_config()
+    monkeypatch.setattr(pad.db, "config", config)
+    return config
+
 
 @pytest.mark.parametrize(
     "path, expected",
     [
         ("", "/"),
         ("/", "/"),
         ("/foo", "/foo"),
@@ -112,20 +136,20 @@
     finally:
         _ctx_stack.pop()
 
 
 def test_url_to_thumbnail(pad, mock_build_context):
     extra_de = pad.get("/extra", alt="de")
     thumbnail = pad.get("/test.jpg").thumbnail(42)
-    assert extra_de.url_to(thumbnail) == "../../test@42.jpg"
+    assert extra_de.url_to(thumbnail) == "../../test@42x56.jpg"
 
 
 @pytest.fixture
-def external_url(pad):
-    pad.config.values["PROJECT"]["url"] = "http://example.org/site/"
+def external_url(config):
+    config.values["PROJECT"]["url"] = "http://example.org/site/"
 
 
 @pytest.mark.parametrize(
     "path, kwargs, expected",
     [
         ("/projects/slave", {}, "../slave/"),
         ("/projects/slave", {"absolute": True}, "/site/projects/slave/"),
@@ -168,14 +192,16 @@
         ("./", {}, "./"),
         ("../", {}, "../"),
         ("../wolf", {}, "./"),
         ("../wolf/", {}, "./"),
         ("../wolf/.", {}, "./"),
         ("../slave", {}, "../slave/"),
         ("../wolf/../slave/", {}, "../slave/"),
+        ("/", {}, "../../"),
+        ("/extra", {}, "../../extra/"),
         ("/projects/wolf", {}, "./"),
         ("/projects/slave", {}, "../slave/"),
         # Test alt
         (".", {"alt": "de"}, "../../de/projects/wolf/"),
         ("../slave", {"alt": "de"}, "../../de/projects/sklave/"),
         ("/projects/wolf", {"alt": "de"}, "../../de/projects/wolf/"),
         ("/projects/slave", {"alt": "de"}, "../../de/projects/sklave/"),
@@ -328,7 +354,76 @@
     record = pad.get("/extra/file.ext")
     assert record.url_path == "/extra/file.ext"
 
 
 def test_url_with_slash_slug(pad):
     record = pad.get("/extra/slash-slug")
     assert record.url_path == "/extra/long/path/"
+
+
+class DummyVirtualSource(VirtualSourceObject):
+    url_path = None  # mask inherited property
+
+    def __init__(self, record, url_path):
+        super().__init__(record)
+        self.url_path = url_path
+
+    @property
+    def url_content_path(self):
+        # This is a url_content_path that is appropriate for a
+        # source object that can contain other child source objects
+        if self.url_path.endswith("/"):
+            return self.url_path
+        head, sep, tail = self.url_path.rpartition("/")
+        return f"{head}{sep}_{tail}/"
+
+    @property
+    def path(self):
+        return f"{self.record.path}@virtual"
+
+
+@pytest.mark.parametrize(
+    "path, url_path, expected",
+    [
+        ("/", "/path/virtual/", "../../"),
+        ("/index.html", "/path/virtual/", "../../index.html"),
+        ("rel", "/path/virtual/", "rel"),
+        ("rel", "/path/virtual.html", "_virtual.html/rel"),
+    ],
+)
+def test_url_from_virtual(pad, path, url_path, expected):
+    virtual = DummyVirtualSource(pad.get("/extra"), url_path)
+    assert virtual.url_to(path) == expected
+
+
+@pytest.mark.parametrize(
+    "path, expected",
+    [
+        ("a", "_file.ext/a"),
+        ("/", "../"),
+        ("/projects", "../projects/"),
+    ],
+)
+def test_url_from_page_with_dotted_name(pad, path, expected):
+    record = pad.get("/extra/file.ext")
+    assert record.url_to(path) == expected
+
+
+@pytest.mark.parametrize(
+    "path, expected",
+    [
+        ("a", "a"),
+        ("/", "../"),
+        ("/projects", "../projects/"),
+    ],
+)
+def test_url_from_attachment(pad, path, expected):
+    record = pad.get("/extra/hello.txt")
+    assert record.url_to(path) == expected
+
+
+def test_url_from_attachment_issues_warning(pad):
+    record = pad.get("/extra/hello.txt")
+    with BufferReporter(pad.env) as reporter:
+        assert record.url_to("a") == "a"
+    message = next(filter(None, (extra.get("message") for _, extra in reporter.buffer)))
+    assert re.match(r"(?i)Suspicious use of relative URL", message)
```

### Comparing `lektor-3.4.0b5/tests/test_videotools.py` & `lektor-3.4.0b6/tests/test_videotools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/admin/test_api.py` & `lektor-3.4.0b6/tests/admin/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,14 @@
     [
         ("/", {"GET"}),
         ("/admin/api/recordinfo?path=%2F", {"GET"}),
         ("/admin/api/clean", {"POST"}),
         ("/admin/api/rawrecord", {"GET", "PUT"}),
     ],
 )
-@pytest.mark.parametrize("method", {"GET", "POST", "PUT"})
+@pytest.mark.parametrize("method", ["GET", "POST", "PUT"])
 def test_allowed_methods(test_client, method, url, allowed):
     if method not in allowed:
         extra_allowed = {"OPTIONS", "HEAD"} if "GET" in allowed else {"OPTIONS"}
         resp = test_client.open(url, method=method)
         assert resp.status_code == 405
         assert set(resp.allow) == allowed | extra_allowed
```

### Comparing `lektor-3.4.0b5/tests/admin/test_dash.py` & `lektor-3.4.0b6/tests/admin/test_dash.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/admin/test_serve.py` & `lektor-3.4.0b6/tests/admin/test_serve.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/admin/test_webui.py` & `lektor-3.4.0b6/tests/admin/test_webui.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/demo-project/content/test-progressive.jpg` & `lektor-3.4.0b6/tests/demo-project/content/test-progressive.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/demo-project/content/test-sof-last.jpg` & `lektor-3.4.0b6/tests/demo-project/content/test-sof-last.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/demo-project/content/test.jpg` & `lektor-3.4.0b6/tests/demo-project/content/test.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/demo-project/content/test.mp4` & `lektor-3.4.0b6/tests/demo-project/content/test.mp4`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/tests/demo-project/templates/page.html` & `lektor-3.4.0b6/tests/demo-project/templates/page.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/LICENSE` & `lektor-3.4.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/README.md` & `lektor-3.4.0b6/README.md`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b5/pyproject.toml` & `lektor-3.4.0b6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -42,20 +42,21 @@
     "importlib_metadata; python_version<'3.8'",
     "inifile>=0.4.1",
     "Jinja2>=3.0",
     "MarkupSafe",
     "marshmallow",
     "marshmallow_dataclass>=8.5.9",
     "mistune>=0.7.0,<3",
+    "Pillow>=6",
     "pip",
     "python-slugify",
     "pytz; python_version<'3.9'",  # favor zoneinfo for python>=3.9
     "requests",
     "tzdata; python_version>='3.9' and sys_platform == 'win32'",
-    "watchdog",
+    "watchfiles",
     "Werkzeug>=2.1.0,<3",
 ]
 optional-dependencies.ipython = [
     "ipython",
     "traitlets",
 ]
 
@@ -92,14 +93,15 @@
 # pytest
 #
 [tool.pytest.ini_options]
 norecursedirs = ["venv", ".tox", ".git", "node_modules"]
 addopts = "--strict-markers"
 markers = [
     "requiresinternet: marks tests requiring an internet connection",
+    "slowtest: marks particularly slow tests that do not need to be run for every testenv variant",
 ]
 
 
 ################################################################
 #
 # coverage
 #
@@ -183,29 +185,43 @@
 
 # We have just started to add annotation.  For now, ignore all errors
 # by default. (This can be disabled on a per-package or per-module
 # basis in the overrides.)
 ignore_errors = true
 
 [[tool.mypy.overrides]]
+module = [
+    "filetype",
+]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 # Packages and modules we want to check
 module = [
     "lektor.constants",
     "lektor.packages",
     "lektor.admin.*",
+    "lektor.imagetools",
     "test_packages",
 ]
 ignore_errors = false
 
 [[tool.mypy.overrides]]
 module = [
     "lektor.packages",
 ]
 disallow_untyped_defs = false
 disallow_untyped_calls = false
 
 [[tool.mypy.overrides]]
 module = [
     "lektor.admin.*",
+    "lektor.imagetools",
 ]
 disallow_untyped_calls = false
 warn_return_any = false
+
+[[tool.mypy.overrides]]
+module = [
+    "lektor.imagetools",
+]
+disallow_untyped_defs = false
```

### Comparing `lektor-3.4.0b5/PKG-INFO` & `lektor-3.4.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lektor
-Version: 3.4.0b5
+Version: 3.4.0b6
 Summary: A static content management system.
 Project-URL: Homepage, https://www.getlektor.com/
 Project-URL: Source, https://github.com/lektor/lektor/
 Project-URL: Documentation, https://www.getlektor.com/docs/
 Project-URL: Changelog, https://github.com/lektor/lektor/blob/master/CHANGES.md
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 License: Copyright (c) 2015-2016 by the Armin Ronacher.
@@ -60,20 +60,21 @@
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: inifile>=0.4.1
 Requires-Dist: jinja2>=3.0
 Requires-Dist: markupsafe
 Requires-Dist: marshmallow
 Requires-Dist: marshmallow-dataclass>=8.5.9
 Requires-Dist: mistune<3,>=0.7.0
+Requires-Dist: pillow>=6
 Requires-Dist: pip
 Requires-Dist: python-slugify
 Requires-Dist: pytz; python_version < '3.9'
 Requires-Dist: requests
 Requires-Dist: tzdata; python_version >= '3.9' and sys_platform == 'win32'
-Requires-Dist: watchdog
+Requires-Dist: watchfiles
 Requires-Dist: werkzeug<3,>=2.1.0
 Provides-Extra: ipython
 Requires-Dist: ipython; extra == 'ipython'
 Requires-Dist: traitlets; extra == 'ipython'
 Description-Content-Type: text/markdown
 
 # Lektor
```

