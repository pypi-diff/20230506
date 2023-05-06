# Comparing `tmp/pagesnap-0.0.1.tar.gz` & `tmp/pagesnap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagesnap-0.0.1.tar", max compression
+gzip compressed data, was "pagesnap-0.0.2.tar", max compression
```

## Comparing `pagesnap-0.0.1.tar` & `pagesnap-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-05-05 14:57:36.376389 pagesnap-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-04 05:40:29.774704 pagesnap-0.0.1/pagesnap/__init__.py
--rw-r--r--   0        0        0     8927 2023-05-05 14:54:53.086106 pagesnap-0.0.1/pagesnap/pagesnap.py
--rw-r--r--   0        0        0      516 2023-05-05 14:53:20.742143 pagesnap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1249 2023-05-05 03:05:14.387126 pagesnap-0.0.1/README.md
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 pagesnap-0.0.1/setup.py
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 pagesnap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-05 14:57:36.376389 pagesnap-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-04 05:40:29.774704 pagesnap-0.0.2/pagesnap/__init__.py
+-rw-r--r--   0        0        0     8795 2023-05-06 15:15:58.959345 pagesnap-0.0.2/pagesnap/pagesnap.py
+-rw-r--r--   0        0        0      516 2023-05-06 15:08:57.297515 pagesnap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2199 2023-05-06 15:17:06.549349 pagesnap-0.0.2/README.md
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 pagesnap-0.0.2/setup.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 pagesnap-0.0.2/PKG-INFO
```

### Comparing `pagesnap-0.0.1/LICENSE` & `pagesnap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pagesnap-0.0.1/pagesnap/pagesnap.py` & `pagesnap-0.0.2/pagesnap/pagesnap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import asyncio
 from bs4 import BeautifulSoup
-from playwright.async_api import async_playwright
+from playwright.async_api import async_playwright, Page
 import base64
 
 resources = {}
 
 async def handle_response(response):
     if response and response.ok:
         print(f'请求成功 {response.url=}')
@@ -27,183 +27,190 @@
             url = response.url
             data = await response.text()
             resources[url] = {
                 'content_type': content_type,
                 'data': data
             }
 
-async def handle_request(route, request):
-    print(f'拦截请求 {route}')
-    request.on('response', handle_response)
-    await route.continue_()
-
 def resources_contains(part_of_url: str) -> str|None:
     for url in resources.keys():
         if part_of_url in url:
             return url
     return None
 
-async def save_as_single_file(url, output_filename):
-    """Save the page as a single file."""
-    async with async_playwright() as p:
-        browser = await p.chromium.launch()
-        page = await browser.new_page()
-        page.on('response', handle_response)
-        await page.goto(url)
-
-        # Wait for the 'networkidle' load state
-        await page.wait_for_load_state("networkidle")
-
-        content = await page.content()
-
-        await page.unroute('**/*', handle_request)
-
-        print(len(resources))
-
-        # embed images
-        for img in await page.query_selector_all('img[src]'):
-            src = await img.get_attribute('src')
-
-            if not src:
-                continue
-
-            if src.startswith('data:'):
-                continue
-
-            print('===============')
-            print(f'fetching {src}')
-
-            full_src =  resources_contains(src)
-            if full_src:
-                print('资源命中缓存')
-                content = content.replace(src, embed_resource(resources[full_src]['content_type'], resources[full_src]['data']))
-            else:
-                print('资源未命中，单独发起请求')
-                try:
-                    # response = await page.evaluate('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)
-                    response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)   
-                    await response.dispose()
-                except Exception as e:
-                    print(f'failed to fetch {src}')
-                    print(e)
-        
-        # embed css
-        for link in await page.query_selector_all('link[rel="stylesheet"]'):
-            href = await link.get_attribute('href')
-
-            if not href:
-                continue
-
-            print('===============')
-            print(f'fetching {href}')
-
-            full_href = resources_contains(href)
-            if full_href:
-                print('资源命中缓存')
-                continue
-
+async def hook_page(page: Page):
+    """Hook page to intercept requests and save resources"""
+    page.on('response', handle_response)
+
+async def page_snap(page: Page) -> str:
+    """Scrape page and embed resources"""
+    content = await page.content()
+
+    print(len(resources))
+
+    # embed images
+    for img in await page.query_selector_all('img[src]'):
+        src = await img.get_attribute('src')
+
+        if not src:
+            continue
+
+        if src.startswith('data:'):
+            continue
+
+        print('===============')
+        print(f'fetching {src}')
+
+        full_src =  resources_contains(src)
+        if full_src:
+            print('资源命中缓存')
+            content = content.replace(src, embed_resource(resources[full_src]['content_type'], resources[full_src]['data']))
+        else:
             print('资源未命中，单独发起请求')
             try:
                 # response = await page.evaluate('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)
-                response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
+                response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)   
                 await response.dispose()
-            except:
-                print(f'failed to fetch {href}')
-            # response = await page.evaluate('(href) => fetch(href).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
-
-        for link in await page.query_selector_all('link[as="style"]'):
-            href = await link.get_attribute('href')
-
-            if not href:
-                continue
-
-            print('===============')
-            print(f'fetching link[as="style"] {href}')
-
-            full_href = resources_contains(href)
-            if full_href:
-                print('资源命中缓存')
-                continue
+            except Exception as e:
+                print(f'failed to fetch {src}')
+                print(e)
+    
+    # embed css
+    for link in await page.query_selector_all('link[rel="stylesheet"]'):
+        href = await link.get_attribute('href')
+
+        if not href:
+            continue
+
+        print('===============')
+        print(f'fetching {href}')
+
+        full_href = resources_contains(href)
+        if full_href:
+            print('资源命中缓存')
+            continue
+
+        print('资源未命中，单独发起请求')
+        try:
+            # response = await page.evaluate('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)
+            response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
+            await response.dispose()
+        except:
+            print(f'failed to fetch {href}')
+        # response = await page.evaluate('(href) => fetch(href).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
+
+    for link in await page.query_selector_all('link[as="style"]'):
+        href = await link.get_attribute('href')
+
+        if not href:
+            continue
+
+        print('===============')
+        print(f'fetching link[as="style"] {href}')
+
+        full_href = resources_contains(href)
+        if full_href:
+            print('资源命中缓存')
+            continue
+
+        print('资源未命中，单独发起请求')
+        try:
+            # response = await page.evaluate('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)
+            response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
+            await response.dispose()
+        except:
+            print(f'failed to fetch {href}')
+        # response = await page.evaluate('(href) => fetch(href).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
+    
+    # Load the HTML with BeautifulSoup
+    soup = BeautifulSoup(content, "html.parser")
+
+    # Replace img tags with base64 embedded images
+    for img in soup.find_all("img", src=True):
+        src = resources_contains(img["src"])
+        if src:
+            resource = resources[src]
+            content_type = resource["content_type"]
+            data = resource["data"]
+            embedded_data = embed_resource(content_type, data)
+            img["src"] = embedded_data
+
+    def link_as_style_filter(tag):
+        return tag.name == "link" and tag.has_attr("as") and tag["as"] == "style"
+    
+    # Replace link tags with inline styles using resources
+    for link in soup.find_all(link_as_style_filter):
+        print('命中 tags with inline styles using resources')
+        href = resources_contains(link["href"])
+        if href:
+            resource = resources[href]
+            content_type = resource["content_type"]
+            data = resource["data"]
+            style_tag = soup.new_tag("style", type="text/css")
+            style_tag.string = data
+            link.replace_with(style_tag)
+    
+    # Replace link tags (CSS) with inline styles
+    for link in soup.find_all("link", rel="stylesheet", href=True):
+        href = resources_contains(link["href"])
+        if href:
+            resource = resources[href]
+            content_type = resource["content_type"]
+            data = resource["data"]
+            style_tag = soup.new_tag("style", type="text/css")
+            style_tag.string = data
+            link.replace_with(style_tag)
+    
+    # Remove all script tags
+    scripts = soup.find_all("script")
+    for script in scripts:
+        script.decompose()
+    
+    def link_script_filter(tag):
+        return tag.name == "link" and (tag.has_attr("as") and tag["as"] == "script") or (tag.has_attr('href') and tag['href'].endswith('.js'))
+    
+    # Remove the matching tags from the DOM
+    for tag in soup.find_all(link_script_filter):
+        tag.decompose()
+    
+    # Define a filter function for finding the desired tags
+    def ssr_dns_prefetch_filter(tag):
+        return tag.name == "link" and (tag.has_attr("data-n-head") and tag["data-n-head"] == "ssr") or (tag.has_attr("rel") and "dns-prefetch" in tag["rel"])
+
+    # Find all tags matching the filter
+    tags_to_remove = soup.find_all(ssr_dns_prefetch_filter)
+
+    # Remove the matching tags from the DOM
+    for tag in tags_to_remove:
+        tag.decompose()
 
-            print('资源未命中，单独发起请求')
-            try:
-                # response = await page.evaluate('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', src)
-                response = await page.evaluate_handle('(src) => fetch(src).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
-                await response.dispose()
-            except:
-                print(f'failed to fetch {href}')
-            # response = await page.evaluate('(href) => fetch(href).then(r => r.arrayBuffer()).then(r => btoa(String.fromCharCode(...new Uint8Array(r))))', href)
-        
-        # Load the HTML with BeautifulSoup
-        soup = BeautifulSoup(content, "html.parser")
+    # Get the modified HTML
+    return soup.prettify()
 
-        # Replace img tags with base64 embedded images
-        for img in soup.find_all("img", src=True):
-            src = resources_contains(img["src"])
-            if src:
-                resource = resources[src]
-                content_type = resource["content_type"]
-                data = resource["data"]
-                embedded_data = embed_resource(content_type, data)
-                img["src"] = embedded_data
+async def save_as_single_file(url, output_filename):
+    """Save the page as a single file."""
+    async with async_playwright() as p:
+        browser = await p.chromium.launch()
+        page = await browser.new_page()
 
-        def link_as_style_filter(tag):
-            return tag.name == "link" and tag.has_attr("as") and tag["as"] == "style"
-        
-        # Replace link tags with inline styles using resources
-        for link in soup.find_all(link_as_style_filter):
-            print('命中 tags with inline styles using resources')
-            href = resources_contains(link["href"])
-            if href:
-                resource = resources[href]
-                content_type = resource["content_type"]
-                data = resource["data"]
-                style_tag = soup.new_tag("style", type="text/css")
-                style_tag.string = data
-                link.replace_with(style_tag)
-        
-        # Replace link tags (CSS) with inline styles
-        for link in soup.find_all("link", rel="stylesheet", href=True):
-            href = resources_contains(link["href"])
-            if href:
-                resource = resources[href]
-                content_type = resource["content_type"]
-                data = resource["data"]
-                style_tag = soup.new_tag("style", type="text/css")
-                style_tag.string = data
-                link.replace_with(style_tag)
-        
-        # Remove all script tags
-        scripts = soup.find_all("script")
-        for script in scripts:
-            script.decompose()
+        # Step1: Hook page to intercept requests and save resources
+        #        note: you can also hook after goto, but you may miss some resources
+        await hook_page(page) 
         
-        def link_script_filter(tag):
-            return tag.name == "link" and (tag.has_attr("as") and tag["as"] == "script") or (tag.has_attr('href') and tag['href'].endswith('.js'))
-        
-        # Remove the matching tags from the DOM
-        for tag in soup.find_all(link_script_filter):
-            tag.decompose()
-        
-        # Define a filter function for finding the desired tags
-        def ssr_dns_prefetch_filter(tag):
-            return tag.name == "link" and (tag.has_attr("data-n-head") and tag["data-n-head"] == "ssr") or (tag.has_attr("rel") and "dns-prefetch" in tag["rel"])
-
-        # Find all tags matching the filter
-        tags_to_remove = soup.find_all(ssr_dns_prefetch_filter)
-
-        # Remove the matching tags from the DOM
-        for tag in tags_to_remove:
-            tag.decompose()
+        # Develop your code, doing your actions
+        await page.goto(url)
+        # It's better to wait for the page to be fully loaded
+        await page.wait_for_load_state("networkidle")
 
-        # Get the modified HTML
-        modified_html = soup.prettify()
+        # Step2: Get the page content
+        embedded_html = await page_snap(page)
 
+        # Then you can save it to a file
         with open(output_filename, 'w', encoding='utf-8') as f:
-            f.write(modified_html)
+            f.write(embedded_html)
 
         await browser.close()
 
 def embed_resource(content_type, data):
     """Embed the resource in the HTML page."""
     if type(data) == str:
         base64_data = data
```

### Comparing `pagesnap-0.0.1/pyproject.toml` & `pagesnap-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pagesnap"
-version = "0.0.1"
+version = "0.0.2"
 description = "Saving webpage in a single HTML file, based on playwright"
 authors = ["maxiee <maxieewong@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/maxiee/pagesnap"
 
 [tool.poetry.scripts]
```

### Comparing `pagesnap-0.0.1/setup.py` & `pagesnap-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['beautifulsoup4>=4.12.2,<5.0.0', 'playwright>=1.33.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pagesnap = pagesnap.pagesnap:main']}
 
 setup_kwargs = {
     'name': 'pagesnap',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Saving webpage in a single HTML file, based on playwright',
-    'long_description': '# PageSnap\n\n[中文文档](./README_zh.md)\n\nPageSnap is a tool that allows you to save web pages offline as single-page HTML files, preserving the original appearance of the web page as much as possible. It is developed using Python and Playwright, which means it can also save dynamic JavaScript web pages offline.\n\nThe advantage of using single-page HTML format is that users can conveniently open and browse the files with any W3C-compliant browser.\n\nAs a Python library, PageSnap can be easily added as a dependency to other projects. If your project uses Python and Playwright, simply import the PageSnap library to add offline-saving capabilities to your pages.\n\nNote: Currently, this project is still in the early stages of feature development and cannot be directly used as a library. The related APIs are still under development. You can keep an eye on the progress, or feel free to clone the project to try it out and share your thoughts.\n\n## Discussion\n\nIf you have any suggestions or improvements, please feel free to submit an issue or pull request. If you like this project, please give it a star.\n\nI am usually active on [Sina Weibo](https://www.weibo.com/u/1240212845) and welcome technical discussions there as well.',
+    'long_description': '# PageSnap\n\n[中文文档](./README_zh.md)\n\nPageSnap is a tool that allows you to save web pages offline as single-page HTML files, preserving the original appearance of the web page as much as possible. It is developed using Python and Playwright, which means it can also save dynamic JavaScript web pages offline.\n\nThe advantage of using single-page HTML format is that users can conveniently open and browse the files with any W3C-compliant browser.\n\nAs a Python library, PageSnap can be easily added as a dependency to other projects. If your project uses Python and Playwright, simply import the PageSnap library to add offline-saving capabilities to your pages.\n\nNote: Currently, this project is still in the early stages of feature development and cannot be directly used as a library. The related APIs are still under development. You can keep an eye on the progress, or feel free to clone the project to try it out and share your thoughts.\n\n## As a Library\n\nPageSnap provides an asyncio-based API. In your Playwright project, you can complete the offline saving of a page in just two steps. Here\'s an example code:\n\n```python\n# Step1: Hook page to intercept requests and save resources\n#        note: you can also hook after goto, but you may miss some resources\nawait hook_page(page) \n\n# Develop your code, doing your actions\nawait page.goto(url)\n# It\'s better to wait for the page to be fully loaded\nawait page.wait_for_load_state("networkidle")\n\n# Step2: Get the page content\nembedded_html = await page_snap(page)\n\n# Then you can save it to a file\nwith open(output_filename, \'w\', encoding=\'utf-8\') as f:\n    f.write(embedded_html)\n```\n\n## As a Command Line\n\nUse the following pip command to install:\n\n```\npip install pagesnap\n```\n\nInitialize Playwright:\n\n```\nplaywright install\n```\n\nStart using:\n\n```\npagesnap https://example.com/ test.html\n```\n\n## Discussion\n\nIf you have any suggestions or improvements, please feel free to submit an issue or pull request. If you like this project, please give it a star.\n\nI am usually active on [Sina Weibo](https://www.weibo.com/u/1240212845) and welcome technical discussions there as well.',
     'author': 'maxiee',
     'author_email': 'maxieewong@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/maxiee/pagesnap',
     'packages': packages,
     'package_data': package_data,
```

