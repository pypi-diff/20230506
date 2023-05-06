# Comparing `tmp/almoststatic-1.0.1.tar.gz` & `tmp/almoststatic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almoststatic-1.0.1.tar", last modified: Sat Apr  8 18:13:43 2023, max compression
+gzip compressed data, was "almoststatic-1.0.2.tar", last modified: Sat May  6 15:48:53 2023, max compression
```

## Comparing `almoststatic-1.0.1.tar` & `almoststatic-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.442071 almoststatic-1.0.1/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.1/LICENSE
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-04-08 18:13:43.442071 almoststatic-1.0.1/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5326 2023-03-21 17:43:21.000000 almoststatic-1.0.1/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.438071 almoststatic-1.0.1/almoststatic/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    28214 2023-04-08 09:46:31.000000 almoststatic-1.0.1/almoststatic/__init__.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.442071 almoststatic-1.0.1/almoststatic.egg-info/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.1/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-04-08 18:13:43.442071 almoststatic-1.0.1/setup.cfg
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.2/LICENSE
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-05-06 15:48:53.446243 almoststatic-1.0.2/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5299 2023-05-06 13:04:22.000000 almoststatic-1.0.2/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/almoststatic/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    29838 2023-05-06 13:05:10.000000 almoststatic-1.0.2/almoststatic/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/almoststatic.egg-info/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.2/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-05-06 15:48:53.446243 almoststatic-1.0.2/setup.cfg
```

### Comparing `almoststatic-1.0.1/LICENSE` & `almoststatic-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `almoststatic-1.0.1/PKG-INFO` & `almoststatic-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
@@ -24,15 +24,16 @@
 
 # Almoststatic
 
 **Almoststatic** is a static sites and web pages generator engine written in
 [Python](https://python.org) which uses the
 [Jinja2 template system](https://jinja.palletsprojects.com) to render pages.
 It can be integrated with [Flask](https://flask.palletsprojects.com) apps to
-serve static contents on dynamic sites or used only for static sites development.
+serve static contents on dynamic sites or can be used stand alone for static
+sites development.
 
 Pages are declared in [yaml](https://yaml.org/) files and rendered with Jinja2
 template files, the html contents can be written in [markdown](https://www.markdownguide.org/)
 markup language or in plain html. "content" folder contains all data needed to
 do the job, the "config.yaml" is used to share global parameters and to setup
 configuration.
 
@@ -141,21 +142,21 @@
 
 Now if you decide that **Almoststatic** is right for you, you can dig into
 source code of sample and tests and read the documentation at:
 [https://almoststatic.readthedocs.io](https://almoststatic.readthedocs.io)
 
 # Status of project
 
-Almoststatic is young but stable! It has all planed features and always gave me
-the right results.
+Almoststatic is young but stable! It has all planned features and always gave me
+the right results so it can be considered "production ready"
 
-At the moment there are only one theme which is ready for production, anyway it
-is a developing theme. You can see a demo on
-[http://flatstep.claudiodriussi.it/](http://flatstep.claudiodriussi.it/)
-and download source from [Flatstep theme repository](https://gitlab.com/almoststatic-themes/flatstep)
+At the moment there are only a few themes, we are developing a "rolling theme"
+with some beautiful widgets ready to use.
+See [Flatstep theme](https://gitlab.com/almoststatic-themes/flatstep)
+and follow the tutorial.
 
 I'm not a designer so the result is of average quality. But I'm sure that good
 designers can write great themes.
 
 
 # Donate
```

### Comparing `almoststatic-1.0.1/README.md` & `almoststatic-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Almoststatic
 
 **Almoststatic** is a static sites and web pages generator engine written in
 [Python](https://python.org) which uses the
 [Jinja2 template system](https://jinja.palletsprojects.com) to render pages.
 It can be integrated with [Flask](https://flask.palletsprojects.com) apps to
-serve static contents on dynamic sites or used only for static sites development.
+serve static contents on dynamic sites or can be used stand alone for static
+sites development.
 
 Pages are declared in [yaml](https://yaml.org/) files and rendered with Jinja2
 template files, the html contents can be written in [markdown](https://www.markdownguide.org/)
 markup language or in plain html. "content" folder contains all data needed to
 do the job, the "config.yaml" is used to share global parameters and to setup
 configuration.
 
@@ -117,21 +118,21 @@
 
 Now if you decide that **Almoststatic** is right for you, you can dig into
 source code of sample and tests and read the documentation at:
 [https://almoststatic.readthedocs.io](https://almoststatic.readthedocs.io)
 
 # Status of project
 
-Almoststatic is young but stable! It has all planed features and always gave me
-the right results.
+Almoststatic is young but stable! It has all planned features and always gave me
+the right results so it can be considered "production ready"
 
-At the moment there are only one theme which is ready for production, anyway it
-is a developing theme. You can see a demo on
-[http://flatstep.claudiodriussi.it/](http://flatstep.claudiodriussi.it/)
-and download source from [Flatstep theme repository](https://gitlab.com/almoststatic-themes/flatstep)
+At the moment there are only a few themes, we are developing a "rolling theme"
+with some beautiful widgets ready to use.
+See [Flatstep theme](https://gitlab.com/almoststatic-themes/flatstep)
+and follow the tutorial.
 
 I'm not a designer so the result is of average quality. But I'm sure that good
 designers can write great themes.
 
 
 # Donate
```

### Comparing `almoststatic-1.0.1/almoststatic/__init__.py` & `almoststatic-1.0.2/almoststatic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,23 @@
 
         self.cache = True
         """bool: global enable or disable cache"""
 
         self.quote_escape = '^^'
         """str: sequence for quote escape in markdown translation"""
 
+        self.macros = {}
+        """dict: macros substituted at runtime keys will be substituted with
+                 values and then the content will be rendered."""
+
+        self.md_extensions = ['tables', 'fenced_code', 'attr_list',
+                              'admonition']
+        """list: list of extensions enabled for markdown rendering, this let
+                 you to add your extensions"""
+
         # ------------------------------------------------------ runtime fields
         self.media_prefix = None
         """str | None: starting directory name to force url location for media
                        files when writing static pages"""
 
         self.cached = {}
         """dict: list of cached pages, recalculated only once"""
@@ -100,14 +109,15 @@
         self.content = config['config'].get("content", self.content)
         self.templates = config['config'].get("templates", self.templates)
         self.templ_name = config['config'].get("templ_name", self.templ_name)
         self.pages = config['config'].get("pages", self.pages)
         self.media = config['config'].get("media", self.media)
         self.static_url = config['config'].get("static_url", self.static_url)
         self.cache = config['config'].get("cache", self.cache)
+        self.macros = config['config'].get("macros", {})
 
         # set the environment and add globals
         self.env = Environment(
             loader=FileSystemLoader(self.templates),
             autoescape=False
         )
         # set globals shortcut
@@ -198,14 +208,22 @@
             self.extra_args = kwargs
             self.page = page
             templ_name = page.get('templ_name', None)
             content = self.render_content(
                 page['content'], page.get('widgets_envelope'))
             content = self.render_template(
                 templ_name=templ_name, content=content)
+            # substitute macros keys with values, first are evaluated page
+            # macros and the the global macros declared in config file.
+            for k, v in self.page.get('macros', {}).items():
+                content = content.replace(k,
+                                          self.get_markdown(v, strip_p=True))
+            for k, v in self.macros.items():
+                content = content.replace(k,
+                                          self.get_markdown(v, strip_p=True))
             # template commands can be embedded within html and md and this is
             # the last rendering which evaluate them
             template = self.env.from_string(content)
             content = template.render(page=page, **kwargs)
             if self.cache and page.get('cacheable', True):
                 self.cached[pagename] = (time.time(), content)
         return content
@@ -312,51 +330,70 @@
                                      self.content, self.media])
         else:
             media_prefix = self._relative_url() + self.media
         filename = '/'.join([media_prefix, media_obj])
         return filename
 
     def get_url(self, page):
-        """Build the url for local links adding prefix and suffix to the page,
-        used inside templates write local url's consistent in dynamic and
-        static sites. Recognize the anchor separator to add suffix before it.
+        """Build the url. If the page parameter contain the colon symbol ":" it
+        is an external link and it is returned as is, otherwise it is an local
+        link and add prefix and suffix to the page to be consistent in dynamic
+        and static sites. It also recognize the anchor separator to add suffix
+        before it.
 
         Args:
-            page (str): local url
+            page (str): local or external url
 
         Returns:
-            str: the url for internal link
+            str: the recalculated url
         """
+        if ':' in page:
+            return page
         try:
             i = page.index('#')
             anchor = page[i:]
             page = page[:i]
         except ValueError:
             anchor = ''
         suffix = self.vars['url_suffix']
         return f"{self._relative_url()}{page}{suffix}{anchor}"
 
-    def get_markdown(self, text):
+    def get_markdown(self, text, strip_p=False):
         """convert markdown to html with tables extension.
 
-        double quote and single quotes by default can be escaped with "^^"
+        Double quote and single quotes by default can be escaped with "^^"
         sequence, this let to insert Jinja2 commands within links.
         In markdown `[My Page]({{get_url("mylink")}})` produce an error because
         markdown uses quotes to identify title attribute. So it can be
-        substituted with `[My Page]({{get_url(``mylink``)}})`. This mean that
-        you can use the sequence "``" only for links.
+        substituted with `[My Page]({{get_url(^^mylink^^)}})`. This mean that
+        you can use the sequence "^^" only for links.
+
+        Usually markdown surround text within a paragraph tag <p></p> this is
+        not desired in macros because usually they are inline, so we have a
+        parameter to strip them out.
 
         Args:
             text (str): the text in markdown format
+            strip_p (bool): strip paragraph tag from evaluated markdown
+
         Returns:
             str: the converted text
         """
         quote_marker = '\\:'
         text = text.replace(self.quote_escape, quote_marker)
-        text = markdown.markdown(text, extensions=['tables', 'fenced_code'])
+        text = markdown.markdown(text, extensions=self.md_extensions)
+
+        if strip_p:
+            try:
+                if text.index('<p>') == 0:
+                    end = text.rindex('</p>')
+                    text = text[3:end]
+            except Exception:
+                pass
+
         return text.replace(quote_marker, "'")
 
     def _relative_url(self):
         """"""
         if self.vars['url_prefix']:
             return self.vars['url_prefix']
         return '../' * self.page['pagename'].count('/')
@@ -589,17 +626,18 @@
         """
         for content in self.page[key]:
             if content['id'] == name:
                 return self.render_content(content)
 
     def eval_widget(self, value, key=''):
         """Eval a single widget searching for a 'text' key which contain the
-        text render. If the text is a string it is always rendered as markdown,
-        if text is a dict, it can contain the key 'include' which allow to
-        include a file and/or 'content' which is rendered as a page content
+        text to render. If the text is a string it is always rendered as
+        markdown, if text is a dict, it can contain the key 'include' which
+        allow to include a file and/or 'content' which is rendered as a page
+        content
         """
         if isinstance(value, list):
             for i, v in enumerate(value):
                 value[i] = self.eval_widget(v)
         if isinstance(value, dict):
             for k, v in value.items():
                 value[k] = self.eval_widget(v, k)
```

### Comparing `almoststatic-1.0.1/almoststatic.egg-info/PKG-INFO` & `almoststatic-1.0.2/almoststatic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
@@ -24,15 +24,16 @@
 
 # Almoststatic
 
 **Almoststatic** is a static sites and web pages generator engine written in
 [Python](https://python.org) which uses the
 [Jinja2 template system](https://jinja.palletsprojects.com) to render pages.
 It can be integrated with [Flask](https://flask.palletsprojects.com) apps to
-serve static contents on dynamic sites or used only for static sites development.
+serve static contents on dynamic sites or can be used stand alone for static
+sites development.
 
 Pages are declared in [yaml](https://yaml.org/) files and rendered with Jinja2
 template files, the html contents can be written in [markdown](https://www.markdownguide.org/)
 markup language or in plain html. "content" folder contains all data needed to
 do the job, the "config.yaml" is used to share global parameters and to setup
 configuration.
 
@@ -141,21 +142,21 @@
 
 Now if you decide that **Almoststatic** is right for you, you can dig into
 source code of sample and tests and read the documentation at:
 [https://almoststatic.readthedocs.io](https://almoststatic.readthedocs.io)
 
 # Status of project
 
-Almoststatic is young but stable! It has all planed features and always gave me
-the right results.
+Almoststatic is young but stable! It has all planned features and always gave me
+the right results so it can be considered "production ready"
 
-At the moment there are only one theme which is ready for production, anyway it
-is a developing theme. You can see a demo on
-[http://flatstep.claudiodriussi.it/](http://flatstep.claudiodriussi.it/)
-and download source from [Flatstep theme repository](https://gitlab.com/almoststatic-themes/flatstep)
+At the moment there are only a few themes, we are developing a "rolling theme"
+with some beautiful widgets ready to use.
+See [Flatstep theme](https://gitlab.com/almoststatic-themes/flatstep)
+and follow the tutorial.
 
 I'm not a designer so the result is of average quality. But I'm sure that good
 designers can write great themes.
 
 
 # Donate
```

### Comparing `almoststatic-1.0.1/setup.cfg` & `almoststatic-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = almoststatic
-version = 1.0.1
+version = 1.0.2
 author = Claudio driussi
 author_email = claudio.driussi@gmail.com
 description = Use Jinja2 template system to build static pages with Flask integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/claudio.driussi/almoststatic
 license = LGPL
```

