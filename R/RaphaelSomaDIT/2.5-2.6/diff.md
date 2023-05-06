# Comparing `tmp/RaphaelSomaDIT-2.5-py3-none-any.whl.zip` & `tmp/RaphaelSomaDIT-2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5061 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    10739 b- defN 23-Apr-28 10:09 RaphaelSomaDIT/__init__.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      434 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      591 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/RECORD
-7 files, 14024 bytes uncompressed, 4007 bytes compressed:  71.4%
+Zip file size: 5319 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    11743 b- defN 23-May-06 19:13 RaphaelSomaDIT/__init__.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      447 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      591 b- defN 23-May-06 19:32 RaphaelSomaDIT-2.6.dist-info/RECORD
+7 files, 15041 bytes uncompressed, 4265 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: RaphaelSomaDIT/__init__.py
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/LICENSE
+Filename: RaphaelSomaDIT-2.6.dist-info/LICENSE
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/LICENSE.txt
+Filename: RaphaelSomaDIT-2.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/METADATA
+Filename: RaphaelSomaDIT-2.6.dist-info/METADATA
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/WHEEL
+Filename: RaphaelSomaDIT-2.6.dist-info/WHEEL
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/top_level.txt
+Filename: RaphaelSomaDIT-2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.5.dist-info/RECORD
+Filename: RaphaelSomaDIT-2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RaphaelSomaDIT/__init__.py

```diff
@@ -29,35 +29,36 @@
     overall_status=''
     sem1_csv=''
     sem2_csv=''
     overall_sem_csv=''
     error = ''
     level =""
     sem = ""
+    results = True
     
     
     
     def result(self,email, password):
-        self.sem1,
-        self.sem2, 
-        self.total_results,
-        self.sem1_csv,
-        self.sem2_csv, 
-        self.overall_sem_csv,
-        self.GPA_sem1=''
-        self.GPA_sem2=''
-        self.GPA_sem1_status=''
-        self.GPA_sem2_status=''
-        self.overall_GPA=''
-        self.overall_status=''
-        
+            self.sem1,
+            self.sem2, 
+            self.total_results,
+            self.sem1_csv,
+            self.sem2_csv, 
+            self.overall_sem_csv,
+            self.GPA_sem1=''
+            self.GPA_sem2=''
+            self.GPA_sem1_status=''
+            self.GPA_sem2_status=''
+            self.overall_GPA=''
+            self.overall_status=''
+            self.results=True
        
         
         
-        try:
+        # try:
             login_url = 'https://soma.dit.ac.tz/login'
             secure_url = 'https://soma.dit.ac.tz/'
             session = requests.Session()
             secure_url = 'https://soma.dit.ac.tz/'
             request = session.get(login_url).content
 
             soup = bs(request,'html.parser')
@@ -89,15 +90,39 @@
                 self.total_results= pd.read_html(total_result)
                 
                 total_result = bs(total_result,'html.parser')
                 self.sem1 = pd.DataFrame(self.total_results[0])
                 #self.sem1.to_csv('matokeo_sem1.csv',index=False)
 
                 self.sem2 = pd.DataFrame(self.total_results[1])
-                
+                total_r = total_result
+                self.results=True
+                if self.results:
+                    section = total_r.find('section')
+                    html_file = 'section.html'
+                    with open(html_file, 'w') as file:
+                        file.write(str(section))
+
+                    # Convert HTML to PDF using pdfkit
+                
+                    from xhtml2pdf import pisa
+
+    # Convert HTML to PDF
+                    html_file = 'section.html'
+                    pdf_file = 'result.pdf'
+
+                    with open(html_file, 'r') as file:
+                        html_content = file.read()
+
+                    with open(pdf_file, 'w+b') as file:
+                        pisa.CreatePDF(html_content, dest=file)
+
+                    # Remove the temporary HTML file
+                    import os
+                    os.remove(html_file)
                 sem_pga = total_result.find_all('h6')
                 sem_pga_total = total_result.find_all('h5')
                 h6 = []
                 h5=[]
                 
                 for sem_pga in sem_pga:
                     h6.append(sem_pga.text.strip())
@@ -120,16 +145,16 @@
                 
                 #self.overall_sem_csv = pd.merge(sem1,sem2, how='outer')
                 #self.overall_sem_csv.to_csv('matokeo.csv', index=False)
             elif 'invalid' in p.text:
                 print('Login Failed: invalid credentials'+ str(p.status_code))
             else:
                 print('invalid status code') 
-        except:
-            print('no internet connection')
+        # except:
+        #     print('no internet connection')
 
 
     
 
 
    
     def studentInfo(self,email, password):
```

## Comparing `RaphaelSomaDIT-2.5.dist-info/LICENSE` & `RaphaelSomaDIT-2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RaphaelSomaDIT-2.5.dist-info/LICENSE.txt` & `RaphaelSomaDIT-2.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `RaphaelSomaDIT-2.5.dist-info/RECORD` & `RaphaelSomaDIT-2.6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-RaphaelSomaDIT/__init__.py,sha256=Nuy6KQOji1eD2latwh470-mZ8FUH8iuYPeuEWe_Eeyo,10739
-RaphaelSomaDIT-2.5.dist-info/LICENSE,sha256=xUNz555ebRqtZIWdrSBf4yp9MZyKOBzw9AYqXOtPZy0,1087
-RaphaelSomaDIT-2.5.dist-info/LICENSE.txt,sha256=A8dltqeNi61ZJtJ_cWCn33uOzz86PQL8ikibobjG1k0,1066
-RaphaelSomaDIT-2.5.dist-info/METADATA,sha256=Rh6nLAfV2ue76K0h0WuqcR0GLoMtGpjlrKuDrJF-s9A,434
-RaphaelSomaDIT-2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-RaphaelSomaDIT-2.5.dist-info/top_level.txt,sha256=8O7Wzc2H8BV5QTK5pfxvbtSQPfa12VdD1NeFb8HMyT0,15
-RaphaelSomaDIT-2.5.dist-info/RECORD,,
+RaphaelSomaDIT/__init__.py,sha256=hiWlD0S87Yny38TXUu-BLRquGh7jE37u1AEeVSksHlY,11743
+RaphaelSomaDIT-2.6.dist-info/LICENSE,sha256=xUNz555ebRqtZIWdrSBf4yp9MZyKOBzw9AYqXOtPZy0,1087
+RaphaelSomaDIT-2.6.dist-info/LICENSE.txt,sha256=A8dltqeNi61ZJtJ_cWCn33uOzz86PQL8ikibobjG1k0,1066
+RaphaelSomaDIT-2.6.dist-info/METADATA,sha256=_dkv_8J8qgb_TWWlJAejatrKvxJsRjNowzsyO4WncBk,447
+RaphaelSomaDIT-2.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+RaphaelSomaDIT-2.6.dist-info/top_level.txt,sha256=8O7Wzc2H8BV5QTK5pfxvbtSQPfa12VdD1NeFb8HMyT0,15
+RaphaelSomaDIT-2.6.dist-info/RECORD,,
```

