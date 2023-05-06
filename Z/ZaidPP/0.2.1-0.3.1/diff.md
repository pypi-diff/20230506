# Comparing `tmp/ZaidPP-0.2.1.tar.gz` & `tmp/ZaidPP-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZaidPP-0.2.1.tar", last modified: Thu Apr 27 12:01:42 2023, max compression
+gzip compressed data, was "ZaidPP-0.3.1.tar", last modified: Sat May  6 17:31:00 2023, max compression
```

## Comparing `ZaidPP-0.2.1.tar` & `ZaidPP-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.763763 ZaidPP-0.2.1/
--rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      842 2023-04-27 12:01:42.763763 ZaidPP-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 12:01:42.764763 ZaidPP-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-04-27 11:59:03.000000 ZaidPP-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.728177 ZaidPP-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.743169 ZaidPP-0.2.1/src/ZaidPP/
--rw-rw-rw-   0        0        0    11990 2023-04-27 11:55:22.000000 ZaidPP-0.2.1/src/ZaidPP/ZaidPP.py
--rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.2.1/src/ZaidPP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.761761 ZaidPP-0.2.1/src/ZaidPP.egg-info/
--rw-rw-rw-   0        0        0      842 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.710495 ZaidPP-0.3.1/
+-rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      842 2023-05-06 17:31:00.709510 ZaidPP-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:31:00.711493 ZaidPP-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-06 17:21:29.000000 ZaidPP-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.669516 ZaidPP-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.684507 ZaidPP-0.3.1/src/ZaidPP/
+-rw-rw-rw-   0        0        0    13721 2023-05-06 17:28:03.000000 ZaidPP-0.3.1/src/ZaidPP/ZaidPP.py
+-rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.3.1/src/ZaidPP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.706511 ZaidPP-0.3.1/src/ZaidPP.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/top_level.txt
```

### Comparing `ZaidPP-0.2.1/PKG-INFO` & `ZaidPP-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.2.1
+Version: 0.3.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ZaidPP-0.2.1/setup.py` & `ZaidPP-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests\nuuid')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="ZaidPP",
-    version="0.2.1",
+    version="0.3.1",
     author="Zaid",
     author_email="www710700@gmail.com",
     description="• Scrape Instagram Profile and login Instagram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `ZaidPP-0.2.1/src/ZaidPP/ZaidPP.py` & `ZaidPP-0.3.1/src/ZaidPP/ZaidPP.py`

 * *Files 15% similar despite different names*

```diff
@@ -90,43 +90,44 @@
 		if req['message'] == 'The password you entered is incorrect. Please try again.':
 			return {"Instagram":"Good","Response ":True}
 		else:
 			return {"Instagram":"Bad","Response ":False} 
 			
 	def Token_Face(cookies: str) -> str:
 		try:
-			r=requests.Session()
-			r.headers.update({'referer': 'https://m.facebook.com/',})
-			data = r.get('https://business.facebook.com/business_locations', headers = {
-							'user-agent'                : 'Mozilla/5.0 (Linux; Android 8.1.0; MI 8 Build/OPM1.171019.011) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/69.0.3497.86 Mobile Safari/537.36', # don't change this user agent.
-							'referer'                   : 'https://www.facebook.com/',
-							'host'                      : 'business.facebook.com',
-							'origin'                    : 'https://business.facebook.com',
-							'upgrade-insecure-requests' : '1',
-							'accept-language'           : 'id-ID,id;q=0.9,en-US;q=0.8,en;q=0.7',
-							'cache-control'             : 'max-age=0',
-							'accept'                    : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8',
-							'content-type'              : 'text/html; charset=utf-8'
-						}, cookies = {
-							'cookie'                    : cookies
-						})
-						
-						
-					
-			find_token = re.search('(EAAG\w+)', data.text)
-			#print(find_token)
-			return '\n* Fail : maybe your cookie invalid !!' if (find_token is None) else find_token.group(1)
-			#print(results)
+		    r=requests.Session()
+		    r.headers.update({'referer': 'https://m.facebook.com/',})
+		    data = r.get('https://business.facebook.com/business_locations', headers = {
+		        'user-agent'                : 'Mozilla/5.0 (Linux; Android 8.1.0; MI 8 Build/OPM1.171019.011) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/69.0.3497.86 Mobile Safari/537.36', # don't change this user agent.
+		        'referer'                   : 'https://www.facebook.com/',
+		        'host'                      : 'business.facebook.com',
+		        'origin'                    : 'https://business.facebook.com',
+		        'upgrade-insecure-requests' : '1',
+		        'accept-language'           : 'id-ID,id;q=0.9,en-US;q=0.8,en;q=0.7',
+		        'cache-control'             : 'max-age=0',
+		        'accept'                    : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8',
+		        'content-type'              : 'text/html; charset=utf-8'
+		    }, cookies = {
+		        'cookie'                    : cookies
+		    })
+		    
+		    
+		
+		    find_token = re.search('(EAAG\w+)', data.text)
+		    results    = '\n* Fail : maybe your cookie invalid !!' if (find_token is None) else find_token.group(1)
 		except requests.exceptions.ConnectionError:
-			return '\n* Fail : no connection here !!'
+		    results    = '\n* Fail : no connection here !!'
 		except:
-		    return '\n* Fail : unknown errors, please try again !!'
-		    
+		    results    = '\n* Fail : unknown errors, please try again !!'
+		
+		return results
+
 
 	def Login_Face(user,pw):
+			
 			ses=requests.Session()
 			application_version = str(random.randint(111,555))+'.0.0.'+str(random.randrange(9,49))+str(random.randint(111,555))
 			application_version_code=str(random.randint(000000000,999999999))
 			fbs=random.choice(['com.facebook.adsmanager','com.facebook.lite','com.facebook.orca','com.facebook.katana','com.facebook.mlite'])
 			gtt=random.choice(['GT-I9190','KOT49H','GT-I9192','KOT49H','GT-I9300I','KTU84P','GT-I9300','IMM76D','GT-I9300','JSS15J','GT-I9301I','KOT4','GT-I9301I','KOT49H','GT-I9500','JDQ39','GT-I9500','LRX22C','GT-N5100','JZO54K','GT-N7100','KOT49H','GT-N8000','JZO54K','GT-N8000','KOT49H','GT-P3110','JZO54K','GT-P5100','IML74K','GT-P5100','JDQ','GT-P5100','JDQ39','GT-P5100','JZO54K','GT-P5110','JDQ39','GT-P5200','KOT49H','GT-P5210','KOT49H','GT-P5220','JDQ39','GT-S7390','JZO54K','SAMSUNG','SM-A500F','SAMSUNG','SM-G532F','SAMSUNG','SM-G920F','SAMSUNG','SM-G935F','SAMSUNG','SM-J320F','SAMSUNG','SM-J510FN','SAMSUNG','SM-N920S','SAMSUNG','SM-T280','SM-A500FU','MMB29M','SM-A500F','LRX22G','SM-A500F','MMB29M','SM-A500H','MMB29M','SM-G900F','KOT49H','SM-G920F','MMB29K','SM-G920F','NRD90M','SM-G930F','NRD90M','SM-G935F','MMB29K','SM-G935F','NRD90M','SM-G950F','NRD90M','SM-J320FN','LMY47V','SM-J320F','LMY4','SM-J320F','LMY47V','SM-J320H','LMY47V','SM-J320M','LMY47V','SM-J510FN','MMB29M','SM-J510FN','NMF2','SM-J510FN','NMF26X','SM-J510FN','NMF26X;','SM-J701F','NRD90M;','SM-T111','JDQ39','SM-T230','KOT49H','SM-T231','KOT49H','SM-T235','KOT4''SM-T310','KOT49H','SM-T311','KOT4','SM-T311','KOT49H','SM-T315','JDQ39','SM-T525','KOT49H','SM-T531','KOT49H','SM-T531','LRX22G','SM-T535','LRX22G','SM-T555','LRX22G','SM-T561','KTU84P','SM-T705','LRX22G','SM-T705','LRX22G','SM-T805','LRX22G','SM*T820','NRD90M','SPH-L720','KOT49H'])
 			gttt=random.choice(['GT-I9190','KOT49H','GT-I9192','KOT49H','GT-I9300I','KTU84P','GT-I9300','IMM76D','GT-I9300','JSS15J','GT-I9301I','KOT4','GT-I9301I','KOT49H','GT-I9500','JDQ39','GT-I9500','LRX22C','GT-N5100','JZO54K','GT-N7100','KOT49H','GT-N8000','JZO54K','GT-N8000','KOT49H','GT-P3110','JZO54K','GT-P5100','IML74K','GT-P5100','JDQ','GT-P5100','JDQ39','GT-P5100','JZO54K','GT-P5110','JDQ39','GT-P5200','KOT49H','GT-P5210','KOT49H','GT-P5220','JDQ39','GT-S7390','JZO54K','SAMSUNG','SM-A500F','SAMSUNG','SM-G532F','SAMSUNG','SM-G920F','SAMSUNG','SM-G935F','SAMSUNG','SM-J320F','SAMSUNG','SM-J510FN','SAMSUNG','SM-N920S','SAMSUNG','SM-T280','SM-A500FU','MMB29M','SM-A500F','LRX22G','SM-A500F','MMB29M','SM-A500H','MMB29M','SM-G900F','KOT49H','SM-G920F','MMB29K','SM-G920F','NRD90M','SM-G930F','NRD90M','SM-G935F','MMB29K','SM-G935F','NRD90M','SM-G950F','NRD90M','SM-J320FN','LMY47V','SM-J320F','LMY4','SM-J320F','LMY47V','SM-J320H','LMY47V','SM-J320M','LMY47V','SM-J510FN','MMB29M','SM-J510FN','NMF2','SM-J510FN','NMF26X','SM-J510FN','NMF26X;','SM-J701F','NRD90M;','SM-T111','JDQ39','SM-T230','KOT49H','SM-T231','KOT49H','SM-T235','KOT4''SM-T310','KOT49H','SM-T311','KOT4','SM-T311','KOT49H','SM-T315','JDQ39','SM-T525','KOT49H','SM-T531','KOT49H','SM-T531','LRX22G','SM-T535','LRX22G','SM-T555','LRX22G','SM-T561','KTU84P','SM-T705','LRX22G','SM-T705','LRX22G','SM-T805','LRX22G','SM*T820','NRD90M','SPH-L720','KOT49H'])
 			android_version=str(random.randrange(6,13))
@@ -163,8 +164,40 @@
 				"x-fb-connection-quality": "EXCELLENT",
 				"x-fb-friendly-name": "authenticate",
 				"accept-encoding": "gzip, deflate",
 				"x-fb-http-engine": "Liger"
 			}
 			rest = ses.post("https://b-api.facebook.com/method/auth.login", data=data, headers=head, allow_redirects=False).text
 			result = json.loads(rest)
-			return result
+			return result
+			
+
+	def info_insta(user):
+		he={
+'accept': '*/*',
+'accept-encoding': 'gzip, deflate, br',
+'accept-language': 'ar,en;q=0.9',
+'cookie': f'ig_did={uuid4}; datr=8J8TZD9P4GjWjawQJMcnRdV_; mid=ZBOf_gALAAGhvjQbR29aVENHIE4Z; ig_nrcb=1; csrftoken=5DoPPeHPd4nUej9JiwCdkvwwmbmkDWpy; ds_user_id=56985317140; dpr=1.25',
+'referer': f'https://www.instagram.com/{user}/?hl=ar',
+'sec-ch-prefers-color-scheme': 'dark',
+'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+'sec-ch-ua-full-version-list': '"Chromium";v="112.0.5615.138", "Google Chrome";v="112.0.5615.138", "Not:A-Brand";v="99.0.0.0"',
+'sec-ch-ua-mobile': '?0',
+'sec-ch-ua-platform': '"Windows"',
+'sec-ch-ua-platform-version': '"10.0.0"',
+'sec-fetch-dest': 'empty',
+'sec-fetch-mode': 'cors',
+'sec-fetch-site': 'same-origin',
+'user-agent': generate_user_agent(),
+'viewport-width': '1051',
+'x-asbd-id': '198387',
+'x-csrftoken': '5DoPPeHPd4nUej9JiwCdkvwwmbmkDWpy',
+'x-ig-app-id': '936619743392459',
+'x-ig-www-claim': '0',
+'x-requested-with': 'XMLHttpRequest',}
+
+		try:
+			rr = requests.get(f'https://www.instagram.com/api/v1/users/web_profile_info/?username={user}',headers=he).json();user=user;id = rr['data']['user']['id'];name=rr['data']['user']['full_name'];bio = rr['data']['user']['biography'];flos = rr['data']['user']['edge_followed_by']['count'];flog = rr['data']['user']['edge_follow']['count'];pr=rr['data']['user']['is_private'];re = requests.get(f"https://o7aa.pythonanywhere.com/?id={id}").json();da = re['date']
+			resp = {"user":user,"name":name,"id":id,"private":pr,"date":da,"following":flog,"followers":flos,"bio":bio}
+			return resp
+		except:
+			return {"status":"Error","Username":"Unavailable"}
```

### Comparing `ZaidPP-0.2.1/src/ZaidPP.egg-info/PKG-INFO` & `ZaidPP-0.3.1/src/ZaidPP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.2.1
+Version: 0.3.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

