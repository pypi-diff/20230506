# Comparing `tmp/cos-python-sdk-v5-1.9.8.tar.gz` & `tmp/cos-python-sdk-v5-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cos-python-sdk-v5-1.9.8.tar", last modified: Thu Aug 19 12:14:23 2021, max compression
+gzip compressed data, was "dist/cos-python-sdk-v5-1.9.9.tar", last modified: Tue Oct 12 07:41:40 2021, max compression
```

## Comparing `cos-python-sdk-v5-1.9.8.tar` & `cos-python-sdk-v5-1.9.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 tiedu     (1000) tiedu     (1000)        0 2021-08-19 12:14:23.000000 cos-python-sdk-v5-1.9.8/
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       40 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/MANIFEST.in
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)      714 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/setup.py
-drwxrwxr-x   0 tiedu     (1000) tiedu     (1000)        0 2021-08-19 12:14:23.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     2947 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_exception.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)    22447 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/tce_demo.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     5646 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_auth.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)   171873 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_client.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     8848 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/resumable_downloader.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     4284 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/select_event_stream.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     3024 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_threadpool.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       24 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/version.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     3617 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/demo.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)    16825 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_comm.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)      440 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/__init__.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     3011 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/streambody.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     7627 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/cos_encryption_client.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)    16051 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/crypto.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     1604 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/qcloud_cos/xml2dict.py
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       47 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/requirements.txt
-drwxrwxr-x   0 tiedu     (1000) tiedu     (1000)        0 2021-08-19 12:14:22.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)        1 2021-08-19 12:14:21.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/dependency_links.txt
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       48 2021-08-19 12:14:21.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/requires.txt
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       11 2021-08-19 12:14:21.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/top_level.txt
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     1473 2021-08-19 12:14:21.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/PKG-INFO
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)      654 2021-08-19 12:14:21.000000 cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/SOURCES.txt
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)    47403 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/CHANGELOG.md
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)      951 2021-08-19 12:10:36.000000 cos-python-sdk-v5-1.9.8/README.rst
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)     1473 2021-08-19 12:14:23.000000 cos-python-sdk-v5-1.9.8/PKG-INFO
--rw-rw-r--   0 tiedu     (1000) tiedu     (1000)       38 2021-08-19 12:14:23.000000 cos-python-sdk-v5-1.9.8/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-12 07:41:40.000000 cos-python-sdk-v5-1.9.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-12 07:41:40.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2021-10-12 07:41:39.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-10-12 07:41:39.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-10-12 07:41:39.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2021-10-12 07:41:39.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2021-10-12 07:41:39.000000 cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2021-10-12 07:41:40.000000 cos-python-sdk-v5-1.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-10-12 07:41:40.000000 cos-python-sdk-v5-1.9.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-12 07:41:40.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4284 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/select_event_stream.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2947 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3024 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_threadpool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199012 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8848 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/resumable_downloader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22447 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/tce_demo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17639 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_comm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6513 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16051 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7627 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/cos_encryption_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3011 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/streambody.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      440 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1604 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/xml2dict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3617 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/qcloud_cos/demo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      966 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47403 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2021-10-12 07:38:42.000000 cos-python-sdk-v5-1.9.9/setup.py
```

### Comparing `cos-python-sdk-v5-1.9.8/setup.py` & `cos-python-sdk-v5-1.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def long_description():
     with io.open('README.rst', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='cos-python-sdk-v5',
-    version='1.9.8',
+    version='1.9.9',
     url='https://www.qcloud.com/',
     license='MIT',
     author='tiedu, lewzylu, channingliu',
     author_email='dutie123@qq.com',
     description='cos-python-sdk-v5',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_exception.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_exception.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/tce_demo.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/tce_demo.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_auth.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,33 +32,57 @@
         if str.lower(i) in valid_headers or str.lower(i[0]) == "x":
             headers[i] = data[i]
     return headers
 
 
 class CosS3Auth(AuthBase):
 
-    def __init__(self, conf, key=None, params={}, expire=10000):
+    def __init__(self, conf, key=None, params={}, expire=10000, sign_host=None):
         self._secret_id = conf._secret_id
         self._secret_key = conf._secret_key
         self._anonymous = conf._anonymous
         self._expire = expire
         self._params = params
+
+        # 如果API指定了是否签名host，则以具体API为准，如果未指定则以配置为准
+        if sign_host is not None:
+            self._sign_host = bool(sign_host)
+        else:
+            self._sign_host = conf._sign_host
+
         if key:
             key = to_unicode(key)
             if key[0] == u'/':
                 self._path = key
             else:
                 self._path = u'/' + key
         else:
             self._path = u'/'
 
     def __call__(self, r):
         path = self._path
         uri_params = self._params
         headers = filter_headers(r.headers)
+
+        # 如果headers中不包含host头域，则从url中提取host，并且加入签名计算
+        if self._sign_host:
+
+            # 判断headers中是否包含host头域
+            contain_host = False
+            for i in headers:
+                if str.lower(i) == "host":  # 兼容host/Host/HOST等
+                    contain_host = True
+                    break
+
+            # 从url中提取host
+            if not contain_host:
+                url_parsed = urlparse(r.url)
+                if url_parsed.hostname is not None:
+                    headers["host"] = url_parsed.hostname
+
         # reserved keywords in headers urlencode are -_.~, notice that / should be encoded and space should not be encoded to plus sign(+)
         headers = dict([(quote(to_bytes(to_str(k)), '-_.~').lower(), quote(to_bytes(to_str(v)), '-_.~')) for k, v in
                         headers.items()])  # headers中的key转换为小写，value进行encode
         uri_params = dict([(quote(to_bytes(to_str(k)), '-_.~').lower(), quote(to_bytes(to_str(v)), '-_.~')) for k, v in
                            uri_params.items()])
         format_str = u"{method}\n{host}\n{params}\n{headers}\n".format(
             method=r.method.lower(),
```

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_client.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class CosConfig(object):
     """config类，保存用户相关信息"""
 
     def __init__(self, Appid=None, Region=None, SecretId=None, SecretKey=None, Token=None, Scheme=None, Timeout=None,
                  Access_id=None, Access_key=None, Secret_id=None, Secret_key=None, Endpoint=None, IP=None, Port=None,
                  Anonymous=None, UA=None, Proxies=None, Domain=None, ServiceDomain=None, PoolConnections=10,
-                 PoolMaxSize=10, AllowRedirects=False):
+                 PoolMaxSize=10, AllowRedirects=False, SignHost=True, EndpointCi=None):
         """初始化，保存用户的信息
 
         :param Appid(string): 用户APPID.
         :param Region(string): 地域信息.
         :param SecretId(string): 秘钥SecretId.
         :param SecretKey(string): 秘钥SecretKey.
         :param Token(string): 临时秘钥使用的token.
@@ -60,39 +60,45 @@
         :param UA(string):  使用自定义的UA来访问COS
         :param Proxies(dict):  使用代理来访问COS
         :param Domain(string):  使用自定义的域名来访问COS
         :param ServiceDomain(string):  使用自定义的域名来访问cos service
         :param PoolConnections(int):  连接池个数
         :param PoolMaxSize(int):      连接池中最大连接数
         :param AllowRedirects(bool):  是否重定向
+        :param SignHost(bool):  是否将host算入签名
+        :param EndpointCi(string):  ci的endpoint
         """
         self._appid = to_unicode(Appid)
         self._token = to_unicode(Token)
         self._timeout = Timeout
         self._region = Region
         self._endpoint = Endpoint
+        self._endpoint_ci = EndpointCi
         self._ip = to_unicode(IP)
         self._port = Port
         self._anonymous = Anonymous
         self._ua = UA
         self._proxies = Proxies
         self._domain = Domain
         self._service_domain = ServiceDomain
         self._pool_connections = PoolConnections
         self._pool_maxsize = PoolMaxSize
         self._allow_redirects = AllowRedirects
+        self._sign_host = SignHost
 
         if self._domain is None:
             self._endpoint = format_endpoint(Endpoint, Region)
         if Scheme is None:
             Scheme = u'https'
         Scheme = to_unicode(Scheme)
         if (Scheme != u'http' and Scheme != u'https'):
             raise CosClientError('Scheme can be only set to http/https')
         self._scheme = Scheme
+        # 格式化ci的endpoint 不支持自定义域名的
+        self._endpoint_ci = format_endpoint(EndpointCi, Region, u'ci.')
 
         # 兼容(SecretId,SecretKey)以及(AccessId,AccessKey)
         if (SecretId and SecretKey):
             self._secret_id = to_unicode(SecretId)
             self._secret_key = to_unicode(SecretKey)
         elif (Secret_id and Secret_key):
             self._secret_id = to_unicode(Secret_id)
@@ -197,23 +203,24 @@
         else:
             self._session = session
 
     def get_conf(self):
         """获取配置"""
         return self._conf
 
-    def get_auth(self, Method, Bucket, Key, Expired=300, Headers={}, Params={}):
+    def get_auth(self, Method, Bucket, Key, Expired=300, Headers={}, Params={}, SignHost=None):
         """获取签名
 
         :param Method(string): http method,如'PUT','GET'.
         :param Bucket(string): 存储桶名称.
         :param Key(string): 请求COS的路径.
         :param Expired(int): 签名有效时间,单位为s.
         :param headers(dict): 签名中的http headers.
         :param params(dict): 签名中的http params.
+        :param SignHost(bool): 是否将host算入签名.
         :return (string): 计算出的V5签名.
 
         .. code-block:: python
 
             config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
             client = CosS3Client(config)
             # 获取上传请求的签名
@@ -225,15 +232,15 @@
                     Headers={'header1': 'value1'},
                     Params={'param1': 'value1'}
                 )
             print (auth_string)
         """
         url = self._conf.uri(bucket=Bucket, path=Key)
         r = Request(Method, url, headers=Headers, params=Params)
-        auth = CosS3Auth(self._conf, Key, Params, Expired)
+        auth = CosS3Auth(self._conf, Key, Params, Expired, SignHost)
         return auth(r).headers['Authorization']
 
     def send_request(self, method, url, bucket, timeout=30, cos_request=True, **kwargs):
         """封装request库发起http请求"""
         if self._conf._timeout is not None:  # 用户自定义超时时间
             timeout = self._conf._timeout
         if self._conf._ua is not None:
@@ -487,65 +494,67 @@
             params=params,
             headers=headers)
 
         data = xml_to_dict(rt.content)
 
         return data
 
-    def get_presigned_url(self, Bucket, Key, Method, Expired=300, Params={}, Headers={}):
+    def get_presigned_url(self, Bucket, Key, Method, Expired=300, Params={}, Headers={}, SignHost=None):
         """生成预签名的url
 
         :param Bucket(string): 存储桶名称.
         :param Key(string): COS路径.
         :param Method(string): HTTP请求的方法, 'PUT'|'POST'|'GET'|'DELETE'|'HEAD'
         :param Expired(int): 签名过期时间.
         :param Params(dict): 签入签名的参数
         :param Headers(dict): 签入签名的头部
+        :param SignHost(bool): 是否将host算入签名.
         :return(string): 预先签名的URL.
 
         .. code-block:: python
 
             config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
             client = CosS3Client(config)
             # 获取预签名链接
             response = client.get_presigned_url(
                 Bucket='bucket',
                 Key='test.txt',
                 Method='PUT'
             )
         """
         url = self._conf.uri(bucket=Bucket, path=Key)
-        sign = self.get_auth(Method=Method, Bucket=Bucket, Key=Key, Expired=Expired, Headers=Headers, Params=Params)
+        sign = self.get_auth(Method=Method, Bucket=Bucket, Key=Key, Expired=Expired, Headers=Headers, Params=Params, SignHost=SignHost)
         sign = urlencode(dict([item.split('=', 1) for item in sign.split('&')]))
         url = url + '?' + sign
         if Params:
             url = url + '&' + urlencode(Params)
         return url
 
-    def get_presigned_download_url(self, Bucket, Key, Expired=300, Params={}, Headers={}):
+    def get_presigned_download_url(self, Bucket, Key, Expired=300, Params={}, Headers={}, SignHost=None):
         """生成预签名的下载url
 
         :param Bucket(string): 存储桶名称.
         :param Key(string): COS路径.
         :param Expired(int): 签名过期时间.
         :param Params(dict): 签入签名的参数
         :param Headers(dict): 签入签名的头部
+        :param SignHost(bool): 是否将host算入签名.
         :return(string): 预先签名的下载URL.
 
         .. code-block:: python
 
             config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
             client = CosS3Client(config)
             # 获取预签名文件下载链接
             response = client.get_presigned_download_url(
                 Bucket='bucket',
                 Key='test.txt'
             )
         """
-        return self.get_presigned_url(Bucket, Key, 'GET', Expired, Params, Headers)
+        return self.get_presigned_url(Bucket, Key, 'GET', Expired, Params, Headers, SignHost)
 
     def get_object_url(self, Bucket, Key):
         """生成对象访问的url
 
         :param Bucket(string): 存储桶名称.
         :param Key(string): COS路径.
         :return(string): 对象访问的URL.
@@ -4362,10 +4371,677 @@
             params=params,
             headers=headers)
 
         response = dict(**rt.headers)
         data = xml_to_dict(rt.content)
         return response, data
 
+    def ci_auditing_submit_common(self, Bucket, Key, DetectType, Type, Url=None, BizType=None, Conf={}, Input=None, **kwargs):
+        """通用提交审核任务接口 https://cloud.tencent.com/document/product/460/46427
+
+        :param Bucket(string): 存储桶名称.
+        :param Key(string): COS路径.
+        :param DetectType(int): 内容识别标志,位计算 1:porn, 2:terrorist, 4:politics, 8:ads
+        :param Type(string): 审核类型，video:视频，text：文本，audio：音频，docment：文档。
+        :param Url(string): Url, 支持非cos上的文件
+        :param Conf(dic): 审核的个性化配置
+        :param Input(dic): Input的个性化配置，dict类型，可跟restful api对应查询
+        :param BizType(string): 审核策略的唯一标识，由后台自动生成，在控制台中对应为Biztype值.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 下载成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 识别cos上的视频
+            response = client.ci_auditing_submit_common(
+                Bucket='bucket',
+                DetectType=CiDetectType.PORN | CiDetectType.POLITICS,
+                Key='test.mp4',
+                Type='video'
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        detect_type = CiDetectType.get_detect_type_str(DetectType)
+        params = format_values(params)
+
+        Conf['DetectType'] = detect_type
+        request = {
+            'Input': {},
+            'Conf': Conf
+        }
+        if BizType:
+            request['Conf']['BizType'] = BizType
+
+        if Key:
+            request['Input']['Object'] = Key
+        if Url:
+            request['Input']['Url'] = Url
+
+        if Input:
+            request['Input'] = Input
+
+        xml_request = format_xml(data=request, root='Request')
+        headers['Content-Type'] = 'application/xml'
+
+        path = Type + '/auditing'
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        logger.info("ci auditing {type} job submit, url=:{url} ,headers=:{headers}, params=:{params}, ci_endpoint=:{ci_endpoint}".format(
+            type=Type,
+            url=url,
+            headers=headers,
+            params=params,
+            ci_endpoint=self._conf._endpoint_ci))
+        rt = self.send_request(
+            method='POST',
+            url=url,
+            bucket=Bucket,
+            data=xml_request,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+
+        data = xml_to_dict(rt.content)
+
+        return data
+
+    def ci_auditing_query_common(self, Bucket, Type, JobID, **kwargs):
+        """通用查询审核任务接口 https://cloud.tencent.com/document/product/460/46926
+
+        :param Bucket(string): 存储桶名称.
+        :param Type(string): 审核类型，video:视频，text：文本，audio：音频，docment：文档。
+        :param JobID(string): 任务id.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 下载成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询视频审核返回的结果
+            response = client.ci_auditing_video_query(
+                Bucket='bucket',
+                JobID='v11122zxxxazzz',
+                Type='video'
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        params = format_values(params)
+
+        path = Type + '/auditing/' + JobID
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        logger.info("query ci auditing {type} result, url=:{url} ,headers=:{headers}, params=:{params}".format(
+            type=Type,
+            url=url,
+            headers=headers,
+            params=params))
+        rt = self.send_request(
+            method='GET',
+            url=url,
+            bucket=Bucket,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+
+        data = xml_to_dict(rt.content)
+
+        return data
+
+    def ci_auditing_video_submit(self, Bucket, Key, DetectType, Url=None, Callback=None, CallbackVersion='Simple', DetectContent=0, Mode='Interval', Count=100, TimeInterval=1.0,
+                                 BizType=None, **kwargs):
+        """提交video审核任务接口 https://cloud.tencent.com/document/product/460/46427
+
+        :param Bucket(string): 存储桶名称.
+        :param Key(string): COS路径.
+        :param Url(string): 支持直接传非cos上url过来审核
+        :param DetectType(int): 内容识别标志,位计算 1:porn, 2:terrorist, 4:politics, 8:ads
+        :param Callback(string): 回调地址，以http://或者https://开头的地址。
+        :param CallbackVersion(string): 回调内容的结构，有效值：Simple（回调内容包含基本信息）、Detail（回调内容包含详细信息）。默认为 Simple。
+        :param DetectContent(int): 用于指定是否审核视频声音，当值为0时：表示只审核视频画面截图；值为1时：表示同时审核视频画面截图和视频声音。默认值为0。
+        :param Mode(string): 截帧模式。Interval 表示间隔模式；Average 表示平均模式；Fps 表示固定帧率模式。
+                            Interval 模式：TimeInterval，Count 参数生效。当设置 Count，未设置 TimeInterval 时，表示截取所有帧，共 Count 张图片。
+                            Average 模式：Count 参数生效。表示整个视频，按平均间隔截取共 Count 张图片。
+                            Fps 模式：TimeInterval 表示每秒截取多少帧，Count 表示共截取多少帧。
+        :param Count(int): 视频截帧数量，范围为(0, 10000]。
+        :param TimeInterval(int): 视频截帧频率，范围为(0, 60]，单位为秒，支持 float 格式，执行精度精确到毫秒。
+        :param BizType(string): 审核策略的唯一标识，由后台自动生成，在控制台中对应为Biztype值.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 任务提交成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 识别cos上的视频
+            response = client.ci_auditing_video_submit(
+                Bucket='bucket',
+                DetectType=CiDetectType.PORN | CiDetectType.POLITICS,
+                Key='test.mp4'
+            )
+            print response
+        """
+
+        conf = {
+            'Snapshot': {
+                'Mode': Mode,
+                'TimeInterval': TimeInterval,
+                'Count': Count,
+            },
+            'DetectContent': DetectContent
+        }
+
+        if Callback:
+            conf['Callback'] = Callback
+
+        if CallbackVersion:
+            conf['CallbackVersion'] = CallbackVersion
+
+        return self.ci_auditing_submit_common(
+            Bucket=Bucket,
+            Key=Key,
+            Type='video',
+            BizType=BizType,
+            Conf=conf,
+            Url=Url,
+            DetectType=DetectType,
+            **kwargs
+        )
+
+    def ci_auditing_video_query(self, Bucket, JobID, **kwargs):
+        """查询video审核任务接口 https://cloud.tencent.com/document/product/460/46926
+
+        :param Bucket(string): 存储桶名称.
+        :param JobID(string): 任务id.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询视频审核返回的结果
+            response = client.ci_auditing_video_query(
+                Bucket='bucket',
+                JobID='v11122zxxxazzz'
+            )
+            print response
+        """
+
+        return self.ci_auditing_query_common(
+            Bucket=Bucket,
+            JobID=JobID,
+            Type='video',
+            **kwargs
+        )
+
+    def ci_auditing_audio_submit(self, Bucket, Key, DetectType, Url=None, Callback=None, CallbackVersion='Simple', BizType=None, **kwargs):
+        """提交音频审核任务接口 https://cloud.tencent.com/document/product/460/53395
+
+        :param Bucket(string): 存储桶名称.
+        :param Key(string): COS路径.
+        :param Url(string): 支持直接传非cos上url过来审核
+        :param DetectType(int): 内容识别标志,位计算 1:porn, 2:terrorist, 4:politics, 8:ads
+        :param Callback(string): 回调地址，以http://或者https://开头的地址。
+        :param CallbackVersion(string): 回调内容的结构，有效值：Simple（回调内容包含基本信息）、Detail（回调内容包含详细信息）。默认为 Simple。
+        :param BizType(string): 审核策略的唯一标识，由后台自动生成，在控制台中对应为Biztype值.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 任务提交成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 识别cos上的音频
+            response = client.ci_auditing_audio_submit(
+                Bucket='bucket',
+                DetectType=CiDetectType.PORN | CiDetectType.POLITICS,
+                Key='test.mp3'
+            )
+            print response
+        """
+
+        conf = {
+        }
+
+        if Callback:
+            conf['Callback'] = Callback
+
+        if CallbackVersion:
+            conf['CallbackVersion'] = CallbackVersion
+
+        return self.ci_auditing_submit_common(
+            Bucket=Bucket,
+            Key=Key,
+            Type='audio',
+            BizType=BizType,
+            Conf=conf,
+            Url=Url,
+            DetectType=DetectType,
+            **kwargs
+        )
+
+    def ci_auditing_audio_query(self, Bucket, JobID, **kwargs):
+        """查询音频审核任务接口 https://cloud.tencent.com/document/product/460/53396
+
+        :param Bucket(string): 存储桶名称.
+        :param JobID(string): 任务id.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询视频审核返回的结果
+            response = client.ci_auditing_audio_query(
+                Bucket='bucket',
+                JobID='v11122zxxxazzz'
+            )
+            print response
+        """
+
+        return self.ci_auditing_query_common(
+            Bucket=Bucket,
+            JobID=JobID,
+            Type='audio',
+            **kwargs
+        )
+
+    def ci_auditing_text_submit(self, Bucket, Key, DetectType, Content=None, Callback=None,  BizType=None, **kwargs):
+        """提交文本审核任务接口 https://cloud.tencent.com/document/product/460/56285
+
+        :param Bucket(string): 存储桶名称.
+        :param Key(string): COS路径.
+        :param Content(string): 当传入的内容为纯文本信息，原文长度不能超过10000个 utf8 编码字符。若超出长度限制，接口将会报错。
+        :param DetectType(int): 内容识别标志,位计算 1:porn, 2:terrorist, 4:politics, 8:ads
+        :param Callback(string): 回调地址，以http://或者https://开头的地址。
+        :param BizType(string): 审核策略的唯一标识，由后台自动生成，在控制台中对应为Biztype值.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 任务提交成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 识别cos上的文本
+            response = client.ci_auditing_text_submit(
+                Bucket='bucket',
+                DetectType=CiDetectType.PORN | CiDetectType.POLITICS,
+                Key='test.txt'
+            )
+            print response
+        """
+
+        Input = {}
+        if Key:
+            Input['Object'] = Key
+        if Content:
+            Input['Content'] = base64.b64encode(Content).decode('UTF-8')
+
+        conf = {
+        }
+
+        if Callback:
+            conf['Callback'] = Callback
+
+        return self.ci_auditing_submit_common(
+            Bucket=Bucket,
+            Key=Key,
+            Type='text',
+            BizType=BizType,
+            Conf=conf,
+            DetectType=DetectType,
+            Input=Input,
+            **kwargs
+        )
+
+    def ci_auditing_text_query(self, Bucket, JobID, **kwargs):
+        """查询文本审核任务接口 https://cloud.tencent.com/document/product/460/56284
+
+        :param Bucket(string): 存储桶名称.
+        :param JobID(string): 任务id.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询文本审核返回的结果
+            response = client.ci_auditing_text_query(
+                Bucket='bucket',
+                JobID='v11122zxxxazzz'
+            )
+            print response
+        """
+
+        return self.ci_auditing_query_common(
+            Bucket=Bucket,
+            JobID=JobID,
+            Type='text',
+            **kwargs
+        )
+
+    def ci_auditing_document_submit(self, Bucket, Url, DetectType, Type=None, Callback=None,  BizType=None, **kwargs):
+        """提交文档审核任务接口 https://cloud.tencent.com/document/product/460/59380
+
+        :param Bucket(string): 存储桶名称.
+        :param Url(string): 文档文件的链接地址，例如 http://www.example.com/doctest.doc
+        :param DetectType(int): 内容识别标志,位计算 1:porn, 2:terrorist, 4:politics, 8:ads
+        :param Type(string): 指定文档文件的类型，如未指定则默认以文件的后缀为类型。
+                             如果文件没有后缀，该字段必须指定，否则会审核失败。例如：doc、docx、ppt、pptx 等
+        :param Callback(string): 回调地址，以http://或者https://开头的地址。
+        :param BizType(string): 审核策略的唯一标识，由后台自动生成，在控制台中对应为Biztype值.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict):任务提交成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 识别cos上的文本
+            response = client.ci_auditing_document_submit(
+                Bucket='bucket',
+                DetectType=CiDetectType.PORN | CiDetectType.POLITICS,
+                Url='http://www.example.com/doctest.doc'
+            )
+            print response
+        """
+
+        Input = {'Url': Url}
+        if Type:
+            Input['Type'] = Type
+
+        conf = {
+        }
+
+        if Callback:
+            conf['Callback'] = Callback
+
+        return self.ci_auditing_submit_common(
+            Bucket=Bucket,
+            Key='',
+            Type='document',
+            BizType=BizType,
+            Conf=conf,
+            DetectType=DetectType,
+            Input=Input,
+            **kwargs
+        )
+
+    def ci_auditing_document_query(self, Bucket, JobID, **kwargs):
+        """查询文档审核任务接口 https://cloud.tencent.com/document/product/460/59383
+
+        :param Bucket(string): 存储桶名称.
+        :param JobID(string): 任务id.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询文本审核返回的结果
+            response = client.ci_auditing_document_query(
+                Bucket='bucket',
+                JobID='v11122zxxxazzz'
+            )
+            print response
+        """
+
+        return self.ci_auditing_query_common(
+            Bucket=Bucket,
+            JobID=JobID,
+            Type='document',
+            **kwargs
+        )
+
+    def ci_get_media_queue(self, Bucket, **kwargs):
+        """查询媒体处理队列接口 https://cloud.tencent.com/document/product/436/54045
+
+        :param Bucket(string): 存储桶名称.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 查询媒体处理队列接口
+            response = client.ci_get_media_queue(
+                Bucket='bucket'
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        params = format_values(params)
+
+        path = "/queue"
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        logger.info("get_media_queue result, url=:{url} ,headers=:{headers}, params=:{params}".format(
+            url=url,
+            headers=headers,
+            params=params))
+        rt = self.send_request(
+            method='GET',
+            url=url,
+            bucket=Bucket,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+
+        data = xml_to_dict(rt.content)
+        # 单个元素时将dict转为list
+        format_dict(data, ['QueueList'])
+        return data
+
+    def ci_create_media_jobs(self, Bucket, Jobs={}, Lst={}, **kwargs):
+        """ 创建任务接口 https://cloud.tencent.com/document/product/436/54013
+
+        :param Bucket(string): 存储桶名称.
+        :param Jobs(dict): 创建任务的配置.
+        :param Lst(dict): 创建任务dict转xml时去除Key数组.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 创建任务接口
+            response = client.ci_create_media_jobs(
+                Bucket='bucket'
+                Jobs={},
+                Lst={}
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        params = format_values(params)
+        xml_config = format_xml(data=Jobs, root='Request', lst=Lst)
+        path = "/jobs"
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        logger.info("create_media_jobs result, url=:{url} ,headers=:{headers}, params=:{params}, xml_config=:{xml_config}".format(
+            url=url,
+            headers=headers,
+            params=params,
+            xml_config=xml_config))
+        rt = self.send_request(
+            method='POST',
+            url=url,
+            bucket=Bucket,
+            data=xml_config,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+
+        data = xml_to_dict(rt.content)
+        # 单个元素时将dict转为list
+        format_dict(data, ['JobsDetail'])
+        return data
+
+    def ci_get_media_jobs(self, Bucket, JobIDs, **kwargs):
+        """ 查询任务接口 https://cloud.tencent.com/document/product/436/54010
+
+        :param Bucket(string): 存储桶名称.
+        :param JobIDs(string): 任务ID，以,分割多个任务ID.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 创建任务接口
+            response = client.ci_get_media_jobs(
+                Bucket='bucket'
+                JobIDs={}
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        params = format_values(params)
+        path = "/jobs/" + JobIDs
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        logger.info("get_media_jobs result, url=:{url} ,headers=:{headers}, params=:{params}".format(
+            url=url,
+            headers=headers,
+            params=params))
+        rt = self.send_request(
+            method='GET',
+            url=url,
+            bucket=Bucket,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+        logger.debug("ci_get_media_jobs result, url=:{url} ,content=:{content}".format(
+            url=url,
+            content=rt.content))
+
+        data = xml_to_dict(rt.content)
+        # 单个元素时将dict转为list
+        format_dict(data, ['JobsDetail'])
+        return data
+
+    def ci_list_media_jobs(self, Bucket, QueueId, Tag, StartCreationTime=None, EndCreationTime=None, OrderByTime='Desc', States='All', Size=10, NextToken='', **kwargs):
+        """ 查询任务接口 https://cloud.tencent.com/document/product/436/54011
+
+        :param Bucket(string): 存储桶名称.
+        :param QueueId(string): 队列ID.
+        :param Tag(string): 任务类型.
+        :param StartCreationTime(string): 开始时间.
+        :param EndCreationTime(string): 结束时间.
+        :param OrderByTime(string): 排序方式.
+        :param States(string): 任务状态.
+        :param Size(string): 任务个数.
+        :param NextToken(string): 请求的上下文，用于翻页.
+        :param kwargs(dict): 设置请求的headers.
+        :return(dict): 查询成功返回的结果,dict类型.
+
+        .. code-block:: python
+
+            config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key, Token=token)  # 获取配置对象
+            client = CosS3Client(config)
+            # 创建任务接口
+            response = client.ci_get_media_jobs(
+                Bucket='bucket'
+                QueueId='',
+                Tag='Transcode'
+            )
+            print response
+        """
+        headers = mapped(kwargs)
+        final_headers = {}
+        params = {}
+        for key in headers:
+            if key.startswith("response"):
+                params[key] = headers[key]
+            else:
+                final_headers[key] = headers[key]
+        headers = final_headers
+
+        params = format_values(params)
+        path = "/jobs"
+        url = self._conf.uri(bucket=Bucket, path=path, endpoint=self._conf._endpoint_ci)
+        url = u"{url}?{QueueId}&{Tag}&{OrderByTime}&{States}&{Size}&{NextToken}".format(
+            url=to_unicode(url),
+            QueueId=to_unicode('queueId='+QueueId),
+            Tag=to_unicode('tag='+Tag),
+            OrderByTime=to_unicode('orderByTime='+OrderByTime),
+            States=to_unicode('states='+States),
+            Size=to_unicode('size='+str(Size)),
+            NextToken=to_unicode('nextToken='+NextToken)
+        )
+        if StartCreationTime is not None:
+            url = u"{url}&{StartCreationTime}".format(StartCreationTime=to_unicode('startCreationTime='+StartCreationTime))
+        if EndCreationTime is not None:
+            url = u"{url}&{EndCreationTime}".format(EndCreationTime=to_unicode('endCreationTime='+EndCreationTime))
+        logger.info("list_media_jobs result, url=:{url} ,headers=:{headers}, params=:{params}".format(
+            url=url,
+            headers=headers,
+            params=params))
+        rt = self.send_request(
+            method='GET',
+            url=url,
+            bucket=Bucket,
+            auth=CosS3Auth(self._conf, path, params=params),
+            params=params,
+            headers=headers)
+        logger.debug("list_media_jobs result, url=:{url} ,content=:{content}".format(
+            url=url,
+            content=rt.content))
+        data = xml_to_dict(rt.content)
+        # 单个元素时将dict转为list
+        format_dict(data, ['JobsDetail'])
+        return data
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/resumable_downloader.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/resumable_downloader.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/select_event_stream.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/select_event_stream.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_threadpool.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_threadpool.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/demo.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/demo.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_comm.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_comm.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,35 +212,35 @@
 def format_values(data):
     """格式化headers和params中的values为bytes"""
     for i in data:
         data[i] = to_bytes(data[i])
     return data
 
 
-def format_endpoint(endpoint, region):
+def format_endpoint(endpoint, region, module=u'cos.'):
     """格式化终端域名"""
     if not endpoint and not region:
         raise CosClientError("Region or Endpoint is required not empty!")
     if not endpoint:
-        region = format_region(region)
+        region = format_region(region, module)
         return u"{region}.myqcloud.com".format(region=region)
     else:
         return to_unicode(endpoint)
 
 
-def format_region(region):
+def format_region(region, module=u'cos.'):
     """格式化地域"""
     if not isinstance(region, string_types):
         raise CosClientError("region is not string type")
     if not region:
         raise CosClientError("region is required not empty!")
     region = to_unicode(region)
     if not re.match(r'^[A-Za-z0-9][A-Za-z0-9.\-]*[A-Za-z0-9]$', region):
         raise CosClientError("region format is illegal, only digit, letter and - is allowed!")
-    if region.find(u'cos.') != -1:
+    if region.find(module) != -1:
         return region  # 传入cos.ap-beijing-1这样显示加上cos.的region
     if region == u'cn-north' or region == u'cn-south' or region == u'cn-east' or region == u'cn-south-2' or region == u'cn-southwest' or region == u'sg':
         return region  # 老域名不能加cos.
     #  支持v4域名映射到v5
     if region == u'cossh':
         return u'cos.ap-shanghai'
     if region == u'cosgz':
@@ -256,15 +256,15 @@
     if region == u'coshk':
         return u'cos.ap-hongkong'
     if region == u'cosca':
         return u'cos.na-toronto'
     if region == u'cosger':
         return u'cos.eu-frankfurt'
 
-    return u'cos.' + region  # 新域名加上cos.
+    return module + region  # 新域名加上cos.
 
 
 def format_bucket(bucket, appid):
     """兼容新老bucket长短命名,appid为空默认为长命名,appid不为空则认为是短命名"""
     if not isinstance(bucket, string_types):
         raise CosClientError("bucket is not string")
     if not bucket:
@@ -460,14 +460,35 @@
 class CiDetectType():
     """ci内容设备的类型设置,可与操作设多个"""
     PORN = 1
     TERRORIST = 2
     POLITICS = 4
     ADS = 8
 
+    @staticmethod
+    def get_detect_type_str(DetectType):
+        """获取审核的文字描述，这里只支持ci域名的入参，cos的跟这个还不一样"""
+        detect_type = ''
+        if DetectType & CiDetectType.PORN > 0:
+            detect_type += 'Porn'
+        if DetectType & CiDetectType.TERRORIST > 0:
+            if len(detect_type) > 0:
+                detect_type += ','
+            detect_type += 'Terrorism'
+        if DetectType & CiDetectType.POLITICS > 0:
+            if len(detect_type) > 0:
+                detect_type += ','
+            detect_type += 'Politics'
+        if DetectType & CiDetectType.ADS > 0:
+            if len(detect_type) > 0:
+                detect_type += ','
+            detect_type += 'Ads'
+
+        return detect_type
+
 
 class ProgressCallback():
     def __init__(self, file_size, progress_callback):
         self.__lock = threading.Lock()
         self.__finished_size = 0
         self.__file_size = file_size
         self.__progress_callback = progress_callback
```

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/streambody.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/streambody.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/cos_encryption_client.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/cos_encryption_client.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/crypto.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/crypto.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/qcloud_cos/xml2dict.py` & `cos-python-sdk-v5-1.9.9/qcloud_cos/xml2dict.py`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/PKG-INFO` & `cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: cos-python-sdk-v5
-Version: 1.9.8
+Version: 1.9.9
 Summary: cos-python-sdk-v5
 Home-page: https://www.qcloud.com/
 Author: tiedu, lewzylu, channingliu
 Author-email: dutie123@qq.com
 License: MIT
-Description: Qcloud COSv5 SDK
-        #######################
-        
-        .. image:: https://img.shields.io/pypi/v/cos-python-sdk-v5.svg
-           :target: https://pypi.org/search/?q=cos-python-sdk-v5
-           :alt: Pypi
-        .. image:: https://travis-ci.org/tencentyun/cos-python-sdk-v5.svg?branch=master
-           :target: https://travis-ci.org/tencentyun/cos-python-sdk-v5
-           :alt: Travis CI 
-        
-        介绍
-        _______
-        
-        腾讯云COSV5Python SDK, 目前可以支持Python2.6与Python2.7以及Python3.x。
-        
-        安装指南
-        __________
-        
-        使用pip安装 ::
-        
-            pip install -U cos-python-sdk-v5
-        
-        手动安装::
-        
-            python setup.py install
-        
-        使用方法
-        __________
-        
-        使用python sdk，参照 https://github.com/tencentyun/cos-python-sdk-v5/blob/master/demo/demo.py
-        
-        cos最新可用地域，参照 https://cloud.tencent.com/document/product/436/6224
-        
-        python sdk 快速入门，参照 https://cloud.tencent.com/document/product/436/12269
-        
-        python sdk 接口文档，参照 https://cloud.tencent.com/document/product/436/12270
-        
 Platform: UNKNOWN
+License-File: LICENSE
+
+Qcloud COSv5 SDK
+#######################
+
+.. image:: https://img.shields.io/pypi/v/cos-python-sdk-v5.svg
+   :target: https://pypi.org/search/?q=cos-python-sdk-v5
+   :alt: Pypi
+.. image:: https://api.travis-ci.com/tencentyun/cos-python-sdk-v5.svg?branch=master
+   :target: https://app.travis-ci.com/github/tencentyun/cos-python-sdk-v5
+   :alt: Travis CI 
+
+介绍
+_______
+
+腾讯云COSV5Python SDK, 目前可以支持Python2.6与Python2.7以及Python3.x。
+
+安装指南
+__________
+
+使用pip安装 ::
+
+    pip install -U cos-python-sdk-v5
+
+手动安装::
+
+    python setup.py install
+
+使用方法
+__________
+
+使用python sdk，参照 https://github.com/tencentyun/cos-python-sdk-v5/blob/master/demo/demo.py
+
+cos最新可用地域，参照 https://cloud.tencent.com/document/product/436/6224
+
+python sdk 快速入门，参照 https://cloud.tencent.com/document/product/436/12269
+
+python sdk 接口文档，参照 https://cloud.tencent.com/document/product/436/12270
+
+
```

### Comparing `cos-python-sdk-v5-1.9.8/cos_python_sdk_v5.egg-info/SOURCES.txt` & `cos-python-sdk-v5-1.9.9/cos_python_sdk_v5.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 cos_python_sdk_v5.egg-info/PKG-INFO
 cos_python_sdk_v5.egg-info/SOURCES.txt
 cos_python_sdk_v5.egg-info/dependency_links.txt
```

### Comparing `cos-python-sdk-v5-1.9.8/CHANGELOG.md` & `cos-python-sdk-v5-1.9.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cos-python-sdk-v5-1.9.8/README.rst` & `cos-python-sdk-v5-1.9.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Qcloud COSv5 SDK
 #######################
 
 .. image:: https://img.shields.io/pypi/v/cos-python-sdk-v5.svg
    :target: https://pypi.org/search/?q=cos-python-sdk-v5
    :alt: Pypi
-.. image:: https://travis-ci.org/tencentyun/cos-python-sdk-v5.svg?branch=master
-   :target: https://travis-ci.org/tencentyun/cos-python-sdk-v5
+.. image:: https://api.travis-ci.com/tencentyun/cos-python-sdk-v5.svg?branch=master
+   :target: https://app.travis-ci.com/github/tencentyun/cos-python-sdk-v5
    :alt: Travis CI 
 
 介绍
 _______
 
 腾讯云COSV5Python SDK, 目前可以支持Python2.6与Python2.7以及Python3.x。
```

### Comparing `cos-python-sdk-v5-1.9.8/PKG-INFO` & `cos-python-sdk-v5-1.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: cos-python-sdk-v5
-Version: 1.9.8
+Version: 1.9.9
 Summary: cos-python-sdk-v5
 Home-page: https://www.qcloud.com/
 Author: tiedu, lewzylu, channingliu
 Author-email: dutie123@qq.com
 License: MIT
-Description: Qcloud COSv5 SDK
-        #######################
-        
-        .. image:: https://img.shields.io/pypi/v/cos-python-sdk-v5.svg
-           :target: https://pypi.org/search/?q=cos-python-sdk-v5
-           :alt: Pypi
-        .. image:: https://travis-ci.org/tencentyun/cos-python-sdk-v5.svg?branch=master
-           :target: https://travis-ci.org/tencentyun/cos-python-sdk-v5
-           :alt: Travis CI 
-        
-        介绍
-        _______
-        
-        腾讯云COSV5Python SDK, 目前可以支持Python2.6与Python2.7以及Python3.x。
-        
-        安装指南
-        __________
-        
-        使用pip安装 ::
-        
-            pip install -U cos-python-sdk-v5
-        
-        手动安装::
-        
-            python setup.py install
-        
-        使用方法
-        __________
-        
-        使用python sdk，参照 https://github.com/tencentyun/cos-python-sdk-v5/blob/master/demo/demo.py
-        
-        cos最新可用地域，参照 https://cloud.tencent.com/document/product/436/6224
-        
-        python sdk 快速入门，参照 https://cloud.tencent.com/document/product/436/12269
-        
-        python sdk 接口文档，参照 https://cloud.tencent.com/document/product/436/12270
-        
 Platform: UNKNOWN
+License-File: LICENSE
+
+Qcloud COSv5 SDK
+#######################
+
+.. image:: https://img.shields.io/pypi/v/cos-python-sdk-v5.svg
+   :target: https://pypi.org/search/?q=cos-python-sdk-v5
+   :alt: Pypi
+.. image:: https://api.travis-ci.com/tencentyun/cos-python-sdk-v5.svg?branch=master
+   :target: https://app.travis-ci.com/github/tencentyun/cos-python-sdk-v5
+   :alt: Travis CI 
+
+介绍
+_______
+
+腾讯云COSV5Python SDK, 目前可以支持Python2.6与Python2.7以及Python3.x。
+
+安装指南
+__________
+
+使用pip安装 ::
+
+    pip install -U cos-python-sdk-v5
+
+手动安装::
+
+    python setup.py install
+
+使用方法
+__________
+
+使用python sdk，参照 https://github.com/tencentyun/cos-python-sdk-v5/blob/master/demo/demo.py
+
+cos最新可用地域，参照 https://cloud.tencent.com/document/product/436/6224
+
+python sdk 快速入门，参照 https://cloud.tencent.com/document/product/436/12269
+
+python sdk 接口文档，参照 https://cloud.tencent.com/document/product/436/12270
+
+
```

