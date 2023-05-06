# Comparing `tmp/smartjs-0.0.3.tar.gz` & `tmp/smartjs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.3.tar", max compression
+gzip compressed data, was "smartjs-0.0.5.tar", max compression
```

## Comparing `smartjs-0.0.3.tar` & `smartjs-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      327 2023-05-05 03:50:25.692153 smartjs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      208 2023-05-05 01:28:03.905694 smartjs-0.0.3/smartjs/__init__.py
--rw-r--r--   0        0        0    13312 2023-05-05 03:48:44.377945 smartjs-0.0.3/smartjs/base.py
--rw-r--r--   0        0        0     2224 2023-05-05 03:50:25.688280 smartjs-0.0.3/smartjs/constants.py
--rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.3/smartjs/elements.py
--rw-r--r--   0        0        0     1094 2023-05-05 01:54:13.346118 smartjs-0.0.3/smartjs/env.py
--rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.3/smartjs/functions.py
--rw-r--r--   0        0        0    13893 2023-05-05 00:52:12.308743 smartjs-0.0.3/smartjs/javascript.py
--rw-r--r--   0        0        0      619 2023-05-05 02:05:47.881002 smartjs-0.0.3/smartjs/page.py
--rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.3/smartjs/style.py
--rw-r--r--   0        0        0      615 2023-05-05 03:50:31.019594 smartjs-0.0.3/setup.py
--rw-r--r--   0        0        0      379 2023-05-05 03:50:31.019816 smartjs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      302 2023-05-06 00:22:13.174930 smartjs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.5/smartjs/__init__.py
+-rw-r--r--   0        0        0    13325 2023-05-06 00:12:29.975202 smartjs-0.0.5/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.5/smartjs/constants.py
+-rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.5/smartjs/elements.py
+-rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.5/smartjs/functions.py
+-rw-r--r--   0        0        0    13961 2023-05-06 00:12:29.971024 smartjs-0.0.5/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.5/smartjs/page.py
+-rw-r--r--   0        0        0      807 2023-05-05 22:30:55.828371 smartjs-0.0.5/smartjs/path.py
+-rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.5/smartjs/style.py
+-rw-r--r--   0        0        0      584 2023-05-06 00:22:19.733975 smartjs-0.0.5/setup.py
+-rw-r--r--   0        0        0      333 2023-05-06 00:22:19.734213 smartjs-0.0.5/PKG-INFO
```

### Comparing `smartjs-0.0.3/smartjs/base.py` & `smartjs-0.0.5/smartjs/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,152 +92,153 @@
         return cap_words_case(name)
     
     @classmethod
     def camel_case(cls, name: str):
         return camel_case(name)
     
     @classmethod
-    def _get_computed_style(cls, element_name: str):
+    def get_computed_style(cls, element_name: str):
         return f'getComputedStyle({element_name})'
     
     @classmethod
-    def _remove(cls, element_name: str):
+    def remove(cls, element_name: str):
         return f'{element_name}.remove()'
     
     @classmethod
-    def _scroll(cls, element_name: str, x: int, y: int):
+    def scroll(cls, element_name: str, x: int, y: int):
         return f'{element_name}.scroll({x}, {y})'
     
     @classmethod
-    def _set_html(cls, element_name: str, html: str):
+    def set_html(cls, element_name: str, html: str):
         return f'{element_name}.setHTML({html})'
     
     @classmethod
-    def _scroll_to(cls, element_name: str, x: int, y: int):
+    def scroll_to(cls, element_name: str, x: int, y: int):
         return f'{element_name}.scrollTo({x}, {y})'
     
     @classmethod
-    def _scroll_by(cls, element_name: str, x: int, y: int):
+    def scroll_by(cls, element_name: str, x: int, y: int):
         return f'{element_name}.scrollBy({x}, {y})'
     
     @classmethod
-    def _replace_with(cls, element_out: str, element_in):
+    def replace_with(cls, element_out: str, element_in):
         return f'{element_out}.replaceWith({element_in})'
     
     @classmethod
-    def _remove_attribute(cls, element_name: str, attribute: str):
+    def remove_attribute(cls, element_name: str, attribute: str):
         return f'{element_name}.removeAttribute("{attribute}")'
     
     @classmethod
-    def _const_by_query_selector(cls, element_name: str, selector: str):
-        return cls._const(element_name, f'querySelector("{selector}")')
+    def const_by_query_selector(cls, element_name: str, selector: str):
+        return cls.const(element_name, f'querySelector("{selector}")')
     
     @classmethod
-    def _const_by_query_selector_all(cls, element_name: str, selector: str):
-        return cls._const(element_name, f'querySelectorAll("{selector}")')
+    def const_by_query_selector_all(cls, element_name: str, selector: str):
+        return cls.const(element_name, f'querySelectorAll("{selector}")')
     
     @classmethod
-    def _const_by_tag_name(cls, element_name, tag_name):
-        return cls._const(element_name, f'getElementsByTagName("{tag_name}")')
+    def const_by_tag_name(cls, element_name, tag_name):
+        return cls.const(element_name, f'getElementsByTagName("{tag_name}")')
     
     @classmethod
-    def _const_by_id(cls, element_id: str):
+    def const_by_id(cls, element_id: str):
         return f'const {cls.camel_case(element_id)} = document.getElementById("{element_id}")'
     
     @classmethod
-    def _const_get_attribute(cls, selection_name: str, element_name: str, attribute: str):
+    def const_get_attribute(cls, selection_name: str, element_name: str, attribute: str):
         return f'const {selection_name} = {element_name}.getAttribute("{attribute}")'
     
     @classmethod
-    def _set_interval(cls, function_name: str, interval: int = 1000):
+    def set_interval(cls, function_name: str, interval: int = 1000):
         return f'setInterval({function_name}, {interval})'
     
     @classmethod
-    def _for_loop(cls, item_name: str, array_name: str, statements: list[str]):
+    def for_loop(cls, item_name: str, array_name: str, statements: list[str]):
         return f'for (const {item_name} of {array_name}) {{{join(statements, "; ")}}}'
     
     @classmethod
-    def _set_timeout(cls, function_name: str, timeout: int = 1000):
+    def set_timeout(cls, function_name: str, timeout: int = 1000):
         return f'setTimeout({function_name}, {timeout})'
     
     @classmethod
-    def _function(cls, name: str, arguments: str = "", statements: list[str] = None):
+    def function(cls, name: str, arguments: str = "", statements: list[str] = None):
         return f'function {name} ({arguments}) {{{join(statements, "; " )}}}'
     
     @classmethod
-    def _anonymous(cls, arguments: str = "", statements: list[str] = None):
+    def anonymous(cls, arguments: str = "", statements: list[str] = None):
         return f'({arguments}) => {{{join(statements, "; " )}}}'
     
     @classmethod
-    def _if_statement(cls, condition: str, statements: list[str]):
+    def if_statement(cls, condition: str, statements: list[str]):
         return f'if({condition}){{{join(statements, "; ")}}}'
     
     @classmethod
-    def _else_if_statement(cls, condition: str, statements: list[str]):
+    def else_if_statement(cls, condition: str, statements: list[str]):
         return f'else if({condition}){{{join(statements, "; ")}}}'
     
     @classmethod
-    def _else_statement(cls, statements: list[str]):
+    def else_statement(cls, statements: list[str]):
         return f'else {{{join(statements, "; ")}}}'
     
     @classmethod
-    def _const_create_element(cls, name: str, tag: str):
+    def const_create_element(cls, name: str, tag: str):
         return f'const {name} = document.createElement("{tag}")'
     
     @classmethod
-    def _let(cls, element_name: str, statement: str):
+    def let(cls, element_name: str, statement: str):
         return f'let {element_name} = {statement}'
     
     @classmethod
-    def _const(cls, element_name: str, statement: str):
+    def const(cls, element_name: str, statement: str):
         return f'const {element_name} = {statement}'
     
     @classmethod
-    def _class_name(cls, element_name: str, class_name: str):
+    def set_class_name(cls, element_name: str, class_name: str):
         return f'{element_name}.className = "{class_name}"'
     
     @classmethod
-    def _set_attribute(cls, element_name: str, attribute_name: str, attribute_value: str):
+    def set_attribute(cls, element_name: str, attribute_name: str, attribute_value: str):
         return f'{element_name}.setAttribute("{underscore_to_hyphen(attribute_name)}", "{attribute_value}")'
     
     @classmethod
-    def _true(cls, element_name: str, argument: str):
+    def set_true(cls, element_name: str, argument: str):
         return f'{element_name}.{argument} = true'
     
     @classmethod
-    def _false(cls, element_name: str, argument: str):
+    def set_false(cls, element_name: str, argument: str):
         return f'{element_name}.{argument} = false'
     
     @classmethod
-    def _set_id(cls, element_name: str, element_id: str):
+    def set_id(cls, element_name: str, element_id: str):
         return f'{element_name}.id = "{element_id}"'
     
     @classmethod
-    def _inner_text(cls, element_name: str, value: str):
+    def set_inner_text(cls, element_name: str, value: str):
         return f'{element_name}.innerText = "{value}"'
     
     @classmethod
-    def _inner_html(cls, element_name: str, value: str):
+    def set_inner_html(cls, element_name: str, value: str):
         return f'{element_name}.innerHTML = "{value}"'
     
     @classmethod
-    def _append_to(cls, element_name: str, *args):
+    def set_append_to(cls, element_name: str, *args):
         return f'{element_name}.append({join(args, sep=", ")})'
     
     @classmethod
-    def _prepend_to(cls, element_name: str, *args):
+    def set_prepend_to(cls, element_name: str, *args):
         return f'{element_name}.prepend({join(args, sep=", ")})'
     
     @classmethod
-    def _style(cls, element_name: str, attribute: str, value: str):
+    def set_style(cls, element_name: str, attribute: str, value: str):
         return f'{element_name}.style.{attribute} = "{value}"'
     
     @classmethod
-    def _create_by_id(cls, element_id: str, tag: str):
-        return join([cls._const_create_element(cls.camel_case(element_id), tag), cls._set_id(cls.camel_case(element_id), element_id)], "; ")
+    def create_by_id(cls, element_id: str, tag: str):
+        return join([cls.const_create_element(cls.camel_case(element_id), tag),
+                     cls.set_id(cls.camel_case(element_id), element_id)], "; ")
 
 
 class BaseStyle(UserString):
     @classmethod
     def root_item(cls, name: str, value: str):
         return f'--{name}: {value}'
```

### Comparing `smartjs-0.0.3/smartjs/constants.py` & `smartjs-0.0.5/smartjs/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import re
 from typing import TypeVar
 from decimal import Decimal
 
 
 GenericType = TypeVar('GenericType')
-
 Number = TypeVar('Number', float, int, Decimal)
 
 
 EMPTY_TAGS: list[str] = ['input', 'img', 'meta', 'link', 'br', 'hr']
 STRUCTURE: list[str] = ['html', 'head', 'body', 'title']
 SEMANTIC: list[str] = ['header', 'footer', 'main', 'aside', 'nav']
 FORM_FIELDS: list[str] = ['input', 'select', 'textarea']
```

### Comparing `smartjs-0.0.3/smartjs/elements.py` & `smartjs-0.0.5/smartjs/elements.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.3/smartjs/functions.py` & `smartjs-0.0.5/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.3/smartjs/javascript.py` & `smartjs-0.0.5/smartjs/javascript.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,55 +9,55 @@
 from smartjs.functions import *
 from smartjs.base import *
 
 
 class ScriptStatement(BaseScript):
     def __init__(self, statement: str):
         self.statement = statement
-        super().__init__(self.statement)
+        super().__init__(str(self.statement))
 
 
 class ScriptJoin(BaseScript):
     def __init__(self, *args):
         self.args = args
         super().__init__(join(SmartList(*self.args), '; '))
 
 
 class ScriptConstant(BaseScript):
     def __init__(self, name: str, statement: Union[str, ScriptStatement]):
         self.name = name
         self.statement = statement
-        super().__init__(f'const {self.name} = {str(self.statement)}')
+        super().__init__(self.const(self.name, str(self.statement)))
 
 
 class ScriptVariable(BaseScript):
     def __init__(self, name: str, statement: Union[str, ScriptStatement]):
         self.name = name
         self.statement = statement
-        super().__init__(f'let {name} = {str(statement)}')
+        super().__init__(self.let(self.name, str(self.statement)))
 
 
 class ScriptIf(BaseScript):
     def __init__(self, condition: str, statements: list[str]):
         self.condition = condition
         self.statements = statements
-        super().__init__(self._if_statement(self.condition, self.statements))
+        super().__init__(self.if_statement(self.condition, self.statements))
         
         
 class ScriptElseIf(BaseScript):
     def __init__(self, condition: str, statements: list[str]):
         self.condition = condition
         self.statements = statements
-        super().__init__(self._else_if_statement(self.condition, self.statements))
+        super().__init__(self.else_if_statement(self.condition, self.statements))
         
         
 class ScriptElse(BaseScript):
     def __init__(self, statements: list[str]):
         self.statements = statements
-        super().__init__(self._else_statement(self.statements))
+        super().__init__(self.else_statement(self.statements))
         
         
 class ScriptCondition(BaseScript):
     def __init__(self, *args):
         self.if_clause = list_of_type(args, ScriptIf)
         self.else_if_clauses = list_of_type(args, ScriptElseIf)
         self.else_clause = list_of_type(args, ScriptElse)
@@ -65,22 +65,22 @@
         
 
 class ScriptFunction(BaseScript):
     def __init__(self, name: str, arguments: str = '', statements: list[Union[str, ScriptStatement]] = None):
         self.name = name
         self.arguments = arguments
         self.statements = statements
-        super().__init__(self._function(self.name, self.arguments, self.statements))
+        super().__init__(self.function(self.name, self.arguments, self.statements))
 
 
 class ScriptAnonymous(BaseScript):
     def __init__(self, arguments: str = '', statements: list[Union[str, ScriptStatement]] = None):
         self.arguments = arguments
         self.statements = statements
-        super().__init__(self._anonymous(self.arguments, self.statements))
+        super().__init__(self.anonymous(self.arguments, self.statements))
 
 
 class ScriptListLoop(BaseScript):
     def __init__(self, list_name: str, statements: list[Union[str, ScriptStatement]]):
         self.list_name = list_name
         self.statements = statements
         super().__init__(f'for (let i = 0; i < {self.list_name}.length; i++) {{{ScriptJoin(self.statements)}}}')
@@ -141,38 +141,38 @@
                 self.append_to_container
         )
     
     @property
     def element_label(self):
         if not self.is_hidden:
             return ScriptJoin(
-                    self._const_create_element(self.label_name, 'label'),
-                    self._class_name(self.label_name, self.label_class),
-                    self._set_attribute(self.label_name, 'for', self.name),
-                    self._set_id(self.label_name, self.field_id),
-                    self._inner_text(self.label_name, self.label_text)
+                    self.const_create_element(self.label_name, 'label'),
+                    self.class_name(self.label_name, self.label_class),
+                    self.set_attribute(self.label_name, 'for', self.name),
+                    self.set_id(self.label_name, self.field_id),
+                    self.set_inner_text(self.label_name, self.label_text)
             )
         return ''
     
     @property
     def element_field(self):
         return ScriptJoin(
-                self._const_create_element(self.field_name, self.field_tag),
-                self._class_name(self.field_name, self.field_class),
-                *[self._set_attribute(self.field_name, k, v) for k, v in self.kwargs.items()],
-                *[self._true(self.field_name, item) for item in self.args],
-                self._set_id(self.field_name, self.name)
+                self.const_create_element(self.field_name, self.field_tag),
+                self.class_name(self.field_name, self.field_class),
+                *[self.set_attribute(self.field_name, k, v) for k, v in self.kwargs.items()],
+                *[self.set_true(self.field_name, item) for item in self.args],
+                self.set_id(self.field_name, self.name)
         )
     
     @property
     def element_container(self):
         return ScriptJoin(
-                self._const_create_element(self.container_name, 'div'),
-                self._class_name(self.container_name, self.container_class),
-                self._set_id(self.container_name, self.container_id)
+                self.const_create_element(self.container_name, 'div'),
+                self.class_name(self.container_name, self.container_class),
+                self.set_id(self.container_name, self.container_id)
         )
     
     @property
     def append_to_container(self):
         if self.is_checkbox:
             return ScriptStatement(f'{self.container_name}.append({self.label_name}, {self.field_name})')
         elif self.is_hidden:
@@ -192,27 +192,28 @@
         self.kwargs = dict_filtered(kwargs)
         self.button_id = f'{self.id}__button'
         self.button_name = self.camel_case(self.button_id)
         super().__init__(self.render())
         
     def render(self):
         return ScriptJoin(
-                self._const_create_element(self.form_name, 'form'),
-                self._set_attribute(self.form_name, 'action', self.action),
-                self._set_attribute(self.form_name, 'method', self.method),
-                self._class_name(self.form_name, self.form_class),
-                *[self._set_attribute(self.form_name, k, v) for k, v in self.kwargs.items()],
-                self._set_id(self.form_name, self.id),
+                self.const_create_element(self.form_name, 'form'),
+                self.set_attribute(self.form_name, 'action', self.action),
+                self.set_attribute(self.form_name, 'method', self.method),
+                self.class_name(self.form_name, self.form_class),
+                *[self.set_attribute(self.form_name, k, v) for k, v in self.kwargs.items()],
+                self.set_id(self.form_name, self.id),
                 ScriptJoin(*self.form_fields),
-                *[self._append_to(self.form_name, *[item.container_name for item in self.form_fields])],
-                self._const_create_element(self.button_name, 'button'),
-                self._set_id(self.button_name, self.button_id),
-                self._append_to(self.form_name, self.button_name)
+                *[self.set_append_to(self.form_name, *[item.container_name for item in self.form_fields])],
+                self.const_create_element(self.button_name, 'button'),
+                self.set_id(self.button_name, self.button_id),
+                self.set_append_to(self.form_name, self.button_name)
         )
     
+    
 class ScriptById(BaseScript):
     def __init__(self, element_id: str):
         self.id = element_id
         self.name = self.camel_case(element_id)
         self.args = []
         self.instances = []
         self.data = repr(self)
@@ -234,76 +235,76 @@
     def append_instance(self, instance: 'ScriptById'):
         self.instances.append(instance)
         self.args = [*self.args, *instance.args]
         self.append(instance.name)
         return self
         
     def tag(self, tag: str):
-        self.args.append(self._create_by_id(self.id, tag))
+        self.args.append(self.create_by_id(self.id, tag))
         return self
     
     def id_as_name(self):
-        self.args.append(self._set_attribute(self.name, 'name', self.id))
+        self.args.append(self.set_attribute(self.name, 'name', self.id))
         return self
     
     def change_name(self, name: str):
-        self.args.append(self._set_attribute(self.name, 'name', name))
+        self.args.append(self.set_attribute(self.name, 'name', name))
         self.name = name
         return self
     
     def get_style(self, attribute: str):
-        return f'{self._get_computed_style(self.name)}["{attribute}"]'
+        return f'{self.get_computed_style(self.name)}["{attribute}"]'
         
-    def change_id(self, id: str):
-        self.args.append(self._set_id(self.name, id))
-        self.id = id
+    def change_id(self, element_id: str):
+        self.args.append(self.set_id(self.name, element_id))
+        self.id = element_id
         return self
     
     def append(self, *args):
-        self.args.append(self._append_to(self.name, *args))
+        self.args.append(self.set_append_to(self.name, *args))
         return self
     
     def append_to(self, element_name: str):
-        self.args.append(self._append_to(element_name, self.name))
+        self.args.append(self.set_append_to(element_name, self.name))
         return self
     
     def prepend_to(self, element_name: str):
-        self.args.append(self._prepend_to(element_name, self.name))
+        self.args.append(self.set_prepend_to(element_name, self.name))
         return self
     
     def prepend(self, *args):
-        self.args.append(self._prepend_to(self.name, *args))
+        self.args.append(self.set_prepend_to(self.name, *args))
         return self
         
     def style(self, name: str, value: str):
-        self.args.append(self._style(self.name, name, value))
+        self.args.append(self.set_style(self.name, name, value))
         return self
     
     def inner_text(self, text: str):
-        self.args.append(self._inner_text(self.name, text))
+        self.args.append(self.set_inner_text(self.name, text))
         return self
     
     def inner_html(self, html: str):
-        self.args.append(self._inner_html(self.name, html))
+        self.args.append(self.set_inner_html(self.name, html))
         return self
         
     def class_name(self, class_name: str):
-        self.args.append(self._class_name(self.name, class_name))
+        self.args.append(self.set_class_name(self.name, class_name))
         return self
     
     def attribute(self, name: str, value: str):
-        self.args.append(self._set_attribute(self.name, name, value))
+        self.args.append(self.set_attribute(self.name, name, value))
         return self
     
     def true(self, argument: str):
-        self.args.append(self._true(self.name, argument))
+        self.args.append(self.set_true(self.name, argument))
         return self
     
     def false(self, argument: str):
-        self.args.append(self._false(self.name, argument))
+        self.args.append(self.set_false(self.name, argument))
         return self
     
 
 class Script(BaseScript):
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
@@ -332,13 +333,15 @@
     n = ScriptById('my_name2').tag('input').class_name('form-control').true('required').attribute('placeholder', 'my_name').style('backgroundColor', 'green').id_as_name()
     nl = ScriptById('my_name2__label').tag('label').class_name('form-label').attribute('for', n.name).inner_html('meu nome')
     nc = ScriptById('my_name2__container').tag('div').class_name('form-floating').append_instance(n).append_instance(nl)
     i3 = ScriptById('check').tag('input').attribute('type', 'checkbox').id_as_name().class_name('form-check-input')
     l3 = ScriptById('check__label').tag('label').attribute('for', i3.id).class_name('form-check-label').inner_html('ativo?')
     c3 = ScriptById('check__container').tag('div').class_name('form-check').append_instance(i3).append_instance(l3)
     f = ScriptById('form').tag('form').class_name('form-control').style('marginTop', '200px').append_instance(t).append_instance(c).append_instance(nc).append_instance(c3).append_to('main')
-    d = Script._for_loop('formField', 'form.elements', ['console.log(formField)'])
+    d = Script.for_loop('formField', 'form.elements', ['console.log(formField)'])
 
     print(ScriptJoin(*f.args, str(d)))
+    
+    print()
```

### Comparing `smartjs-0.0.3/smartjs/style.py` & `smartjs-0.0.5/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.3/setup.py` & `smartjs-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['smartjs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Unidecode>=1.3.6,<2.0.0', 'python-dotenv>=1.0.0,<2.0.0']
+['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.3',
+    'version': '0.0.5',
     'description': '',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

