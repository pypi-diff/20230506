# Comparing `tmp/los_docusign-0.6.5.tar.gz` & `tmp/los_docusign-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "los_docusign-0.6.5.tar", max compression
+gzip compressed data, was "los_docusign-0.6.6.tar", max compression
```

## Comparing `los_docusign-0.6.5.tar` & `los_docusign-0.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1571 2022-02-09 21:29:17.720800 los_docusign-0.6.5/LICENSE
--rw-r--r--   0        0        0     3650 2022-03-21 11:49:57.380120 los_docusign-0.6.5/README.md
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.720971 los_docusign-0.6.5/los_docusign/__init__.py
--rw-r--r--   0        0        0     5716 2023-03-07 22:21:14.008395 los_docusign-0.6.5/los_docusign/admin.py
--rw-r--r--   0        0        0      219 2022-02-09 21:29:17.721103 los_docusign-0.6.5/los_docusign/apps.py
--rw-r--r--   0        0        0      401 2022-02-09 21:29:17.721157 los_docusign-0.6.5/los_docusign/asgi.py
--rw-r--r--   0        0        0    17806 2022-02-09 21:29:17.721263 los_docusign-0.6.5/los_docusign/migrations/0001_initial.py
--rw-r--r--   0        0        0     6960 2022-02-09 21:29:17.721334 los_docusign-0.6.5/los_docusign/migrations/0002_auto_20211125_0208.py
--rw-r--r--   0        0        0     2174 2022-02-09 21:29:17.721402 los_docusign-0.6.5/los_docusign/migrations/0003_auto_20211227_1445.py
--rw-r--r--   0        0        0      716 2022-02-09 21:29:17.721456 los_docusign-0.6.5/los_docusign/migrations/0004_auto_20220119_1610.py
--rw-r--r--   0        0        0      582 2022-02-09 21:29:17.721507 los_docusign-0.6.5/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py
--rw-r--r--   0        0        0      385 2022-03-21 10:17:43.895436 los_docusign-0.6.5/los_docusign/migrations/0006_remove_docusignuserauth_two_factor_enabled_flag.py
--rw-r--r--   0        0        0      485 2023-02-10 16:58:05.166483 los_docusign-0.6.5/los_docusign/migrations/0007_alter_docusignenvelopestagedata_error_message.py
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721530 los_docusign-0.6.5/los_docusign/migrations/__init__.py
--rw-r--r--   0        0        0    11978 2023-02-10 16:58:05.167989 los_docusign-0.6.5/los_docusign/models.py
--rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721654 los_docusign-0.6.5/los_docusign/tests.py
--rw-r--r--   0        0        0      754 2022-02-09 21:29:17.721713 los_docusign-0.6.5/los_docusign/urls.py
--rw-r--r--   0        0        0     2690 2022-02-09 21:29:17.721801 los_docusign-0.6.5/los_docusign/utils/XmlParser.py
--rw-r--r--   0        0        0      233 2022-02-09 21:29:17.721848 los_docusign-0.6.5/los_docusign/utils/__init__.py
--rw-r--r--   0        0        0     7750 2022-12-06 19:12:40.613469 los_docusign-0.6.5/los_docusign/utils/api_handler.py
--rw-r--r--   0        0        0     9372 2022-12-06 19:12:40.613994 los_docusign-0.6.5/los_docusign/utils/client.py
--rw-r--r--   0        0        0    17546 2023-02-10 16:58:05.168493 los_docusign-0.6.5/los_docusign/utils/docusign_adapter.py
--rw-r--r--   0        0        0    20730 2022-12-06 19:12:40.614585 los_docusign-0.6.5/los_docusign/utils/docusign_helper.py
--rw-r--r--   0        0        0     4652 2022-02-25 19:02:11.957541 los_docusign-0.6.5/los_docusign/utils/validators.py
--rw-r--r--   0        0        0       26 2022-02-09 21:29:17.722208 los_docusign-0.6.5/los_docusign/views.py
--rw-r--r--   0        0        0      401 2022-02-09 21:29:17.722254 los_docusign-0.6.5/los_docusign/wsgi.py
--rw-r--r--   0        0        0     1012 2023-03-07 22:21:14.009091 los_docusign-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4771 2023-03-07 22:22:02.574669 los_docusign-0.6.5/setup.py
--rw-r--r--   0        0        0     4691 2023-03-07 22:22:02.575163 los_docusign-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1571 2022-02-09 21:29:17.720800 los_docusign-0.6.6/LICENSE
+-rw-r--r--   0        0        0     3650 2022-03-21 11:49:57.380120 los_docusign-0.6.6/README.md
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.720971 los_docusign-0.6.6/los_docusign/__init__.py
+-rw-r--r--   0        0        0     5794 2023-04-03 18:34:44.502327 los_docusign-0.6.6/los_docusign/admin.py
+-rw-r--r--   0        0        0      219 2022-02-09 21:29:17.721103 los_docusign-0.6.6/los_docusign/apps.py
+-rw-r--r--   0        0        0      401 2022-02-09 21:29:17.721157 los_docusign-0.6.6/los_docusign/asgi.py
+-rw-r--r--   0        0        0    17806 2022-02-09 21:29:17.721263 los_docusign-0.6.6/los_docusign/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6960 2022-02-09 21:29:17.721334 los_docusign-0.6.6/los_docusign/migrations/0002_auto_20211125_0208.py
+-rw-r--r--   0        0        0     2174 2022-02-09 21:29:17.721402 los_docusign-0.6.6/los_docusign/migrations/0003_auto_20211227_1445.py
+-rw-r--r--   0        0        0      716 2022-02-09 21:29:17.721456 los_docusign-0.6.6/los_docusign/migrations/0004_auto_20220119_1610.py
+-rw-r--r--   0        0        0      582 2022-02-09 21:29:17.721507 los_docusign-0.6.6/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py
+-rw-r--r--   0        0        0      385 2022-03-21 10:17:43.895436 los_docusign-0.6.6/los_docusign/migrations/0006_remove_docusignuserauth_two_factor_enabled_flag.py
+-rw-r--r--   0        0        0      485 2023-02-10 16:58:05.166483 los_docusign-0.6.6/los_docusign/migrations/0007_alter_docusignenvelopestagedata_error_message.py
+-rw-r--r--   0        0        0     3368 2023-05-05 20:44:43.455719 los_docusign-0.6.6/los_docusign/migrations/0008_auto_20230412_2119.py
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721530 los_docusign-0.6.6/los_docusign/migrations/__init__.py
+-rw-r--r--   0        0        0    12038 2023-05-05 20:44:43.457031 los_docusign-0.6.6/los_docusign/models.py
+-rw-r--r--   0        0        0        0 2022-02-09 21:29:17.721654 los_docusign-0.6.6/los_docusign/tests.py
+-rw-r--r--   0        0        0      754 2022-02-09 21:29:17.721713 los_docusign-0.6.6/los_docusign/urls.py
+-rw-r--r--   0        0        0     2690 2022-02-09 21:29:17.721801 los_docusign-0.6.6/los_docusign/utils/XmlParser.py
+-rw-r--r--   0        0        0      233 2022-02-09 21:29:17.721848 los_docusign-0.6.6/los_docusign/utils/__init__.py
+-rw-r--r--   0        0        0     7771 2023-04-12 09:35:46.064826 los_docusign-0.6.6/los_docusign/utils/api_handler.py
+-rw-r--r--   0        0        0     9718 2023-04-12 09:35:46.065116 los_docusign-0.6.6/los_docusign/utils/client.py
+-rw-r--r--   0        0        0    16929 2023-04-12 09:35:46.065491 los_docusign-0.6.6/los_docusign/utils/docusign_adapter.py
+-rw-r--r--   0        0        0    23671 2023-04-12 09:35:46.066247 los_docusign-0.6.6/los_docusign/utils/docusign_helper.py
+-rw-r--r--   0        0        0     4652 2022-02-25 19:02:11.957541 los_docusign-0.6.6/los_docusign/utils/validators.py
+-rw-r--r--   0        0        0       26 2022-02-09 21:29:17.722208 los_docusign-0.6.6/los_docusign/views.py
+-rw-r--r--   0        0        0      401 2022-02-09 21:29:17.722254 los_docusign-0.6.6/los_docusign/wsgi.py
+-rw-r--r--   0        0        0     1012 2023-05-05 20:44:43.458238 los_docusign-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 los_docusign-0.6.6/PKG-INFO
```

### Comparing `los_docusign-0.6.5/LICENSE` & `los_docusign-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/README.md` & `los_docusign-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/admin.py` & `los_docusign-0.6.6/los_docusign/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 
     def has_add_permission(self, request):
         return False
 
     def has_delete_permission(self, request, obj=None):
         return False
 
+    def has_change_permission(self, request, obj=None):
+        return False
+
 
 @admin.register(DocusignOrgTemplate)
 class DocusignOrgTemplateAdmin(admin.ModelAdmin):
     model = DocusignOrgTemplate
     list_display = ("organization_model", "docusign_template", "created", "modified")
     readonly_fields = ["organization_model", "docusign_template"]
     list_filter = (
```

### Comparing `los_docusign-0.6.5/los_docusign/migrations/0001_initial.py` & `los_docusign-0.6.6/los_docusign/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/migrations/0002_auto_20211125_0208.py` & `los_docusign-0.6.6/los_docusign/migrations/0002_auto_20211125_0208.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/migrations/0003_auto_20211227_1445.py` & `los_docusign-0.6.6/los_docusign/migrations/0003_auto_20211227_1445.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/migrations/0004_auto_20220119_1610.py` & `los_docusign-0.6.6/los_docusign/migrations/0004_auto_20220119_1610.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py` & `los_docusign-0.6.6/los_docusign/migrations/0005_docusignenvelopeauditlog_recipient_details.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/models.py` & `los_docusign-0.6.6/los_docusign/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     class Meta:
         db_table = "docusign_client_auths"
         verbose_name = "Docusign user authentication"
         verbose_name_plural = "Docusign user authentications"
 
     access_token = models.TextField("Access Token")
     expires_at = models.DateTimeField("Token Expires At")
-    # organization = models.ForeignKey("organizations.Organization", on_delete=models.CASCADE,unique=True)
+    # organization = models.ForeignKey("organizations.Organization", on_delete=models.PROTECT,unique=True)
     organization_model = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.SET_NULL,
+        null=True,
         related_name="+",
         verbose_name=_("Organization Model"),
     )
     organization_pk = models.CharField(
         max_length=255, verbose_name=_("organization pk")
     )
     docusign_api_username = models.CharField("Docusign API Username", max_length=255)
@@ -92,24 +93,25 @@
     envelope_response = models.CharField("Envelope Response", max_length=255)
     error_message = models.TextField(
         "Error Message", blank=True, null=True
     )
     docusign_user = models.ForeignKey(
         "los_docusign.DocuSignUserAuth", on_delete=models.PROTECT
     )
-    # etran_loan = models.ForeignKey("loans.EtranLoan",on_delete=models.CASCADE, blank=True, null=True, related_name='envelopes')
+    # etran_loan = models.ForeignKey("loans.EtranLoan",on_delete=models.PROTECT, blank=True, null=True, related_name='envelopes')
     client_user_id = models.CharField(
         "Client User Id", max_length=255, null=True, blank=True
     )
     recipient_auth_info = JSONField(
         "Recipient Authentication Info", null=True, blank=True
     )
     content_type = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.SET_NULL,
+        null=True,
         related_name="+",
         verbose_name=_("content type"),
     )
     object_pk = models.CharField(max_length=255, verbose_name=_("object pk"))
     phase = models.CharField(
         max_length=255, blank=True, null=True, verbose_name=_("Application Phase")
     )
@@ -138,23 +140,23 @@
     class Meta:
         db_table = "docusign_org_templates"
         verbose_name = "Docusign Organization Template"
         verbose_name_plural = "Docusign Organization Templates"
 
     organization_model = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.PROTECT,
         related_name="+",
         verbose_name=_("Organization Model"),
     )
     organization_pk = models.CharField(
         max_length=255, verbose_name=_("organization pk")
     )
     docusign_template = models.ForeignKey(
-        "los_docusign.DocusignTemplate", on_delete=models.CASCADE
+        "los_docusign.DocusignTemplate", on_delete=models.PROTECT
     )
 
     def __str__(self):
         return f"{self.organization_pk}-{self.docusign_template.template_type}"
 
 
 class DocusignTemplateOrgExclusion(TimeStampedModel, SoftDeleteMixin):
@@ -162,26 +164,26 @@
         db_table = "docusign_template_org_exclusions"
         verbose_name = "Docusign Organization Template Exclusion"
         verbose_name_plural = "Docusign Organization Template Exclusions"
         unique_together = ["organization_pk", "document_name", "template"]
 
     organization_model = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.PROTECT,
         related_name="+",
         verbose_name=_("Organization Model"),
     )
     organization_pk = models.CharField(
         max_length=255, verbose_name=_("organization pk")
     )
     document_name = models.ForeignKey(
-        "los_docusign.DocusignChoiceConfig", on_delete=models.CASCADE
+        "los_docusign.DocusignChoiceConfig", on_delete=models.PROTECT
     )
     template = models.ForeignKey(
-        "los_docusign.DocusignTemplate", on_delete=models.CASCADE
+        "los_docusign.DocusignTemplate", on_delete=models.PROTECT
     )
 
 
 class DocusignChoiceConfig(TimeStampedModel, SoftDeleteMixin):
     class Meta:
         db_table = "docusign_choice_configs"
         verbose_name = "Docusign Choice Config"
@@ -207,15 +209,15 @@
         db_table = "docusign_templates"
         verbose_name = "Docusign Template"
         verbose_name_plural = "Docusign Templates"
 
     docusign_payload = models.TextField("Docusign Payload")
     # template_type = models.CharField("Template Type",max_length=32,choices=TEMPLATE_TYPE_CHOICES)
     template_type = models.ForeignKey(
-        "los_docusign.DocusignChoiceConfig", on_delete=models.CASCADE
+        "los_docusign.DocusignChoiceConfig", on_delete=models.PROTECT
     )
     is_active = models.BooleanField("Is Active", default=True)
     is_default = models.BooleanField("Default Template", default=False)
 
     def save(self, *args, **kwargs):
         # Do not allow more than 1 default
         ds = DocusignTemplate.objects.filter(
@@ -232,27 +234,27 @@
 class DocusignOrgTemplateConfig(TimeStampedModel, SoftDeleteMixin):
     class Meta:
         db_table = "docusign_org_template_configs"
         verbose_name = "Docusign Organization Template Config"
         verbose_name_plural = "Docusign Organizations Templates Configs"
         unique_together = ["organization_pk", "template"]
 
-    # organization = models.ForeignKey("organizations.Organization", on_delete=models.CASCADE)
+    # organization = models.ForeignKey("organizations.Organization", on_delete=models.PROTECT)
     organization_model = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.PROTECT,
         related_name="+",
         verbose_name=_("content type"),
     )
     organization_pk = models.CharField(
         db_index=True, max_length=255, verbose_name=_("object pk")
     )
     template_config = JSONField("Template Configuration")
     template = models.ForeignKey(
-        "los_docusign.DocusignTemplate", on_delete=models.CASCADE
+        "los_docusign.DocusignTemplate", on_delete=models.PROTECT
     )
     is_active = models.BooleanField("Is Active", default=True)
     is_default = models.BooleanField("Default Config", default=False)
 
     def save(self, *args, **kwargs):
         # Do not allow more than 1 default
         ds = DocusignOrgTemplateConfig.objects.filter(
@@ -271,15 +273,16 @@
         db_table = "docusign_envelope_audit_log"
         verbose_name = "Docusign Envelope Audit Log"
         verbose_name_plural = "Docusign Envelopes Audits Logs"
 
     # etran_loan = models.ForeignKey('loans.EtranLoan',on_delete=models.SET_NULL, null=True)
     content_type = models.ForeignKey(
         to="contenttypes.ContentType",
-        on_delete=models.CASCADE,
+        on_delete=models.SET_NULL,
+        null=True,
         related_name="+",
         verbose_name=_("content type"),
     )
     object_pk = models.CharField(
         db_index=True, max_length=255, verbose_name=_("object pk")
     )
     event_received_at = models.DateTimeField(null=True, blank=True)
```

### Comparing `los_docusign-0.6.5/los_docusign/urls.py` & `los_docusign-0.6.6/los_docusign/urls.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/utils/XmlParser.py` & `los_docusign-0.6.6/los_docusign/utils/XmlParser.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/los_docusign/utils/api_handler.py` & `los_docusign-0.6.6/los_docusign/utils/api_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
 #
 """Module to define base handler for external API calls"""
 
 import json
 import logging
+import typing
 
 import requests
 from requests.exceptions import (
     ConnectionError,
     HTTPError,
     ProxyError,
     ReadTimeout,
@@ -51,15 +52,15 @@
         return kwargs
 
     def send_request(
         self,
         method,
         params=None,
         payload=None,
-        log_config: dict = None,
+        log_config: dict | None = None,
         add_custom_fields: bool = False,
         event=None,
         event_type="ENVELOPE",
     ):
         """Send API request for the given URL with the specified method, params and payload"""
         headers = self.get_headers()
```

### Comparing `los_docusign-0.6.5/los_docusign/utils/client.py` & `los_docusign-0.6.6/los_docusign/utils/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #
 # Created on Tue Dec 21 2021
 #
 # Copyright (c) 2021 Lenders Cooperative, a division of Summit Technology Group, Inc.
 #
 import json
 import logging
+import typing
 
 from django.conf import settings
 
-from .api_handler import ApiHandler
-from .docusign_helper import process_docusign_webhook, extract_documents
 from los_docusign.utils.validators import validate_payload
 
+from .api_handler import ApiHandler
+from .docusign_helper import process_docusign_webhook, process_webhook_response
+
 LOGGER = logging.getLogger("root")
 
 
 class DocuSignClient:
     def __init__(self, access_token: str, timeout: int, tenant_schema: str):
         self.account_id = settings.DOCUSIGN_API_ACCOUNT_ID
         self.api_key = f"Bearer {access_token}"
@@ -59,27 +61,26 @@
         preview_data = {
             "authenticationMethod": authentication_method,
             "email": email,
             "userName": user_name,
             "clientUserId": client_user_id,
             "returnUrl": return_url,
         }
-        LOGGER.info("Calling API Handler's send request for generate_docusign_preview_url")
+        LOGGER.info("Calling API Handler's send request for generate_docusign_preview_url: [%s]", preview_url)
         docusign_handler = ApiHandler(preview_url, self.api_key, self.tenant_schema, timeout=self.timeout)
         envelope_result = docusign_handler.send_request(
             method="POST", payload=json.dumps(preview_data), log_config=log_config, event="EMBEDDED_URL"
         )
 
         LOGGER.debug(
             f"generate_docusign_preview_url completed for envelope {envelope_id} with status; {envelope_result.status_code}. Preview Url Data: {envelope_result.text}"
         )
         return envelope_result
 
     def create_envelope(self, payload, log_config: dict = None):
-
         ## Validate necessary values from payload
         response = validate_payload(payload=payload)
         if response != "Success":
             if log_config:
                 log_entry = log_config.get("model")(
                     loan=log_config.get("loan"),
                     object_pk=log_config.get("object_pk"),
@@ -89,17 +90,17 @@
                     request_headers=log_config.get("request_headers"),
                     request_body=log_config.get("request_body"),
                     response_body=response,
                     request_time=log_config.get("timezone").now(),
                     response_time=log_config.get("timezone").now(),
                     tin=log_config.get("tin"),
                     request_ip=log_config.get("request_ip"),
-                    response_code=log_config.get("response_code"),
+                    response_code=log_config.get("response_code", 0),
                     event_type="ENVELOPE",
-                    event="SENT",
+                    event="CREATE",
                 )
                 log_entry.save()
             raise Exception(response)
 
         url = settings.DOCUSIGN_API_ENDPOINT
 
         resource_path = self.account_id + "/envelopes"
@@ -136,21 +137,25 @@
         docusign_handler = ApiHandler(doc_url, self.api_key, self.tenant_schema, timeout=self.timeout)
         doc_download_result = docusign_handler.send_request(method="GET", log_config=log_config, event="DOWNLOAD_DOC")
         LOGGER.info(
             f"download_docusign_document completed with status: {doc_download_result.status_code} for envelope id: {envelopeId}"
         )
         return doc_download_result
 
-    def process_docusign_notification(self, xml_string: str, log_config: dict = None):
-        return process_docusign_webhook(xml_string, log_config)
-
-    def extract_docusign_documents(self, xml_string: str):
-        return extract_documents(xml_string)
+    def process_docusign_notification(
+        self, xml_string: str, log_config: dict | None = None, webhook_json_sim_enabled: bool | None = False
+    ):
+        LOGGER.debug(f"JSON Webhook: {webhook_json_sim_enabled}")
+        return process_docusign_webhook(xml_string, log_config, webhook_json_sim_enabled)
+
+    def extract_docusign_documents(self, xml_string: str, webhook_json_sim_enabled: bool = False):
+        docusign_data_dict = process_webhook_response(xml_string, webhook_json_sim_enabled)
+        return docusign_data_dict["documents"]
 
-    def update_envelope_and_resend(self, envelope_id, signers_data: dict, log_config: dict = None):
+    def update_envelope_and_resend(self, envelope_id, signers_data: dict, log_config: dict | None = None):
         url = settings.DOCUSIGN_API_ENDPOINT
 
         signer_payload = {}
         signers = []
         for signer in signers_data:
             signer_data = {}
             signer_data["recipientId"] = signer["recipientId"]
```

### Comparing `los_docusign-0.6.5/los_docusign/utils/docusign_adapter.py` & `los_docusign-0.6.6/los_docusign/utils/docusign_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,30 +71,26 @@
         """
         This should be implemented by the application, and should set the
         organization to self.organization
         """
         raise NotImplementedError("You must implement this method")
 
     @abc.abstractmethod
-    def prepare_payload(
-        self, instance, payload, client_user_id, is_embedded_docusign, **kwargs
-    ) -> dict:
+    def prepare_payload(self, instance, payload, client_user_id, is_embedded_docusign, **kwargs) -> dict:
         """
         This should be implemented by the application, and should return a dictionary in the form of
         """
         raise NotImplementedError("You must implement this method")
 
     def _error_payload_not_configured_0001(self, connection):
         raise ValidationError(_("Docusign payload not configured"))
 
     def _error_in_progress_0002(self):
         raise ValidationError(
-            _(
-                "DocuSign for this application is already in process, please try again after some time."
-            )
+            _("DocuSign for this application is already in process, please try again after some time.")
         )
 
     def _error_high_volume_throttle_0003(self):
         raise ValidationError(
             _(
                 "Our electronic signature process is currently experiencing high volume and we are throttling requests to protect your experience. Please return after one or two hours to complete your signature process. Your application is complete and your place in line is reserved."
             )
@@ -120,58 +116,50 @@
     def _error_unknown_0007(self, loan, exception):
         raise ValidationError(
             _(
                 "Our electronic signature process is currently experiencing high volume and we are throttling requests to protect your experience. Please return after one or two hours to complete your signature process. Your application is complete and your place in line is reserved."
             )
         )
 
-    def process_docusign_error(
-        self, instance, docusign_envelope_stage_data, envelope_result
-    ):
+    def process_docusign_error(self, instance, docusign_envelope_stage_data, envelope_result):
         error_text = json.loads(envelope_result.text)
         error_code = error_text["errorCode"]
+
         if error_code in [
             "HOURLY_APIINVOCATION_LIMIT_EXCEEDED",
             "BURST_APIINVOCATION_LIMIT_EXCEEDED",
+            "HOURLY_APIINVOCATION_ENVELOPE_LIMIT_EXCEEDED",
         ]:
-            raise Exception(
-                "DocuSign API THROTTLING Error: {error_text}".format(
-                    error_text=envelope_result.text
-                )
-            )
-        else:
-            docusign_envelope_stage_data.record_status = "F"
-            docusign_envelope_stage_data.error_message = envelope_result.text
+            raise Exception("DocuSign API THROTTLING Error: {error_text}".format(error_text=envelope_result.text))
 
-            # Since we are creating a new instance
-            docusign_envelope_stage_data.save()  # nosemgrep
-            raise Exception(
-                "DocuSign Error: Failed to create the envelope for application"
-                " id: {instance_id} : {error_text}".format(
-                    instance_id=instance, error_text=envelope_result.text
-                )
-            )
+        docusign_envelope_stage_data.record_status = "F"
+        docusign_envelope_stage_data.error_message = envelope_result.text
 
-    def _get_envelope_content_type(self, instance):
-        return ContentType.objects.get(
-            model=instance._meta.model_name, app_label=instance._meta.app_label
+        # Since we are creating a new instance
+        docusign_envelope_stage_data.save()  # nosemgrep
+        raise Exception(
+            "DocuSign Error: Failed to create the envelope for application"
+            " id: {instance_id} : {error_text}".format(instance_id=instance, error_text=envelope_result.text)
         )
 
+    def _get_envelope_content_type(self, instance):
+        return ContentType.objects.get(model=instance._meta.model_name, app_label=instance._meta.app_label)
+
     def get_client_user_id(self, is_embedded_docusign):
         return str(randint(10000, 99999)) if is_embedded_docusign else None
 
     def _create_current_status(self, envelope_id, envelope_status, signers):
         recipients = []
         for signer in signers:
             recipient = {
                 "name": signer["name"],
                 "email": signer["email"],
                 "recipient_id": signer["recipientId"],
                 "routing_order": signer["routingOrder"],
-                "custom_fields": {"CustomField": signer["customFields"][0]},
+                "custom_fields": [signer["customFields"][0]],
                 "status": "created",
                 "phone_auth": {
                     "fail_count": None,
                     "status": None,
                     "last_event_time": None,
                 },
             }
@@ -200,17 +188,15 @@
             object_pk=instance.pk if instance else None,
         )
 
         docusign_envelope_stage_data.docusign_user = self.docusign_user
 
         docusign_envelope_stage_data.object_pk = instance.pk if instance else None
 
-        docusign_envelope_stage_data.content_type = self._get_envelope_content_type(
-            instance
-        )
+        docusign_envelope_stage_data.content_type = self._get_envelope_content_type(instance)
 
         if not payload:
             docusign_template = self.docusign_template
             docusign_los_payload = docusign_template.docusign_payload
         else:
             docusign_los_payload = payload
 
@@ -221,22 +207,18 @@
             request_payload = docusign_los_payload
         else:
             request_payload = json.loads(docusign_los_payload)
 
         # If consent is required, then a dict with consent url will be returned by the wrapper.
         if isinstance(self.access_token, dict):
             raise Exception(
-                "Docusign Consent is required for the user: {error_text}".format(
-                    error_text=self.access_token
-                )
+                "Docusign Consent is required for the user: {error_text}".format(error_text=self.access_token)
             )
 
-        client_user_id = self.get_client_user_id(
-            is_embedded_docusign=is_embedded_docusign
-        )
+        client_user_id = self.get_client_user_id(is_embedded_docusign=is_embedded_docusign)
 
         docusign_payload = self.prepare_payload(
             payload=request_payload,
             instance=instance,
             client_user_id=client_user_id,
             is_embedded_docusign=is_embedded_docusign,
             phase=phase,
@@ -279,38 +261,34 @@
                 "authenticationMethod": "None",
                 "email": signer_email,
                 "userName": signer_name,
                 "clientUserId": client_user_id,
                 "access_token": "Bearer " + self.access_token,
                 "returnUrl": return_url,
             }
-            envelope_result = self.docusign_client.generate_docusign_preview_url(
-                params, self.log_config
-            )
+            envelope_result = self.docusign_client.generate_docusign_preview_url(params, self.log_config)
             if self.use_signing_cache:
-                cache.set(f"docusign_embedded_signing:{self.id}", True, 600)
+                cache.set(f"docusign_embedded_signing:{instance.id}", True, 600)
             if envelope_result.status_code != 201:
-                return self.process_docusign_error(
-                    instance, docusign_envelope_stage_data, envelope_result
-                )
+                return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
 
             return envelope_result
 
     def _send_for_docusign(
         self,
         docusign_envelope_stage_data,
         client_user_id,
         request_payload,
         phase,
         instance,
         is_embedded_docusign,
         signer_email,
         signer_name,
         return_url,
-        **kwargs
+        **kwargs,
     ):
         """
         Handle common logic for sending data to docusign.  This should not be called directly by the application.
         """
         docusign_envelope_stage_data.client_user_id = client_user_id
 
         existing_envelope_result = self._check_for_existing_envelope(
@@ -320,17 +298,15 @@
             signer_email,
             signer_name,
             docusign_envelope_stage_data,
         )
         if existing_envelope_result:
             return existing_envelope_result
 
-        envelope_result = self.docusign_client.create_envelope(
-            request_payload, self.log_config
-        )
+        envelope_result = self.docusign_client.create_envelope(request_payload, self.log_config)
         docusign_envelope_stage_data.envelope_response = envelope_result.text
 
         if envelope_result.status_code == 201:
             resp = json.loads(envelope_result.text)
             docusign_envelope_stage_data.record_status = "S"
             docusign_envelope_stage_data.envelope_id = resp["envelopeId"]
             docusign_envelope_stage_data.envelope_status = resp["status"]
@@ -338,48 +314,38 @@
             current_status = self._create_current_status(
                 resp["envelopeId"],
                 resp["status"],
                 request_payload["recipients"]["signers"],
             )
             docusign_envelope_stage_data.current_status = current_status
 
-            self._envelope_response_audit_log(
-                instance, docusign_envelope_stage_data, current_status, resp
-            )
+            self._envelope_response_audit_log(instance, docusign_envelope_stage_data, current_status, resp)
 
             if is_embedded_docusign:
                 params = {
                     "envelope_id": resp["envelopeId"],
                     "authenticationMethod": "None",
                     "email": signer_email,
                     "userName": signer_name,
                     "clientUserId": client_user_id,
                     "returnUrl": return_url,
                 }
-                envelope_result = self.docusign_client.generate_docusign_preview_url(
-                    params, self.log_config
-                )
+                envelope_result = self.docusign_client.generate_docusign_preview_url(params, self.log_config)
                 if envelope_result.status_code != 201:
-                    return self.process_docusign_error(
-                        instance, docusign_envelope_stage_data, envelope_result
-                    )
+                    return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
                 if self.use_signing_cache:
                     cache.set(f"docusign_embedded_signing:{instance.id}", True, 600)
         else:
-            return self.process_docusign_error(
-                instance, docusign_envelope_stage_data, envelope_result
-            )
+            return self.process_docusign_error(instance, docusign_envelope_stage_data, envelope_result)
 
         # Since we are creating a new instance
         docusign_envelope_stage_data.save()  # nosemgrep
         return envelope_result
 
-    def _envelope_response_audit_log(
-        self, instance, docusign_envelope_stage_data, current_status, resp
-    ):
+    def _envelope_response_audit_log(self, instance, docusign_envelope_stage_data, current_status, resp):
         pass
 
     def initiate_docusign(
         self,
         return_url,
         phase,
         instance,
@@ -421,30 +387,30 @@
                 http.HTTPStatus.BAD_REQUEST,
                 http.HTTPStatus.UNAUTHORIZED,
                 http.HTTPStatus.NOT_FOUND,
                 http.HTTPStatus.UNSUPPORTED_MEDIA_TYPE,
             ]:
                 error_text = json.loads(response.text)
                 error_code = error_text["errorCode"]
+
                 if error_code == "HOURLY_APIINVOCATION_LIMIT_EXCEEDED":
                     if not cache.get("docusign_rate_reset", None):
                         reset_timestamp = int(response.headers["X-RateLimit-Reset"])
                         calculated_timeout = reset_timestamp - int(time.time())
-                        cache.set(
-                            "docusign_rate_reset",
-                            reset_timestamp,
-                            timeout=calculated_timeout,
-                        )
+                        cache.set("docusign_rate_reset", reset_timestamp, timeout=calculated_timeout)
+
                     return self._error_high_volume_throttle_0006()
+
                 elif error_code == "BURST_APIINVOCATION_LIMIT_EXCEEDED":
                     if not cache.get("docusign_rate_reset", None):
                         # Setting the timeout to 30 seconds as for burst limit
                         reset_timestamp = int(response.headers["X-RateLimit-Reset"])
                         cache.set("docusign_rate_reset", reset_timestamp, timeout=30)
 
                     return self._error_high_volume_throttle_0005()
+
                 else:
                     return self._error_docusigning_failed_0004()
         except Exception as excp:
             # TODO: Handle this with correct error code.
             return self._error_unknown_0007(instance, excp)
             raise
```

### Comparing `los_docusign-0.6.5/los_docusign/utils/docusign_helper.py` & `los_docusign-0.6.6/los_docusign/utils/docusign_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,40 +5,51 @@
 #
 import base64
 import hashlib
 import hmac
 import json
 import logging
 import re
-from datetime import datetime, timedelta
+from datetime import timedelta
 from os import path
 from xml.etree import cElementTree as ElementTree
 
 from django.conf import settings
 from django.http import Http404
 
 # import sentry_sdk
 from django.utils import timezone
 from docusign_esign import ApiClient
 from docusign_esign.client.api_exception import ApiException
 
 from los_docusign.models import (
-    DocusignEnvelopeAuditLog,
     DocusignEnvelopeStageData,
     DocusignOrgTemplate,
     DocuSignUserAuth,
 )
 
 from .XmlParser import XmlDictConfig
 
 SCOPES = ["signature"]
 
 LOGGER = logging.getLogger("root")
 
 
+def get_webhook_is_json(default: bool | None = None):
+    # `default` will allow other fn's to be able to accept input,
+    #  and keep the same logic without repeated if statements everywhere this is called
+    if default is not None:
+        return default
+    # if nothing was passed in, check settings
+    if hasattr(settings, "DOCUSIGN_ENABLE_JSON_SIM"):
+        return settings.DOCUSIGN_ENABLE_JSON_SIM
+    # if the setting is not found, fall back to xml
+    return False
+
+
 def get_docusign_user(organization_pk):
     try:
         # Try if the user is the available and has the docusign account
         docusign_user = DocuSignUserAuth.objects.get(organization_pk=organization_pk)
     except DocuSignUserAuth.DoesNotExist:
         # Else use the default user
         docusign_user = DocuSignUserAuth.objects.get(default_user=True)
@@ -49,15 +60,14 @@
 def get_access_token(docusign_user, redirect_url=None):
     docusign_token_expiry = settings.DOCUSIGN_TOKEN_EXPIRY_IN_SECONDS
 
     if docusign_user.expires_at >= timezone.now():
         access_token = docusign_user.access_token
     else:
         token_response = _jwt_auth(docusign_user.docusign_api_username, redirect_url)
-        # print(f"Token Response: {token_response}")
         try:
             if token_response["consent_url"]:
                 return token_response
         except TypeError as e:
             pass
         access_token = token_response.access_token
         docusign_user.access_token = access_token
@@ -144,15 +154,15 @@
 def populate_text_tabs(text_tabs_forms, text_tabs_data: dict):
     # Need to populate all the text tabs with the values
     for textTabsInfo in text_tabs_forms:
         tab_label = textTabsInfo["tabLabel"]
         try:
             textTabsInfo["value"] = text_tabs_data.get(tab_label)
         except KeyError as e:
-            print(f"Key not found {e}")
+            LOGGER.debug(f"Key not found {e}")
 
 
 def get_docusign_template(organization_pk, template_name=None):
     docusign_payload = None
     try:
         docusign_template = DocusignOrgTemplate.objects.get(
             organization_model="organization",
@@ -163,35 +173,100 @@
         dsua = DocuSignUserAuth.objects.get(default_user=True)
         docusign_template = DocusignOrgTemplate.objects.get(
             object_pk=dsua.object_pk, docusign_template__template_type=template_name
         ).docusign_template
 
     docusign_payload = docusign_template.docusign_payload
     if docusign_payload is None:
-        print("Payload Not found for org. Check database..return")
         LOGGER.error(f"Payload Not found for org {organization_pk}. Check database..return")
         return
 
     # resp = json.loads(docusign_payload)
     return docusign_payload
 
 
-def _read_response_webhook(xml_string):
+def _process_json_webhook_response(json_str):
+    docusign_response_obj = json.loads(json_str)
+
+    trimmed_object = {
+        "raw": docusign_response_obj,
+        "event": docusign_response_obj["event"],
+        "envelope_id": docusign_response_obj["data"]["envelopeId"],
+        "envelope_status": str(docusign_response_obj["data"]["envelopeSummary"]["status"]).lower(),
+        "custom_fields": {
+            field["name"]: field["value"]
+            for field in docusign_response_obj["data"]["envelopeSummary"]["customFields"]["listCustomFields"]
+        },
+        "recipients": [],
+    }
+
+    for raw_recipient in docusign_response_obj["data"]["envelopeSummary"].get("recipients", {}).get("signers", []):
+        recipient_data = {
+            "recipient_id": raw_recipient["recipientId"],
+            "email": raw_recipient["email"],
+            "name": raw_recipient["name"],
+            "sent_time": raw_recipient.get("sentDateTime", None),
+            "routing_order": raw_recipient["routingOrder"],
+            "custom_fields": raw_recipient.get("customFields"),
+            "status": raw_recipient["status"],
+        }
+
+        # recipient_auth_status = raw_recipient.get("RecipientAuthenticationStatus")
+        if recipient_auth_status := raw_recipient.get("RecipientAuthenticationStatus"):
+            phone_auth_status = recipient_auth_status.get("PhoneAuthResult", {})
+
+            recipient_data["raw_auth_status"] = recipient_auth_status
+            recipient_data["phone_auth_timestamp"] = phone_auth_status.get("EventTimestamp")
+
+        # XXX: this is missing from the sample json
+        # for rd_key, ras_key in (
+        #     ('id_question_status',"IDQuestionsResult"),
+        #     ('id_lookup_status',"IDLookupResult"),
+        #     ('phone_auth_status',"PhoneAuthResult"),
+        # ):
+        #     status = recipient_auth_status.get(ras_key)
+        #     if status is not None:
+        #         status = str(status.get("Status")).lower()
+
+        #     recipient_data[rd_key] = status
+
+        trimmed_object["recipients"].append(recipient_data)
+
+    # read and map documents
+    document_pdfs = docusign_response_obj["data"]["envelopeSummary"].get("envelopeDocuments", [])
+    if not isinstance(document_pdfs, list):
+        document_pdfs = [document_pdfs]
 
+    documents = []
+    for document_pdf in document_pdfs:
+        document = {
+            "name": document_pdf["name"],
+            "pdf_bytes": document_pdf["PDFBytes"],
+            "document_id": document_pdf.get("documentId"),
+            "document_type": document_pdf["type"],
+        }
+        documents.append(document)
+
+    trimmed_object["documents"] = documents
+
+    return trimmed_object
+
+
+def _process_xml_webhook_response(xml_string):
     root = ElementTree.XML(xml_string)
     request_data_dict = XmlDictConfig(root)
     m = re.search("{http://www.docusign.net/API/(.+?)}EnvelopeStatus", str(request_data_dict))
     api_version = None
     if m:
         api_version = m.group(1)
     else:
         # sentry_sdk.capture_exception(Exception(f'Failed to retrieve API Version for the DocuSign Webhook: {str(request_data_dict)}'))
         raise Http404
 
-    docusign_schema = "{http://www.docusign.net/API/" + api_version + "}"
+    docusign_schema = f"{{http://www.docusign.net/API/{api_version}}}"
 
     # Since we are not using any of the data sent back by DocuSign, we clear those fields which potentially causes json.dumps to fail to parse Decimal Values which are set by the Parser
     recipient_signers = request_data_dict[f"{docusign_schema}EnvelopeStatus"][f"{docusign_schema}RecipientStatuses"][
         f"{docusign_schema}RecipientStatus"
     ]
 
     if not isinstance(recipient_signers, list):
@@ -202,192 +277,193 @@
         recipients[f"{docusign_schema}FormData"] = None
 
     line = re.sub(
         r"({http://www.docusign.net/API/[0-9].[0-9]})",
         "",
         json.dumps(request_data_dict),
     )
-    docusign_data_dict = json.loads(line)
+    docusign_response_obj = json.loads(line)
 
-    return docusign_data_dict
+    trimmed_object = {
+        "raw": docusign_response_obj,
+        "envelope_id": docusign_response_obj["EnvelopeStatus"]["EnvelopeID"],
+        "envelope_status": str(docusign_response_obj["EnvelopeStatus"]["Status"]).lower(),
+        "custom_fields": {
+            docusign_response_obj["EnvelopeStatus"]["CustomFields"][field]["Name"]: docusign_response_obj[
+                "EnvelopeStatus"
+            ]["CustomFields"][field]["Value"]
+            for field in docusign_response_obj["EnvelopeStatus"]["CustomFields"]
+        },
+        "recipients": [],
+    }
+    recipient_statues = docusign_response_obj["EnvelopeStatus"]["RecipientStatuses"]
+    for raw_recipient in recipient_statues:
+        recipient_data = {
+            "recipient_id": recipient_statues[raw_recipient]["RecipientId"],
+            "email": recipient_statues[raw_recipient]["Email"],
+            "name": recipient_statues[raw_recipient]["UserName"],
+            "sent_time": recipient_statues[raw_recipient].get("Sent", None),
+            "routing_order": recipient_statues[raw_recipient]["RoutingOrder"],
+            "custom_fields": recipient_statues[raw_recipient].get("CustomFields"),
+            "status": recipient_statues[raw_recipient]["Status"],
+        }
+
+        recipient_auth_status = recipient_statues[raw_recipient].get("RecipientAuthenticationStatus", {})
+        phone_auth_status = (
+            recipient_statues[raw_recipient].get("RecipientAuthenticationStatus", {}).get("PhoneAuthResult", {})
+        )
+
+        recipient_data["raw_auth_status"] = recipient_auth_status
+        recipient_data["phone_auth_timestamp"] = phone_auth_status.get("EventTimestamp")
+
+        for rd_key, ras_key in (
+            ("id_question_status", "IDQuestionsResult"),
+            ("id_lookup_status", "IDLookupResult"),
+            ("phone_auth_status", "PhoneAuthResult"),
+        ):
+            status = recipient_auth_status.get(ras_key)
+            if status is not None:
+                status = str(status.get("Status")).lower()
+
+            recipient_data[rd_key] = status
+
+        trimmed_object["recipients"].append(recipient_data)
+
+    # read and map documents
+    document_pdfs = docusign_response_obj["DocumentPDFs"]["DocumentPDF"]
+    if not isinstance(document_pdfs, list):
+        document_pdfs = [document_pdfs]
 
+    documents = []
+    for document_pdf in document_pdfs:
+        document = {
+            "name": document_pdf["Name"],
+            "pdf_bytes": document_pdf["PDFBytes"],
+            "document_id": document_pdf.get("DocumentID"),
+            "document_type": document_pdf["DocumentType"],
+        }
+        documents.append(document)
 
-def process_docusign_webhook(xml_string, log_config, event=None, event_type="WEBHOOK"):
-    # request_data_dict = request.data
+    trimmed_object["documents"] = documents
 
-    docusign_data_dict = _read_response_webhook(xml_string)
+    return trimmed_object
 
-    envelopeId = docusign_data_dict["EnvelopeStatus"]["EnvelopeID"]
+
+def process_webhook_response(xml_string, webhook_json_sim_enabled=None):
+    if get_webhook_is_json(webhook_json_sim_enabled):
+        docusign_data_dict = _process_json_webhook_response(xml_string)
+    else:
+        docusign_data_dict = _process_xml_webhook_response(xml_string)
+    return docusign_data_dict
+
+
+def process_docusign_webhook(
+    xml_string,
+    log_config,
+    webhook_json_sim_enabled=None,
+    event=None,
+    event_type="WEBHOOK",
+):
+    docusign_data_dict = process_webhook_response(xml_string, webhook_json_sim_enabled)
+    envelopeId = docusign_data_dict["envelope_id"]
 
     try:
         envelope_stage_data = DocusignEnvelopeStageData.objects.get(envelope_id=envelopeId)
     except DocusignEnvelopeStageData.DoesNotExist:
         LOGGER.error(f"Envelope id  {envelopeId} not found in system")
         raise Exception(f"Envelope id  {envelopeId} not found in system")
 
-    return _extract_envelope_information(envelope_stage_data, docusign_data_dict, log_config, event, event_type)
-
-
-def extract_documents(xml_string):
-    root = ElementTree.XML(xml_string)
-    request_data_dict = XmlDictConfig(root)
-    line = re.sub(
-        r"({http://www.docusign.net/API/[0-9].[0-9]})",
-        "",
-        json.dumps(request_data_dict),
-    )
-    docusign_data_dict = json.loads(line)
-    documents = []
-    document_pdfs = docusign_data_dict["DocumentPDFs"]["DocumentPDF"]
-    if isinstance(document_pdfs, list):
-        for document_pdf in document_pdfs:
-            document = {}
-            document["name"] = document_pdf["Name"]
-            document["pdf_bytes"] = document_pdf["PDFBytes"]
-            try:
-                document["document_id"] = document_pdf["DocumentID"]
-            except KeyError as e:
-                document["document_id"] = None
-            document["document_type"] = document_pdf["DocumentType"]
-            documents.append(document)
-    else:
-        document = {}
-        document["name"] = document_pdfs["Name"]
-        document["pdf_bytes"] = document_pdfs["PDFBytes"]
-        try:
-            document["document_id"] = document_pdfs["DocumentID"]
-        except KeyError as e:
-            document["document_id"] = None
-        document["document_type"] = document_pdfs["DocumentType"]
-        documents.append(document)
-    return documents
+    return _extract_envelope_information(envelope_stage_data, docusign_data_dict, log_config, event_type)
 
 
-def _extract_envelope_information(
-    envelope_stage_data, docusign_data_dict, log_config=None, event=None, event_type="WEBHOOK"
-):
+def _extract_envelope_information(envelope_stage_data, docusign_data_dict, log_config=None, event_type="WEBHOOK"):
+    event_value = None
     try:
-        envelopeId = docusign_data_dict["EnvelopeStatus"]["EnvelopeID"]
-        recipients = docusign_data_dict["EnvelopeStatus"]["RecipientStatuses"]["RecipientStatus"]
-        envelope_status = docusign_data_dict["EnvelopeStatus"]["Status"]
-        envelope_status = str(envelope_status).lower()
-        envelope_output = {}
+        envelope_id = docusign_data_dict["envelope_id"]
+        recipients = docusign_data_dict["recipients"]
+        envelope_status = str(docusign_data_dict["envelope_status"]).lower()
 
         if not isinstance(recipients, list):
             recipients = [recipients]
 
         recipient_failed_delivery = False
         recipient_failed_authentication = False
         recipients_data = []
         for recipient in recipients:
-            recipient_data = {}
+            recipient_data = {
+                "recipient_id": recipient["recipient_id"],
+                "email": recipient["email"],
+                "name": recipient["name"],
+                "sent_time": recipient["sent_time"],
+                "routing_order": recipient["routing_order"],
+                "custom_fields": recipient["custom_fields"],
+                "status": recipient["status"],
+            }
+
+            recipient_auth_status = recipient.get("raw_auth_status")
+            recipient_id_question_status = recipient.get("id_question_status")
+            recipient_id_lookup_status = recipient.get("id_lookup_status")
+            recipient_phone_auth_status = recipient.get("phone_auth_status")
+            recipient_status = str(recipient_data["status"]).lower()
 
-            recipient_status = recipient["Status"]
-            email = recipient["Email"]
-            username = recipient["UserName"]
-            recipient_id = recipient["RecipientId"]
-            sent_time = recipient.get("Sent", None)
-            routing_order = recipient["RoutingOrder"]
-
-            try:
-                custom_fields = recipient["CustomFields"]
-            except KeyError as e:
-                custom_fields = None
-
-            recipient_auth_status = recipient.get("RecipientAuthenticationStatus", None)
-            recipient_id_question_status = None
-            recipient_id_lookup_status = None
-            recipient_phone_auth_status = None
+            recipient_data["phone_auth"] = {}
 
             if recipient_auth_status:
-                recipient_idquestion_result = recipient_auth_status.get("IDQuestionsResult", None)
-
-                recipient_id_lookup_result = recipient_auth_status.get("IDLookupResult", None)
-
-                recipient_phone_auth_result = recipient_auth_status.get("PhoneAuthResult", None)
-
-                if recipient_idquestion_result:
-                    recipient_id_question_status = recipient_idquestion_result["Status"]
-                    recipient_id_question_status = str(recipient_id_question_status).lower()
-                if recipient_id_lookup_result:
-                    recipient_id_lookup_status = recipient_id_lookup_result["Status"]
-                    recipient_id_lookup_status = str(recipient_id_lookup_status).lower()
-
-                if recipient_phone_auth_result:
-                    recipient_phone_auth_status = recipient_phone_auth_result["Status"]
-                    recipient_phone_auth_status = str(recipient_phone_auth_status).lower()
+                phone_auth = {}
+                current_status = envelope_stage_data.current_status
 
+                if recipient_status in ["autoresponded"]:
+                    recipient_failed_delivery = True
                 if "failed" in (
                     recipient_id_lookup_status,
                     recipient_id_question_status,
                     recipient_phone_auth_status,
                 ):
                     recipient_status = "authentication failed"
                     recipient_failed_authentication = True
 
-            recipient_status = str(recipient_status).lower()
-
-            if recipient_status in ["autoresponded"]:
-                recipient_failed_delivery = True
-
-            recipient_data["recipient_id"] = recipient_id
-            recipient_data["email"] = email
-            recipient_data["name"] = username
-            recipient_data["status"] = recipient_status
-            recipient_data["sent_time"] = sent_time
-            recipient_data["routing_order"] = routing_order
-            if custom_fields:
-                recipient_data["custom_fields"] = custom_fields
-
-            recipient_data["phone_auth"] = {}
-            if recipient_auth_status is not None:
-                phone_auth = {}
-                current_status = envelope_stage_data.current_status
                 if current_status is None:
                     if recipient_phone_auth_status:
-                        phone_auth["status"] = recipient_phone_auth_status
-                        phone_auth["last_event_time"] = recipient_phone_auth_result["EventTimestamp"]
-                        if recipient_phone_auth_status == "passed":
-                            phone_auth["fail_count"] = 0
-                        else:
-                            phone_auth["fail_count"] = 1
+                        phone_auth = {
+                            "status": recipient_phone_auth_status,
+                            "last_event_time": recipient["phone_auth_timestamp"],
+                            "fail_count": (0 if recipient_phone_auth_status == "passed" else 1),
+                        }
                     recipient_data["phone_auth"] = phone_auth
                 else:
-                    recipient_status = current_status["recipients"]
-                    for recipient in recipient_status:
-                        phone_auth = recipient["phone_auth"]
+                    current_status_recipients = current_status["recipients"]
+                    for current_recipient in current_status_recipients:
+                        phone_auth = current_recipient.get("phone_auth")
                         if (
-                            recipient["email"] == recipient_data["email"]
-                            and recipient["name"] == recipient_data["name"]
-                            and recipient["custom_fields"]["CustomField"] in custom_fields["CustomField"]
+                            current_recipient["email"] == recipient_data["email"]
+                            and current_recipient["name"] == recipient_data["name"]
+                            and current_recipient["custom_fields"]["CustomField"] in recipient_data["custom_fields"]
                         ):
                             # Currently not relying on the recipient id as we do store the sent recipient id and we receive the Docusign internal recipient id
-                            if phone_auth is {}:
-                                phone_auth["fail_count"] = None
-                                phone_auth["status"] = None
-                                phone_auth["last_event_time"] = None
+                            if phone_auth is None:
+                                phone_auth = {
+                                    "fail_count": None,
+                                    "status": None,
+                                    "last_event_time": None,
+                                }
 
                             if recipient_phone_auth_status:
                                 if recipient_phone_auth_status == "passed":
                                     phone_auth["fail_count"] = 0
                                 else:
-                                    if phone_auth.get("fail_count", None):
-                                        fail_count = phone_auth["fail_count"]
-                                        fail_count = fail_count + 1
-                                        phone_auth["fail_count"] = fail_count
+                                    if phone_auth.get("fail_count"):
+                                        phone_auth["fail_count"] += 1
                                     else:
-                                        fail_count = 1
-                                        phone_auth["fail_count"] = fail_count
+                                        phone_auth["fail_count"] = 1
                                         phone_auth["status"] = recipient_phone_auth_status
-                                        phone_auth["last_event_time"] = recipient_phone_auth_result["EventTimestamp"]
+                                        phone_auth["last_event_time"] = recipient["phone_auth_timestamp"]
                             recipient_data["phone_auth"] = phone_auth
                             break
 
             recipients_data.append(recipient_data)
-            # envelope_output["recipients"].append(recipient_data)
 
         # Let's not overwrite the status of authentication failed if the recipient failed authentication.
         # We need this to know if the receipient failed authentication and later on completed the application
         # Assigning the envelope status value to recipient status as the for multiple signers,
         # Env status will be updated to "Completed" only when all signers sign.
 
         if not envelope_stage_data.recipient_status == "authentication failed":
@@ -398,26 +474,26 @@
             recipient_id_question_status,
             recipient_phone_auth_status,
         ):
             envelope_stage_data.recipient_status = "authentication failed"
             envelope_stage_data.recipient_auth_info = recipient_auth_status
             recipient_status = "authentication failed"
 
-        if recipient_failed_delivery:
-            recipient_status = "autoresponded"
-
         if recipient_failed_authentication:
             recipient_status = "authentication failed"
+        elif recipient_failed_delivery:
+            recipient_status = "autoresponded"
+        else:
+            recipient_status = ""
 
         event_value = envelope_status
 
         if recipient_status == "authentication failed" and envelope_status == "sent":
             event_value = "authentication failed"
-
-        if recipient_status == "autoresponded" and envelope_status == "sent":
+        elif recipient_status == "autoresponded" and envelope_status == "sent":
             event_value = "autoresponded"
 
         # TODO: Need to understand how can we log this in the DocuSignEnvelopeAuditLog, since we do not have the content type?
         # log = DocusignEnvelopeAuditLog(
         #     content_type=envelope_stage_data.content_type,
         #     object_pk=envelope_stage_data.object_pk,
         #     event_received_at=datetime.now(),
@@ -449,26 +525,25 @@
             )
             log_entry.save()
 
         if event_value == "authentication failed":
             envelope_status = "authentication failed"
 
         envelope_output = {
-            "envelopeId": envelopeId,
+            "envelopeId": envelope_id,
             "envelope_status": envelope_status,
             "recipients": recipients_data,
         }
         envelope_stage_data.envelope_status = envelope_status
         envelope_stage_data.current_status = envelope_output
         envelope_stage_data.recipient_status = recipient_status
         # envelope_stage_data.updated_at = timezone.now()
         envelope_stage_data.save()
 
-        print(f"END process_docusign_notification: {envelopeId}")
-        LOGGER.debug(f"END process_docusign_notification: {envelopeId}")
+        LOGGER.debug(f"END process_docusign_notification: {envelope_id}")
 
     except Exception as e:
         LOGGER.error(f"Exception while extracting status from Webhook notification: {e}")
         if log_config:
             log_entry = log_config.get("model")(
                 loan=log_config.get("loan"),
                 object_pk=log_config.get("object_pk"),
```

### Comparing `los_docusign-0.6.5/los_docusign/utils/validators.py` & `los_docusign-0.6.6/los_docusign/utils/validators.py`

 * *Files identical despite different names*

### Comparing `los_docusign-0.6.5/pyproject.toml` & `los_docusign-0.6.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "los_docusign"
-version = "0.6.5"
+version = "0.6.6"
 description = "Docusign Django Wrapper for integrating DocuSign with Django Application"
 authors = ["tejasb <tejas@thesummitgrp.com>"]
 homepage = "https://github.com/Lenders-Cooperative/Django-DocuSign"
 license = "BSD-3-Clause"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-Django = "^3.1.13"
+python = "^3.10.2"
+Django = "3.2.15"
 docusign-esign = "^3.6.0"
 django-utils-six = "^2.0"
 django-environ = "^0.4.5"
 PyJWT = "2.4"
 django-model-utils = "^4.1.1"
 django-lc-utils = "^0.2.1"
 requests = "^2.26.0"
```

### Comparing `los_docusign-0.6.5/setup.py` & `los_docusign-0.6.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: los-docusign
+Version: 0.6.6
+Summary: Docusign Django Wrapper for integrating DocuSign with Django Application
+Home-page: https://github.com/Lenders-Cooperative/Django-DocuSign
+License: BSD-3-Clause
+Author: tejasb
+Author-email: tejas@thesummitgrp.com
+Requires-Python: >=3.10.2,<4.0.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (==3.2.15)
+Requires-Dist: PyJWT (==2.4)
+Requires-Dist: django-environ (>=0.4.5,<0.5.0)
+Requires-Dist: django-lc-utils (>=0.2.1,<0.3.0)
+Requires-Dist: django-model-utils (>=4.1.1,<5.0.0)
+Requires-Dist: django-utils-six (>=2.0,<3.0)
+Requires-Dist: docusign-esign (>=3.6.0,<4.0.0)
+Requires-Dist: phonenumbers (==8.12.26)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
+
+# Django-DocuSign
+Django wrapper app for DocuSign functionalities
+
+`pip install django-docusign`
+
+## Running Tests
+We have a unit test defined for testing the los application.
+This can be executed using the below command.
+
+```
+python manage.py test
+```
+
+## Usage
+In order to use the system you must add los_docusign.apps.LosDocusignConfig to your installed apps in your settings.py file.
+```python
+INSTALLED_APPS = [
+    'los_docusign'
+]
+```
+
+Test file has the sample implementation of the test_app
+
+## Functions in client.py
+1.  generate_docusign_preview_url(dict)
+
+    Params required in dict:
+    -   "envelope_id"
+    -   "authentication_method"
+    -   "email"
+    -   "user_name"
+    -   "client_user_id"
+    -   "return_url"
+
+2. create_envelope(payload)
+
+    Params required:
+    -   DocuSign payload in JSON format
+
+3. download_docusign_document(dict)
+
+    Params required in dict:
+    -   "envelope_id"
+    -   "doc_download_option"
+        -   Valid Values:
+            1. archive - If the document to be downloaded in zip format.
+            2. combined - If the document to be downloaded as a combined document.
+
+4. process_docusign_webhook(xml_string)
+
+    Params required:
+    -   Webhook XML string received from Docusign.
+
+    Response dict:
+        {
+            "envelopeId": "c57ec066-c5fa-4aa0-873d-6f285d70242a",
+            "envelope_status": "sent",
+            "recipients": [
+                {
+                    "recipient_id": "a7f73f21-c4ff-4bcb-97c4-b03c91b8528a",
+                    "email": "test@test.com",
+                    "name": "John Nash",
+                    "status": "autoresponded"
+                },
+                {
+                    "recipient_id": "511b2ad3-6650-4773-a6b4-47f64a0ccdaf",
+                    "email": "jerry@test.com",
+                    "name": "Jerry Tunes",
+                    "status": "created"
+                },
+                {
+                    "recipient_id": "0851505f-5af2-42df-bce4-9e0ebe8bd2e2",
+                    "email": "tom@test.com",
+                    "name": "Tom Tunes",
+                    "status": "created"
+                }
+            ]
+        }
+
+5. update_envelope_and_resend(envelope_id, signers_data)
+This function is used to update the email/phone number of the signer.
+This is also used to resend the same envelope to the signers. For resending, recipientId and email are mandatory.
+
+    Params required:
+    -   envelope_id - The envelope id for which we need to update the signers information or send the same envelope to the signers.
+    -   signers_data - The signer array which has the information about the signers that needs to be updated.
+    Params required in signers_data:
+    -   email - The email of the signer.
+    -   recipientId - The recipient id of the signer
+    -   phone  - The phone number of the signer (optional)
+
+    signers_data example:
+    [
+        {
+            "recipientId":"123456",
+            "email":"test@test.com",
+            "phone":"1234567890"
+        }
+    ]
+
+5. update_envelope_status(status_info):
+This function is used to update the status of the envelope.
+
+    Params required:
+    -   status_info - The dictionary variale which has the following parameters.
+        - envelope_id - The envelope id for which the status needs to be updated
+        - status - The status in which we need to set the envelope
+        - reason - The reason (if applicable) to be set for the status change. This will be visible to the signer
+
+    status_info example:
+    {
+        "envelope_id":"b1435c5d-3d67-46e8-ab6a-54789f42924e",
+        "status":"voided",
+        "reason":"Voiding an envelope"
+    }
+    
 
-packages = \
-['los_docusign', 'los_docusign.migrations', 'los_docusign.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Django>=3.1.13,<4.0.0',
- 'PyJWT==2.4',
- 'django-environ>=0.4.5,<0.5.0',
- 'django-lc-utils>=0.2.1,<0.3.0',
- 'django-model-utils>=4.1.1,<5.0.0',
- 'django-utils-six>=2.0,<3.0',
- 'docusign-esign>=3.6.0,<4.0.0',
- 'phonenumbers==8.12.26',
- 'requests>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'los-docusign',
-    'version': '0.6.5',
-    'description': 'Docusign Django Wrapper for integrating DocuSign with Django Application',
-    'long_description': '# Django-DocuSign\nDjango wrapper app for DocuSign functionalities\n\n`pip install django-docusign`\n\n## Running Tests\nWe have a unit test defined for testing the los application.\nThis can be executed using the below command.\n\n```\npython manage.py test\n```\n\n## Usage\nIn order to use the system you must add los_docusign.apps.LosDocusignConfig to your installed apps in your settings.py file.\n```python\nINSTALLED_APPS = [\n    \'los_docusign\'\n]\n```\n\nTest file has the sample implementation of the test_app\n\n## Functions in client.py\n1.  generate_docusign_preview_url(dict)\n\n    Params required in dict:\n    -   "envelope_id"\n    -   "authentication_method"\n    -   "email"\n    -   "user_name"\n    -   "client_user_id"\n    -   "return_url"\n\n2. create_envelope(payload)\n\n    Params required:\n    -   DocuSign payload in JSON format\n\n3. download_docusign_document(dict)\n\n    Params required in dict:\n    -   "envelope_id"\n    -   "doc_download_option"\n        -   Valid Values:\n            1. archive - If the document to be downloaded in zip format.\n            2. combined - If the document to be downloaded as a combined document.\n\n4. process_docusign_webhook(xml_string)\n\n    Params required:\n    -   Webhook XML string received from Docusign.\n\n    Response dict:\n        {\n            "envelopeId": "c57ec066-c5fa-4aa0-873d-6f285d70242a",\n            "envelope_status": "sent",\n            "recipients": [\n                {\n                    "recipient_id": "a7f73f21-c4ff-4bcb-97c4-b03c91b8528a",\n                    "email": "test@test.com",\n                    "name": "John Nash",\n                    "status": "autoresponded"\n                },\n                {\n                    "recipient_id": "511b2ad3-6650-4773-a6b4-47f64a0ccdaf",\n                    "email": "jerry@test.com",\n                    "name": "Jerry Tunes",\n                    "status": "created"\n                },\n                {\n                    "recipient_id": "0851505f-5af2-42df-bce4-9e0ebe8bd2e2",\n                    "email": "tom@test.com",\n                    "name": "Tom Tunes",\n                    "status": "created"\n                }\n            ]\n        }\n\n5. update_envelope_and_resend(envelope_id, signers_data)\nThis function is used to update the email/phone number of the signer.\nThis is also used to resend the same envelope to the signers. For resending, recipientId and email are mandatory.\n\n    Params required:\n    -   envelope_id - The envelope id for which we need to update the signers information or send the same envelope to the signers.\n    -   signers_data - The signer array which has the information about the signers that needs to be updated.\n    Params required in signers_data:\n    -   email - The email of the signer.\n    -   recipientId - The recipient id of the signer\n    -   phone  - The phone number of the signer (optional)\n\n    signers_data example:\n    [\n        {\n            "recipientId":"123456",\n            "email":"test@test.com",\n            "phone":"1234567890"\n        }\n    ]\n\n5. update_envelope_status(status_info):\nThis function is used to update the status of the envelope.\n\n    Params required:\n    -   status_info - The dictionary variale which has the following parameters.\n        - envelope_id - The envelope id for which the status needs to be updated\n        - status - The status in which we need to set the envelope\n        - reason - The reason (if applicable) to be set for the status change. This will be visible to the signer\n\n    status_info example:\n    {\n        "envelope_id":"b1435c5d-3d67-46e8-ab6a-54789f42924e",\n        "status":"voided",\n        "reason":"Voiding an envelope"\n    }\n    \n',
-    'author': 'tejasb',
-    'author_email': 'tejas@thesummitgrp.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Lenders-Cooperative/Django-DocuSign',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

