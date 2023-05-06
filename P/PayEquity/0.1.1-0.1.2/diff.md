# Comparing `tmp/PayEquity-0.1.1.tar.gz` & `tmp/PayEquity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PayEquity-0.1.1.tar", last modified: Sat May  6 15:05:20 2023, max compression
+gzip compressed data, was "PayEquity-0.1.2.tar", last modified: Sat May  6 21:06:40 2023, max compression
```

## Comparing `PayEquity-0.1.1.tar` & `PayEquity-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:20.321856 PayEquity-0.1.1/
--rw-rw-rw-   0        0        0      153 2023-05-01 01:45:33.000000 PayEquity-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7576 2023-05-06 15:05:20.320855 PayEquity-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:20.269845 PayEquity-0.1.1/PayEquity.egg-info/
--rw-rw-rw-   0        0        0     7576 2023-05-06 15:05:19.000000 PayEquity-0.1.1/PayEquity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-06 15:05:20.000000 PayEquity-0.1.1/PayEquity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 15:05:19.000000 PayEquity-0.1.1/PayEquity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 15:05:19.000000 PayEquity-0.1.1/PayEquity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 15:05:19.000000 PayEquity-0.1.1/PayEquity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:20.303851 PayEquity-0.1.1/payequity/
--rw-rw-rw-   0        0        0    15966 2023-05-01 01:44:26.000000 PayEquity-0.1.1/payequity/Audit.py
--rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.1/payequity/JobGroup.py
--rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.1/payequity/JobGroupEnssemble.py
--rw-rw-rw-   0        0        0    22425 2023-05-01 02:32:23.000000 PayEquity-0.1.1/payequity/Regressor.py
--rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.1/payequity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:20.319855 PayEquity-0.1.1/payequity/tests/
--rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.1/payequity/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.1/payequity/tests/test_audit.py
--rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.1/payequity/tests/test_job_group.py
--rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.1/payequity/tests/test_job_group_enssemble.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.1/payequity/tests/test_regressor.py
--rw-rw-rw-   0        0        0       21 2023-05-01 01:45:29.000000 PayEquity-0.1.1/payequity/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 15:05:20.321856 PayEquity-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-05-06 14:59:20.000000 PayEquity-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:06:40.771159 PayEquity-0.1.2/
+-rw-rw-rw-   0        0        0      355 2023-05-06 21:04:37.000000 PayEquity-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7576 2023-05-06 21:06:40.770159 PayEquity-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 21:06:40.757156 PayEquity-0.1.2/PayEquity.egg-info/
+-rw-rw-rw-   0        0        0     7576 2023-05-06 21:06:40.000000 PayEquity-0.1.2/PayEquity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-06 21:06:40.000000 PayEquity-0.1.2/PayEquity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 21:06:40.000000 PayEquity-0.1.2/PayEquity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 21:06:40.000000 PayEquity-0.1.2/PayEquity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 21:06:40.000000 PayEquity-0.1.2/PayEquity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 21:06:40.764157 PayEquity-0.1.2/payequity/
+-rw-rw-rw-   0        0        0    16221 2023-05-06 18:30:03.000000 PayEquity-0.1.2/payequity/Audit.py
+-rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.2/payequity/JobGroup.py
+-rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.2/payequity/JobGroupEnssemble.py
+-rw-rw-rw-   0        0        0    22436 2023-05-06 20:26:01.000000 PayEquity-0.1.2/payequity/Regressor.py
+-rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.2/payequity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:06:40.769158 PayEquity-0.1.2/payequity/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.2/payequity/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.2/payequity/tests/test_audit.py
+-rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.2/payequity/tests/test_job_group.py
+-rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.2/payequity/tests/test_job_group_enssemble.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.2/payequity/tests/test_regressor.py
+-rw-rw-rw-   0        0        0       21 2023-05-06 21:03:14.000000 PayEquity-0.1.2/payequity/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 21:06:40.771159 PayEquity-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-06 14:59:20.000000 PayEquity-0.1.2/setup.py
```

### Comparing `PayEquity-0.1.1/LICENSE.txt` & `PayEquity-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/MANIFEST.in` & `PayEquity-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/PKG-INFO` & `PayEquity-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.1/PayEquity.egg-info/PKG-INFO` & `PayEquity-0.1.2/PayEquity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.1/PayEquity.egg-info/SOURCES.txt` & `PayEquity-0.1.2/PayEquity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/README.md` & `PayEquity-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/payequity/Audit.py` & `PayEquity-0.1.2/payequity/Audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import date
 import string
 import pandas.io.formats.excel
 import numpy as np
 from scipy.stats import ttest_ind
 
 pandas.io.formats.excel.ExcelFormatter.header_style = None
+from io import BytesIO
 
 class Audit():
 #     def __str__(self):
 #         pass
     
 #     def __repr__(self):
 #         return "<Job Group Object> {} | Headcount: {}".format(self.name, self.df.shape[0])
@@ -181,18 +182,21 @@
         summary["Model"]=self.name
         self.summary = summary[[x for x in summary.columns if x not in exclude]].rename({'Ratio':'DoF Ratio'},
                                                                                         axis=1
                                                                                        )
 
         self.logger.info("Audit updated with compiled summary")
 
-    def export_all(self, version="", diagnostic=True, predictions=True, iter=False):
-
+    def export_all(self, version="", diagnostic=True, predictions=True, iter=False, io=False):
+        
+        output = BytesIO()
         version = date.today().strftime("%d.%m.%Y")+version
-        writer = pd.ExcelWriter('{} Pay Equity Audit {}.xlsx'.format(self.name, version), engine='xlsxwriter')
+        filename= '{} Pay Equity Audit {}.xlsx'.format(self.name, version)
+        path = output if io else filename
+        writer = pd.ExcelWriter(path, engine='xlsxwriter')
         workbook = writer.book
 
         header_fmt = workbook.add_format({"bg_color": "#ed1b2c","bold": True,'font_color': '#FFFFFF','border': 1})
         default_fmt_dict = {"bg_color":"#FFFFFF", 'border': 1}
         default_fmt = workbook.add_format(default_fmt_dict)
         
         money_fmt = workbook.add_format(dict(list({'num_format':'$#,##0'}.items())+ list(default_fmt_dict.items())))
@@ -291,17 +295,22 @@
         for sheet in df_dict:
             # print(sheet)
             df_dict[sheet].to_excel(writer, index=False, sheet_name=sheet) 
             worksheet = writer.sheets[sheet]
             self._format_worksheet(worksheet, df_dict[sheet], sheet_format[sheet])
             
         
-        writer.close()
+        writer.save()
+        
         if iter:
             self._export_iter_regressions(version=version)
+        
+        if io:
+            processed_data = output.getvalue()
+            return processed_data
 
     def _format_worksheet(self, worksheet, df, format_dict):
 
         last_idx = 0
         for idx, col in enumerate(df):  # loop through all columns
             series = df[col]
```

### Comparing `PayEquity-0.1.1/payequity/JobGroup.py` & `PayEquity-0.1.2/payequity/JobGroup.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/payequity/JobGroupEnssemble.py` & `PayEquity-0.1.2/payequity/JobGroupEnssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/payequity/Regressor.py` & `PayEquity-0.1.2/payequity/Regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         init_stat = sig if "S2" in scenario else gap
         crit = 0.05 if "S2" in scenario else 0
         self.logger.info("Variable: {} | Init Gap: {:.2%} | Init Sig: {:.3f}".format(variable, gap, sig))
 
         if "S1" in scenario:
             pred, gap, sig, alpha = self._remediate_outliers(variable)
 
-        elif init_stat < crit:
+        elif init_stat < crit and gap <0:
             pred, gap, sig, alpha =  self._remediation_loop(scenario, init_stat, crit, 
             eligibility, variable, _from, init_gap=gap, init_sig=sig)
         
         else:
             pred = self.predictions[["Actual",_from]].copy().rename({_from:'Adjusted Pay'}, axis=1)
             alpha=0.95
```

### Comparing `PayEquity-0.1.1/payequity/tests/test_job_group.py` & `PayEquity-0.1.2/payequity/tests/test_job_group.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/payequity/tests/test_job_group_enssemble.py` & `PayEquity-0.1.2/payequity/tests/test_job_group_enssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.1/setup.py` & `PayEquity-0.1.2/setup.py`

 * *Files identical despite different names*

