# Comparing `tmp/fastapi_amis_admin-0.5.6a1.tar.gz` & `tmp/fastapi_amis_admin-0.5.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.5.6a1.tar", last modified: Thu Apr 27 13:01:21 2023, max compression
+gzip compressed data, was "fastapi_amis_admin-0.5.7a1.tar", last modified: Sat May  6 15:14:44 2023, max compression
```

## Comparing `fastapi_amis_admin-0.5.6a1.tar` & `fastapi_amis_admin-0.5.7a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     8952 2022-10-24 02:06:23.761811 fastapi_amis_admin-0.5.6a1/README.md
--rw-r--r--   0        0        0      603 2023-04-27 13:00:39.542409 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    58994 2023-04-27 12:59:14.169742 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3822 2023-04-15 02:00:42.051799 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    13527 2023-04-10 02:48:15.553268 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     1765 2023-04-03 15:08:16.449121 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   148056 2023-04-18 02:57:48.156531 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     5096 2023-04-10 02:48:14.390933 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      205 2023-02-15 09:21:27.181461 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    23195 2023-04-25 12:57:47.625491 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     8069 2023-04-10 02:55:03.995604 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0     8763 2023-04-10 02:48:15.229453 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1950 2023-04-06 13:53:04.589440 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     3449 2023-04-10 02:48:14.872657 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/base.pot
--rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       75 2022-09-22 08:34:57.595807 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2975 2023-04-10 02:48:15.151497 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     1899 2023-04-10 02:48:15.171486 fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0     2765 2023-04-10 02:53:34.454713 fastapi_amis_admin-0.5.6a1/pyproject.toml
--rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.5.6a1/PKG-INFO
+-rw-r--r--   0        0        0     8952 2022-10-24 02:06:23.761811 fastapi_amis_admin-0.5.7a1/README.md
+-rw-r--r--   0        0        0      603 2023-05-06 15:14:25.657171 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    58785 2023-05-06 15:05:25.998150 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3822 2023-04-15 02:00:42.051799 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    13527 2023-04-10 02:48:15.553268 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     1765 2023-05-06 13:59:35.102228 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   148784 2023-04-28 13:40:19.195342 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     5096 2023-04-10 02:48:14.390933 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      205 2023-02-15 09:21:27.181461 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    23195 2023-05-05 13:47:21.715192 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     8069 2023-04-10 02:55:03.995604 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0     8763 2023-04-10 02:48:15.229453 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1950 2023-04-06 13:53:04.589440 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     3449 2023-04-10 02:48:14.872657 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/base.pot
+-rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       75 2022-09-22 08:34:57.595807 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2975 2023-04-10 02:48:15.151497 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     1899 2023-04-10 02:48:15.171486 fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0     2765 2023-04-10 02:53:34.454713 fastapi_amis_admin-0.5.7a1/pyproject.toml
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.5.7a1/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.5.6a1/README.md` & `fastapi_amis_admin-0.5.7a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/__init__.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.6a1"
+__version__ = "0.5.7a1"
 __url__ = "https://github.com/amisadmin/fastapi_amis_admin"
 
 import gettext
 import os
 
 from .utils.translation import i18n
```

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -698,14 +698,15 @@
                 if modelfield:
                     columns.append(await self.get_list_column(request, modelfield))
         # Append operation column
         actions = await self.get_actions(request, flag="column") or []
         for action in actions:
             columns.append(
                 ColumnOperation(
+                    fixed="right",
                     label=getattr(action, "label", _("Operation")),
                     breakpoint="*",
                     buttons=[action],
                 )
             )
         # Append inline link model column
         for link_form in self.link_model_forms:
@@ -856,39 +857,35 @@
                 Action(actionType="submit", label=_("Search"), level=LevelEnum.primary),
             ],
             trimValues=True,
         )
 
     async def get_create_form(self, request: Request, bulk: bool = False) -> Form:
         fields = [field for field in self.schema_create.__fields__.values() if field.name != self.pk_name]
+        body = await self._conv_modelfields_to_formitems(request, fields, CrudEnum.create)
         if not bulk:
             return Form(
                 api=f"post:{self.router_path}/item",
                 name=CrudEnum.create,
-                body=await self._conv_modelfields_to_formitems(request, fields, CrudEnum.create),
+                body=body,
             )
-        columns, keys = [], {}
-        for field in fields:
-            column = await self.get_list_column(request, self.parser.get_modelfield(field))
-            keys[column.name] = "${" + column.label + "}"
-            column.name = column.label
-            columns.append(column)
         return Form(
             api=AmisAPI(
                 method="post",
                 url=f"{self.router_path}/item",
-                data={"&": {"$excel": keys}},
+                data={"&": "$excel"},
             ),
+            name=CrudEnum.create,
             mode=DisplayModeEnum.normal,
             body=[
                 InputExcel(name="excel"),
                 InputTable(
                     name="excel",
                     showIndex=True,
-                    columns=columns,
+                    columns=body,
                     addable=True,
                     copyable=True,
                     editable=True,
                     removable=True,
                 ),
             ],
         )
```

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/parser.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/settings.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     site_icon: str = "https://baidu.gitee.io/amis/static/favicon_b3b0647.png"
     site_url: str = ""
     site_path: str = "/admin"
     database_url_async: str = Field("", env="DATABASE_URL_ASYNC")
     database_url: str = Field("", env="DATABASE_URL")
     language: Union[Literal["zh_CN", "en_US", "de_DE"], str] = ""
     amis_cdn: str = "https://unpkg.com"
-    amis_pkg: str = "amis@2.9.0"
+    amis_pkg: str = "amis@3.0.0"
     amis_theme: Literal["cxd", "antd", "dark", "ang"] = "cxd"
     amis_image_receiver: API = None  # Image upload interface
     amis_file_receiver: API = None  # File upload interface
     logger: Union[logging.Logger, Any] = logging.getLogger("fastapi_amis_admin")
 
     @validator("amis_cdn", "site_path", "site_url", pre=True)
     def valid_url(cls, url: str):
```

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,43 +392,54 @@
     children: List["PageSchema"] = None  # Submenu
     sort: int = None  # Unofficial attribute. sort
     tabsMode: TabsModeEnum = None  # Unofficial attribute. Display mode, the value can be line, card, radio, vertical,
     # chrome, simple, strong, tiled, sidebar, collapse
 
     def as_page_body(self, group_extra: Dict[str, Any] = None, item_extra: Dict[str, Any] = None):
         if self.children:
+            exclude = {"type", "url", "schema_", "schemaApi", "link", "redirect", "rewrite", "isDefaultPage", "children"}
             if self.tabsMode is None:
                 body = App(pages=[PageSchema(children=self.children)])
             elif self.tabsMode == TabsModeEnum.collapse:
-                body = CollapseGroup(
-                    body=[
-                        CollapseGroup.CollapseItem(
-                            header=item.label,
-                            body=item.as_page_body(group_extra, item_extra),
-                        ).update_from_dict(item_extra or {})
-                        for item in self.children
-                    ],
-                ).update_from_dict(group_extra or {})
+                body = (
+                    CollapseGroup.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
+                    .update_from_kwargs(
+                        body=[
+                            CollapseGroup.CollapseItem.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
+                            .update_from_kwargs(
+                                header=item.label,
+                                body=item.as_page_body(group_extra, item_extra),
+                            )
+                            .update_from_dict(item_extra or {})
+                            for item in self.children
+                        ],
+                    )
+                    .update_from_dict(group_extra or {})
+                )
             else:
-                body = Tabs(
-                    tabsMode=self.tabsMode,
-                    mountOnEnter=True,
-                    tabs=[
-                        Tabs.Item(
-                            title=item.label,
-                            icon=item.icon,
-                            tab=item.as_page_body(group_extra, item_extra),
-                        ).update_from_dict(item_extra or {})
-                        for item in self.children
-                    ],
-                ).update_from_dict(group_extra or {})
+                body = (
+                    Tabs.parse_obj(self.dict(exclude=exclude, exclude_defaults=True))
+                    .update_from_kwargs(
+                        mountOnEnter=True,
+                        tabs=[
+                            Tabs.Item.parse_obj(item.dict(exclude=exclude, exclude_defaults=True))
+                            .update_from_kwargs(
+                                title=item.label,
+                                tab=item.as_page_body(group_extra, item_extra),
+                            )
+                            .update_from_dict(item_extra or {})
+                            for item in self.children
+                        ],
+                    )
+                    .update_from_dict(group_extra or {})
+                )
         elif self.schema_:
             body = self.schema_
             if isinstance(body, Iframe):
-                body.height = 1080
+                body.height = body.height or 1080
         elif self.schemaApi:
             body = Service(schemaApi=self.schemaApi)
         elif self.link:
             body = Page(body=Link(href=self.link, body=self.label, blank=True))
         else:
             body = None
         return body
```

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/constants.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/templates/app.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/templates/page.html` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/templates/page.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/amis/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/README.md` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/_sqlmodel.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/_sqlmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,15 @@
 
         return route
 
     @property
     def route_create(self) -> Callable:
         async def route(
             request: Request,
-            data: Union[self.schema_create, List[self.schema_create]] = Body(...),  # type: ignore
+            data: Union[List[self.schema_create], self.schema_create] = Body(...),  # type: ignore
         ) -> BaseApiOut[Union[int, self.schema_model]]:  # type: ignore
             if not await self.has_create_permission(request, data):
                 return self.error_no_router_permission(request)
             if not isinstance(data, list):
                 data = [data]
             items = [await self.on_create_pre(request, obj) for obj in data]
             if not items:
```

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/parser.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/parser.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/crud/utils.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/crud/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/base.pot` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/base.pot`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/models/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/models/fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/utils/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.5.7a1/fastapi_amis_admin/utils/translation.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/pyproject.toml` & `fastapi_amis_admin-0.5.7a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.5.6a1/PKG-INFO` & `fastapi_amis_admin-0.5.7a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin
-Version: 0.5.6a1
+Version: 0.5.7a1
 Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
 Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

