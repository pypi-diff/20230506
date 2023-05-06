# Comparing `tmp/spacetool-1.0.2.tar.gz` & `tmp/spacetool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.2.tar", last modified: Tue Apr 25 08:53:42 2023, max compression
+gzip compressed data, was "spacetool-1.0.3.tar", last modified: Sat May  6 03:09:19 2023, max compression
```

## Comparing `spacetool-1.0.2.tar` & `spacetool-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.281538 spacetool-1.0.2/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.2/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-25 08:53:42.281413 spacetool-1.0.2/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.2/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-04-25 08:53:42.281584 spacetool-1.0.2/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2519 2023-04-25 08:53:13.000000 spacetool-1.0.2/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.280187 spacetool-1.0.2/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.2/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.2/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    50834 2023-04-25 05:52:01.000000 spacetool-1.0.2/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-25 08:53:42.281220 spacetool-1.0.2/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       60 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-04-25 08:53:42.000000 spacetool-1.0.2/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.615988 spacetool-1.0.3/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.3/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:09:19.615868 spacetool-1.0.3/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.3/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-06 03:09:19.616029 spacetool-1.0.3/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2519 2023-05-06 03:09:09.000000 spacetool-1.0.3/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.614715 spacetool-1.0.3/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.3/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.3/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    52059 2023-05-06 03:07:37.000000 spacetool-1.0.3/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.615661 spacetool-1.0.3/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       60 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.2/LICENSE` & `spacetool-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.2/setup.py` & `spacetool-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="spacetool",
-    version="1.0.2",
+    version="1.0.3",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
     install_requires=["requests", "cos-python-sdk-v5==1.9.23", "qcloud-python-sts==3.1.3"],
     python_requires=">=3.6,<3.11",
```

### Comparing `spacetool-1.0.2/spacetool/main_tool.py` & `spacetool-1.0.3/spacetool/main_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     上传停车场采集记录信息；
     """
     def __init__(self, name, code, host="http://127.0.0.1:8000/"):
         now = datetime.now().strftime("%m-%d-%Y:%H-%M-%S")
         self._log_file_name = f"./walk_{now}.log.txt"
         self.name = name               # 用户name
         self.code = code               # 用户code
-        self.uid = None                # 用户ID
+        # self.uid = None                # 用户ID
         self.authorization = None
         # self.temp_carparking_name = "carparking_name"
         # self.temp_unique_time_string = "unique_time_string"
         self.host = host               # api Domain
 
         # assert self.temp_carparking_name, "请携带正确的停车场名称"
         # assert self.host, "请携带api host"
@@ -120,37 +120,37 @@
 
     def check_code(self):
         # 用户校验
         res = requests_post(self.check_code_url, {"name": self.name, "code": self.code})
         assert res.status_code == 200, f"请求有错, errmsg【{res.reason}】"
         json_data = json.loads(res.text)
         assert json_data['code'] == 2000, f"请求有错, errmsg【{json_data['msg']}】"
-        self.uid = json_data['data']['uid']
+        # self.uid = json_data['data']['uid']
         return json_data['data']
 
     def update_code(self, new_code):
         # 用户更新code
         assert 4 <= len(new_code) <= 10, "请输入长度为4~10的新code"
         res = requests_post(self.update_code_url, {"name": self.name, "code": self.code, "new_code": new_code})
         assert res.status_code == 200, f"请求有错, errmsg【{res.reason}】"
         json_data = json.loads(res.text)
-        self.uid = json_data['data']['uid']
+        # self.uid = json_data['data']['uid']
         return json_data['data']
 
     def upload_car_parking_info(self, carparking_name, city="城市", district="区", address="地址", update=False):
         carparking_name = carparking_name.strip()
         if not carparking_name.endswith("停车场"):
             carparking_name = carparking_name + "停车场"
         res = requests_post(self.car_parking_serial_id_url, {
             "carparking_name": carparking_name,
             "city": city,
             "district": district,
             "address": address,
             "update": update,
-            "uid": self.uid
+            # "uid": self.uid
         })
         assert res.status_code == 200, f"请求有错, errmsg【{res.reason}】"
         json_data = json.loads(res.text)
         return json_data
 
     def get_car_parking_info(self, carparking_name):
         carparking_name = carparking_name.strip()
@@ -161,15 +161,15 @@
         json_data = json.loads(res.text)
         return json_data
 
     def upload_carparking_collection_record_info(self, carparking_serial, unique_time_string, other_data={}):
         payload = {
             "carparking_serial": carparking_serial,
             "unique_time_string": unique_time_string,
-            "uid": self.uid
+            # "uid": self.uid
         }
         payload.update(other_data)
         res = requests_post(self.collection_record_serial_id_url, payload)
         assert res.status_code == 200, f"请求有错, errmsg【{res.reason}】"
         json_data = json.loads(res.text)
         return json_data
 
@@ -233,14 +233,32 @@
                 "collection_record_serial": collection_record_serial,
                 "handle_type": handle_type,
                 "handle_path": handle_path,
                 "handle_status": False
             }
         return True
 
+    # def manual_walk_dir(self, origin_dir):
+    #     """
+    #     # 针对同一停车场的密集数据入库
+    #     # 读取文件路径，获取停车场名称和唯一时间戳
+    #     # walk记录运行到多少行, 跳过重复处理位置
+    #     # 格式：
+    #     # - 停车场名称
+    #     #     - video1_name.mp4
+    #     #     - video1_name.mp4
+    #     """
+    #     num = 0
+    #     for root, dirs, files in os.walk(origin_dir, topdown=False):
+    #         for file_name in files:
+    #             full_f_name = os.path.join(root, file_name)
+    #             if file_name.endswith("mp4"):
+    #                 carparking_name = full_f_name.split(os.path.sep)[-2]
+    #                 unique_time_string = file_name.split(".")[0]
+
     def walk_dir(self, origin_dir):
         """
         # 读取文件路径，获取停车场名称和唯一时间戳
         # walk记录运行到多少行, 跳过重复处理位置
 
         # 格式1:
         # - 追势自有格式
@@ -974,18 +992,26 @@
 import main_tool
 d = main_tool.DataTool(name="", code="", host="http://127.0.0.1:8000/")
 to_handle_dir = "/Users/leo/Documents/data/test数据格式样本/紫横家园东区"
 car_p_ser_path = d.walk_dir(to_handle_dir)
 res = d.handle_local()
 
 import main_tool
-d = main_tool.DataTool(name="", code="", host="http://127.0.0.1:8000/")
+d = main_tool.DataTool(name="", code="", host="")
 f = "/Users/leo/Downloads/追势数据4号盘.txt"
-res = d.walk_log_file(f)
-res2 = d.walk_log_and_upload_info(f)
+res = d.walk_log_file(f3)
+res2 = d.walk_log_and_upload_info(f3)
+
+f1 = "/Users/leo/Downloads/用所选项目新建的文件夹2/离线硬盘path地址/追势数据1号盘.txt"
+f2 = "/Users/leo/Downloads/用所选项目新建的文件夹2/离线硬盘path地址/追势数据2号盘.txt"
+f3 = "/Users/leo/Downloads/用所选项目新建的文件夹2/离线硬盘path地址/追势数据3号盘.txt"
+
+f1 = "/var/www/data/追势数据1号盘.txt"
+f2 = "/var/www/data/追势数据2号盘.txt"
+f3 = "/var/www/data/追势数据3号盘.txt"
 
 """
 
 
 """
 qcloud 测试
 if __name__ == "__main__":
```

