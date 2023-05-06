# Comparing `tmp/ddreport-3.9.tar.gz` & `tmp/ddreport-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddreport-3.9.tar", last modified: Mon Mar 27 06:45:43 2023, max compression
+gzip compressed data, was "ddreport-4.0.tar", last modified: Sat May  6 08:11:59 2023, max compression
```

## Comparing `ddreport-3.9.tar` & `ddreport-4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 06:45:43.809931 ddreport-3.9/
--rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-3.9/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-03-27 06:45:43.809931 ddreport-3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-27 06:45:43.764128 ddreport-3.9/ddreport/
--rw-rw-rw-   0        0        0        0 2022-11-02 07:43:40.000000 ddreport-3.9/ddreport/__init__.py
--rw-rw-rw-   0        0        0     4250 2023-03-06 03:20:09.000000 ddreport-3.9/ddreport/api.py
--rw-rw-rw-   0        0        0     2715 2023-03-17 07:50:48.000000 ddreport-3.9/ddreport/db.py
--rw-rw-rw-   0        0        0      452 2022-11-18 10:03:26.000000 ddreport-3.9/ddreport/exceptd.py
--rw-rw-rw-   0        0        0     6592 2023-03-21 09:25:40.000000 ddreport-3.9/ddreport/func.py
--rw-rw-rw-   0        0        0     1175 2023-03-08 10:44:46.000000 ddreport-3.9/ddreport/orm.py
-drwxrwxrwx   0        0        0        0 2023-03-27 06:45:43.809931 ddreport-3.9/ddreport/template/
--rw-rw-rw-   0        0        0    16836 2023-03-16 06:50:35.000000 ddreport-3.9/ddreport/template/index.html
--rw-rw-rw-   0        0        0     8283 2023-03-20 08:22:25.000000 ddreport-3.9/ddreport/testReport.py
-drwxrwxrwx   0        0        0        0 2023-03-27 06:45:43.794921 ddreport-3.9/ddreport.egg-info/
--rw-rw-rw-   0        0        0      303 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-27 06:45:43.000000 ddreport-3.9/ddreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 06:45:43.809931 ddreport-3.9/setup.cfg
--rw-rw-rw-   0        0        0     1415 2023-03-27 06:44:19.000000 ddreport-3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.629799 ddreport-4.0/
+-rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      496 2023-05-06 08:11:59.629799 ddreport-4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.584015 ddreport-4.0/ddreport/
+-rw-rw-rw-   0        0        0        0 2022-11-02 07:43:40.000000 ddreport-4.0/ddreport/__init__.py
+-rw-rw-rw-   0        0        0     7107 2023-04-23 03:57:17.000000 ddreport-4.0/ddreport/api.py
+-rw-rw-rw-   0        0        0     2554 2023-04-27 06:51:09.000000 ddreport-4.0/ddreport/db.py
+-rw-rw-rw-   0        0        0      389 2023-04-22 12:51:35.000000 ddreport-4.0/ddreport/exceptd.py
+-rw-rw-rw-   0        0        0     3756 2023-04-27 12:20:47.000000 ddreport-4.0/ddreport/func.py
+-rw-rw-rw-   0        0        0     2016 2023-05-04 09:10:09.000000 ddreport-4.0/ddreport/handle.py
+-rw-rw-rw-   0        0        0     1175 2023-03-08 10:44:46.000000 ddreport-4.0/ddreport/orm.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.629799 ddreport-4.0/ddreport/template/
+-rw-rw-rw-   0        0        0    20482 2023-04-28 01:19:06.000000 ddreport-4.0/ddreport/template/index.html
+-rw-rw-rw-   0        0        0    11205 2023-04-24 09:38:45.000000 ddreport-4.0/ddreport/testReport.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.617744 ddreport-4.0/ddreport.egg-info/
+-rw-rw-rw-   0        0        0      496 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 08:11:59.629799 ddreport-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1621 2023-04-26 03:12:31.000000 ddreport-4.0/setup.py
```

### Comparing `ddreport-3.9/ddreport/db.py` & `ddreport-4.0/ddreport/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pymysql
 from sshtunnel import SSHTunnelForwarder
-from ddreport.exceptd import exceptContentObj
+
 
 
 class PytestMysql:
     def __init__(self, db, db_ssh=None):
         self.__SSH = False
         if db_ssh:
             self.__SSH = True
@@ -14,18 +14,14 @@
             if db_ssh.get('password'):
                 ssh_db_config['ssh_password'] = db_ssh.get('password')
             else:
                 ssh_db_config['ssh_pkey'] = db_ssh.get('pkey') or None
             self.__server = SSHTunnelForwarder(**ssh_db_config)
         self.__condb(db)
 
-    # 抛出异常
-    def __execptions(self, err):
-        exceptContentObj.raiseException({"错误详情": err})
-
     def __condb(self, db):
         try:
             data = {**db, **{'charset': 'utf8', 'cursorclass': pymysql.cursors.DictCursor, 'autocommit': True}}
             if self.__SSH is True:
                 self.__server.start()
                 data['host'], data['port'] = "127.0.0.1", self.__server.local_bind_port  # 重新赋值
             self.__conn = pymysql.connect(**data)
@@ -51,15 +47,15 @@
                     last_id = self.__cursor.lastrowid
                     self.__cursor.fetchall()
                     return last_id
                 else:
                     res = self.__cursor.fetchall()
                     return res or []
         else:
-            self.__execptions("Mysql Connection timed out: Connect failed")
+            raise ConnectionError("Mysql Connection timed out: Connect failed")
 
     def off(self):
         if self.__conn:
             self.__cursor.close()  # 关闭游标
             self.__conn.close()  # 关闭数据库连接
             if self.__SSH is True:
                 self.__server.close()
```

### Comparing `ddreport-3.9/ddreport/orm.py` & `ddreport-4.0/ddreport/orm.py`

 * *Files identical despite different names*

### Comparing `ddreport-3.9/ddreport/template/index.html` & `ddreport-4.0/ddreport/template/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -42,14 +42,26 @@
         margin-right: 40px;
     }
 
     .row-expand {
         background-color: #f5f5f5;
         padding: 10px;
     }
+
+    .block {
+  padding: 30px 0;
+  text-align: center;
+  border-right: solid 1px var(--el-border-color);
+  display: inline-block;
+  width: 49%;
+  box-sizing: border-box;
+  vertical-align: top;
+}
+
+
 </style>
 <body>
 <div id="app">
     <el-scrollbar height="100vh">
         <el-backtop target="#app  .el-scrollbar__wrap"></el-backtop>
         <h2 class="title">{{sourceData.title}}</h2>
         <el-row style="margin: 10px;">
@@ -138,22 +150,46 @@
                     </template>
                     <el-table :data="tableData" ref="refTable" border style="width: 100%">
                         <el-table-column type="expand">
                             <template #default="scope">
                                 <el-row class="row-expand">
                                     <el-col>
                                         <el-tabs type="border-card">
-                                            <el-tab-pane label=打印内容 v-if="scope.row.print">
+                                            <el-tab-pane label="打印内容" v-if="scope.row.print">
                                                 <pre v-html="scope.row.print"></pre>
                                             </el-tab-pane>
-                                            <el-tab-pane :label="scope.row.status==='skipped'? '跳过详情': '错误详情'" v-if="scope.row.error">
-                                                <pre v-html="scope.row.error"></pre>
+                                            <el-tab-pane label="请求内容" v-if="scope.row.query">
+                                                <pre v-html="scope.row.query"></pre>
+                                            </el-tab-pane>
+                                            <el-tab-pane label="响应头" v-if="scope.row.resp_headers">
+                                                <pre v-html="scope.row.resp_headers"></pre>
+                                            </el-tab-pane>
+                                            <el-tab-pane label="响应内容" v-if="scope.row.response">
+                                                <pre v-html="scope.row.response"></pre>
+                                            </el-tab-pane>
+                                            <el-tab-pane label="跳过说明" v-if="scope.row.skipped">
+                                                <pre v-html="scope.row.skipped"></pre>
+                                            </el-tab-pane>
+                                            <el-tab-pane v-if="scope.row.msg_dict">
+                                                <template #label>
+                                                    <span style="background-color: #f6c3c6; padding: 2px 5px; border-radius: 3px">失败详情</span>
+                                                </template>
+                                                <el-tag style="margin: 0 0 5px 20px" type="danger" v-if="scope.row.typed">{{f_errorInfo(scope.row.typed)}}</el-tag>
+                                                <pre v-html="scope.row.msg_dict"></pre>
                                             </el-tab-pane>
-                                            <el-tab-pane v-for="(value, item, i) in scope.row.info" :key="i" :label="item">
-                                                <pre v-html="value"></pre>
+                                            <el-tab-pane label="图片预览" v-if="scope.row.img">
+                                                <el-image :src="scope.row.img" fit="contain" alt="图片" @error="f_handleImageLoadError"></el-image>
+                                                <span v-if="imgErrorText" style="color: #9d300b">{{imgErrorText}}</span>
+                                            </el-tab-pane>
+                                            <el-tab-pane v-if="scope.row.status_code" disabled>
+                                                <template #label>
+                                                    <span class="custom-tabs-label">
+                                                        <el-tag :type="scope.row.status_code==200?'success':'danger'">{{scope.row.status_code}}</el-tag>
+                                                    </span>
+                                                </template>
                                             </el-tab-pane>
                                         </el-tabs>
                                     </el-col>
                                 </el-row>
                             </template>
                         </el-table-column>
                         <el-table-column label="序号" type="index" width="80px"></el-table-column>
@@ -171,50 +207,77 @@
                             </template>
                         </el-table-column>
                     </el-table>
                 </el-card>
             </el-col>
         </el-row>
         <!-- 展开/折叠/top按钮 -->
-        <div>
-            <el-affix position="bottom" :offset="200" style="right: 0; position: absolute; height: 0">
+        <div style="right: 40px; position: absolute; width:40px;">
+            <el-affix position="bottom" :offset="150" >
                 <el-row>
-                    <el-col style="margin-bottom: 20px">
+                    <el-col style="margin-bottom: 20px;">
                         <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(true)">+</el-button>
                     </el-col>
                     <el-col>
                         <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(false)">-</el-button>
                     </el-col>
                 </el-row>
             </el-affix>
-            <el-backtop target="#app .el-scrollbar__wrap"></el-backtop>
         </div>
+        <el-backtop target="#app .el-scrollbar__wrap"></el-backtop>
     </el-scrollbar>
 </div>
 <script>
     Object.assign(window, Vue)
     const App = {
         setup() {
             const tableData = ref([])
             const refTable = ref()
             const runRespTimeList = ref([])       // 折线图主数据（响应时间）
             const filterData = reactive({model_v: null, model_options: [], status_v: null,})
             const form = reactive({passed: 0, failed: 0, error: 0, skipped: 0})
             const sourceData = reactive(templateData)
+            const imgErrorText = ref('')
 
             const setupInfo = () => {
                 // 获取组列表
                 sourceData.cases.map(el => {
                     if (filterData.model_options.indexOf(el['model']) === -1) {
                         filterData.model_options.push(el['model'])
                     }
                 })
                 f_selectChange()
             }
 
+            const f_errorInfo = (typed) =>{
+                if(typed == 10){
+                    msg = "响应异常"
+                }else if (typed == 11){
+                    msg = "断言类型错误"
+                }else if (typed == 12){
+                    msg = "断言元素类型错误"
+                }else if (typed == 13){
+                    msg = "断言元素key错误"
+                }else if (typed == 14){
+                    msg = "响应内容不是json"
+                }else if (typed == 15){
+                    msg = "断言type字段值错误"
+                }else if (typed == 20){
+                    msg = "状态码错误"
+                }else if (typed == 21){
+                    msg = "text匹配失败"
+                }else if (typed == 22){
+                    msg = "json匹配失败"
+                }else {
+                    msg = null
+                }
+                return msg
+            }
+
+
             // 下拉框过滤
             const f_selectChange = () => {
                 tableData.value = sourceData.cases.filter(el => {
                     return (filterData.model_v || filterData.model_options).indexOf(el.model) !== -1 && (filterData.status_v || ["passed", "failed", "skipped", "error"]).indexOf(el.status) !== -1
                 })
                 form.passed = tableData.value.filter(el => {
                     return el.status === "passed"
@@ -242,14 +305,19 @@
             //展开或者折叠
             const f_toggleRowExpansion = (isExpansion) => {
                 tableData.value.map(el => {
                     refTable.value.toggleRowExpansion(el, isExpansion)
                 })
             }
 
+            // 图片加载失败
+            const f_handleImageLoadError = () => {
+                imgErrorText.value = "图片加载失败"
+            }
+
             // 饼图
             const chart1 = () => {
                 let seriesData = [
                     {name: "成功", value: form.passed},
                     {name: "失败", value: form.failed},
                     {name: "错误", value: form.error},
                     {name: "跳过", value: form.skipped}
@@ -350,16 +418,19 @@
 
             return {
                 sourceData,
                 form,
                 filterData,
                 tableData,
                 refTable,
+                imgErrorText,
                 f_selectChange,
                 f_toggleRowExpansion,
+                f_errorInfo,
+                f_handleImageLoadError,
             }
         },
     }
     const app = Vue.createApp(App)
     app.use(ElementPlus)
     app.mount("#app")
 </script>
```

#### html2text {}

```diff
@@ -25,16 +25,22 @@
 change="f_selectChange" placeholder="å¨é¨" style="width: 400px">
 key="item" :label="item" :value="item">  ç»æ:
 change="f_selectChange" placeholder="å¨é¨">
 span="4" style="text-align: right"> ç¨ä¾æ»æ°: {{tableData.length}}
 data="tableData" ref="refTable" border style="width: 100%">
 default="scope">
 
-label="scope.row.status==='skipped'? 'è·³è¿è¯¦æ': 'éè¯¯è¯¦æ'" v-
-if="scope.row.error">
 
-key="i" :label="item">
 
+
+
+label> å¤±è´¥è¯¦æ  {{f_errorInfo(scope.row.typed)}}
+
+src="scope.row.img" fit="contain" alt="å¾ç" @error="f_handleImageLoadError">
+{{imgErrorText}}
+label>
+type="scope.row.status_code==200?'success':'danger'">{{scope.row.status_code}}
 default="scope"> æå éè¯¯ å¤±è´¥ è·³è¿
-offset="200" style="right: 0; position: absolute; height: 0">
+offset="150" >
 click="f_toggleRowExpansion(true)">+
 click="f_toggleRowExpansion(false)">-
+
```

### Comparing `ddreport-3.9/setup.py` & `ddreport-4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,23 +31,23 @@
 
 #### 每次更新需要修改 version 字段
 
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ddreport",
-    version = "3.9",
-    keywords = ("pip", "pytest","testReport"),
+    version = "4.0",
+    keywords = ("pip", "pytest", "testReport"),
     description = "pytest测试报告",
-    long_description = "添加日期常用方法",
+    long_description = "1.增加正确的请求展示；2.增加用例运行时动态添加用例；3.添加测试报告中展示图片逻辑；4.api请求优化；5.异常信息优化；6.测试报告优化；7.数据对比采用deepdiff库",
     license = "MIT Licence",
 
     url = "https://gitee.com/duanliangcong/dlc_pytest-report.git",
     author = "duanliangcong",
     author_email = "137562703@qq.com",
     entry_points={"pytest11": ["test_report=ddreport.testReport"]},
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = ["requests", "jsonpath"],
+    install_requires = ["requests", "jsonpath", "deepdiff"],
 )
```

