# Comparing `tmp/cnki_html2json-0.1.5.tar.gz` & `tmp/cnki_html2json-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.5.tar", last modified: Fri May  5 17:58:22 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.6.tar", last modified: Sat May  6 04:42:04 2023, max compression
```

## Comparing `cnki_html2json-0.1.5.tar` & `cnki_html2json-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:42:04.233306 cnki_html2json-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-06 04:42:04.233306 cnki_html2json-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:42:04.229306 cnki_html2json-0.1.6/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:42:04.233306 cnki_html2json-0.1.6/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 04:42:04.000000 cnki_html2json-0.1.6/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 04:42:04.233306 cnki_html2json-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:42:04.233306 cnki_html2json-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-06 04:41:51.000000 cnki_html2json-0.1.6/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.5/LICENSE` & `cnki_html2json-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.5/PKG-INFO` & `cnki_html2json-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
@@ -116,16 +116,15 @@
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
 |  | issue |  | 刊号 |
-| body_text |  |  |  |
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+| body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
 
 ## 开源协议
```

### Comparing `cnki_html2json-0.1.5/README.md` & `cnki_html2json-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
@@ -93,16 +93,15 @@
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
 |  | issue |  | 刊号 |
-| body_text |  |  |  |
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+| body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
 
 ## 开源协议
```

### Comparing `cnki_html2json-0.1.5/cnki_html2json/cli.py` & `cnki_html2json-0.1.6/cnki_html2json/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='start index, default is 1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='end index, default is None, which means download to the end')
     parser.add_argument('-m','--mode',type=str,default='raw',help='mode: raw(default)|structure|plain')
     parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='browser type: Chrome(default)|Firefox|Edge')
-    parser.add_argument('-save','--save_path',type=str,default='data',help='save path, default is <data> folder in the current directory')
+    parser.add_argument('-save','--save_path',type=str,default='data',help='save path, default is <dataset> folder in the current directory')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='waiting time for search, default is 120 seconds')
     parser.add_argument('-l','--log',action='store_true',help="whether to save log, specify this parameter to save log, no need to pass value")
     args = parser.parse_args()
     start_crawl(start_paper_index = args.start_paper_index,
                 end_paper_index = args.end_paper_index,
                 mode = args.mode,
                 save_path = args.save_path,
```

### Comparing `cnki_html2json-0.1.5/cnki_html2json/crawl.py` & `cnki_html2json-0.1.6/cnki_html2json/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
+from selenium.webdriver.support.wait import WebDriverWait
 import time
 import os
 import json
 import random
 import sys
 import math
 from loguru import logger
@@ -56,15 +57,19 @@
     except:
         logger.error('论文未提供html页面')
         return concat_content(metadata,{'body_text':None,'citation':None})
     
     else:
         handles = driver.window_handles
         driver.switch_to.window(handles[-1])
-        time.sleep(10)
+        # time.sleep(10)
+        # 将固定等待10s改为动态等待，直到页面加载完成
+        wait = WebDriverWait(driver, 15, 1)
+        wait.until(lambda driver: driver.execute_script('return document.readyState') == 'complete')
+        time.sleep(random.randint(1,5))
 
         # 调用判断验证码函数
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
@@ -94,15 +99,15 @@
             visible_page_elements = driver.find_elements(By.XPATH,'//div[@class="pages"]/a[position() >= 3 and position() <= last()-1]')
             visible_page_index = [int(i.text) for i in visible_page_elements]
 
         if start_page in visible_page_index:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{start_page}"]').click()
             time.sleep(3)
-            logger.info(f'已跳转到指定的第{start_page}页')
+            logger.info(f'已跳转到第 {start_page} 页')
             break
         
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
@@ -125,15 +130,15 @@
     else:
         save_path_files = [i for i in os.listdir(save_path) if i.endswith('.json')]
         if save_path_files and start_paper_index==1:
             cover_risk = input(f'{save_path}文件夹中已存在json文件, 覆盖请输入y, 不覆盖请输入n, 程序将退出, 请输入: ')
             if cover_risk == 'y':
                 logger.warning(f'新下载的文件将覆盖{save_path}文件夹里的文件')
             else:
-                sys.exit('程序已退出')
+                sys.exit()
     
     if log:
         if not os.path.exists(f'{save_path}/log'):
             os.mkdir(f'{save_path}/log')
             logger.info(f'已创建{save_path}/log文件夹')
 
         current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
@@ -174,15 +179,15 @@
     total_records_num = int(''.join(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[1]/em').text.split(',')))
     if end_paper_index:
         avaiable_records_num = min([total_records_num,end_paper_index,6000])
     else:
         avaiable_records_num = min([total_records_num,6000])
     
     need_download_num = avaiable_records_num-start_paper_index+1
-    logger.info(f'总文献数量 {total_records_num}; 可下载文献数 {avaiable_records_num}' )
+    logger.info(f'总文献数量 {total_records_num}; 可下载到第 {avaiable_records_num} 篇' )
     
     start_page = start_paper_index//papers_per_page+1
     
     # 总页数
     # total_page_num = int(driver.find_element(By.XPATH,'//*[@id="countPageDiv"]/span[2]').text.split('/')[1])
     # print(f'总页数{total_page_num}')
     
@@ -222,15 +227,15 @@
                 logger.error(f'fail {current_paper_index} {paper_content["metadata"]["title"]}')
             time.sleep(random.randint(3,5))
             current_paper_index += 1
         
             if current_paper_index == avaiable_records_num+1:
                 logger.info('下载完成')
                 driver.quit()
-                sys.exit('下载完成，程序已退出')
+                sys.exit()
                 
         logger.info(f'第 {current_page} 页下载完成')
         
         # 点击下一页
         driver.find_element(By.ID,'PageNext').click()
 
         time.sleep(5)
```

### Comparing `cnki_html2json-0.1.5/cnki_html2json/html2json.py` & `cnki_html2json-0.1.6/cnki_html2json/html2json.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class ExtractContent:
 
     def __init__(self,html_str:str) -> None:
         self.html_str = html_str
         self.error = False
 
-    def __process_html(self):
+    def _process_html(self):
         """处理原始html"""
         html_str = re.sub(r'<script.*?>.*?</script>','',self.html_str,flags=re.S)
         html_str = re.sub(r'<style.*?>.*?</style>','',html_str,flags=re.S)
 
         # remove image
         html_str = re.sub(r'<div class="area_img".*?</div>','',html_str,flags=re.S)
         try:
@@ -90,17 +90,20 @@
         text_content = ''
         for id in node_list:
             try:
                 node = self.body_tree.xpath(f'//p[@id="{id}"]')[0]
             except IndexError:
                 pass
             else:
-                node_str = html.tostring(node,encoding='unicode')
-                node_content = ''.join([i for i in re.findall(r'>(.*?)<', node_str) if i != '']) # type:ignore
-                text_content += node_content.strip()+'\n'
+                node_str = str(html.tostring(node,encoding='unicode'))
+                node_content_list = [i for i in re.findall(r'>(.*?)<', node_str) if i != '']
+
+                # 将正文中包含的[]转换为(),防止参考文献索引识别错误
+                node_content_list = [re.sub(r'\[(\d+(,\s*\d+)*)\]',r'(\1)',node) for node in node_content_list]
+                text_content += ''.join(node_content_list).strip()+'\n'
 
         # 获取参考文献索引  
         nested_ref_index = [eval(i) for i in re.findall(r'\[[\d,]+\]',text_content)]
         flat_ref_index = sorted(set([j for i in nested_ref_index for j in i]))
 
         # 获取节点所在段落的参考文献索引
         # ref_index_xpath_expression = '//p[' + ' or '.join([f'@id="{id}"' for id in node_list]) + ']/citation//a[@class="sup"]/text()'
@@ -167,15 +170,15 @@
 
     def extract(self,mode:str='raw',export_path=None):
         """将论文的html字符串转换为字典
         mode: 模式，structure|plain|raw，默认为raw
         export_path: 导出json文件的路径，默认为None，如果导出json文件，该参数必须指定
         """
         
-        self.__process_html()
+        self._process_html()
         if self.error:
             return {'body_text':None,'other':None}
         self._extract_node()
         if self.error:
             return {'body_text':None,'other':None}
         self._extract_reference()
```

### Comparing `cnki_html2json-0.1.5/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.6/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.5/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.6/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.5/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.6/cnki_html2json.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
+- `v0.1.5` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
   - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
@@ -116,16 +116,15 @@
 |  | orgs |  | 作者所属机构 |
 |  | abstract |  | 论文摘要 |
 |  | keywords |  | 论文关键词 |
 |  | funds |  | 基金资助 |
 |  | class_num |  | 分类号 |
 |  | source |  | 来源期刊 |
 |  | issue |  | 刊号 |
-| body_text |  |  |  |
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+| body_text | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
 |  | 2.xxx | 2.1xxx |  |
 |  | ...| ... |  |
 | other | 作者贡献声明 |  |  |
 |  | 利益冲突声明 |  |  |
 |  | 参考文献 |  |  |
 
 ## 开源协议
```

### Comparing `cnki_html2json-0.1.5/setup.py` & `cnki_html2json-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.5",
+    version="0.1.6",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.5/tests/test_html2json.py` & `cnki_html2json-0.1.6/tests/test_html2json.py`

 * *Files identical despite different names*

