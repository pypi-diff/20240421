# Comparing `tmp/dubborequests-0.9.3.tar.gz` & `tmp/dubborequests-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubborequests-0.9.3.tar", last modified: Wed Aug 30 16:02:50 2023, max compression
+gzip compressed data, was "dubborequests-0.9.4.tar", last modified: Sun Apr 21 15:01:07 2024, max compression
```

## Comparing `dubborequests-0.9.3.tar` & `dubborequests-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-30 16:02:50.541582 dubborequests-0.9.3/
--rw-r--r--   0 fa_junjie   (501) staff       (20)     6422 2023-08-30 16:02:50.541431 dubborequests-0.9.3/PKG-INFO
--rw-r--r--   0 fa_junjie   (501) staff       (20)     4895 2023-08-30 16:00:12.000000 dubborequests-0.9.3/README.md
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-30 16:02:50.540463 dubborequests-0.9.3/dubborequests/
--rw-r--r--   0 fa_junjie   (501) staff       (20)      207 2023-02-01 14:29:05.000000 dubborequests-0.9.3/dubborequests/__init__.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)     3654 2023-08-09 01:34:13.000000 dubborequests-0.9.3/dubborequests/api.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)      258 2023-03-24 03:07:07.000000 dubborequests-0.9.3/dubborequests/config.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)     9445 2023-08-30 15:58:51.000000 dubborequests-0.9.3/dubborequests/util.py
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-30 16:02:50.541183 dubborequests-0.9.3/dubborequests.egg-info/
--rw-r--r--   0 fa_junjie   (501) staff       (20)     6422 2023-08-30 16:02:50.000000 dubborequests-0.9.3/dubborequests.egg-info/PKG-INFO
--rw-r--r--   0 fa_junjie   (501) staff       (20)      295 2023-08-30 16:02:50.000000 dubborequests-0.9.3/dubborequests.egg-info/SOURCES.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)        1 2023-08-30 16:02:50.000000 dubborequests-0.9.3/dubborequests.egg-info/dependency_links.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)        6 2023-08-30 16:02:50.000000 dubborequests-0.9.3/dubborequests.egg-info/requires.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)       14 2023-08-30 16:02:50.000000 dubborequests-0.9.3/dubborequests.egg-info/top_level.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)       38 2023-08-30 16:02:50.541633 dubborequests-0.9.3/setup.cfg
--rw-r--r--   0 fa_junjie   (501) staff       (20)      782 2023-08-30 15:30:42.000000 dubborequests-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:01:07.737528 dubborequests-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-21 15:00:58.000000 dubborequests-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-21 15:01:07.737528 dubborequests-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-21 15:00:58.000000 dubborequests-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:01:07.737528 dubborequests-0.9.4/dubborequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-21 15:00:58.000000 dubborequests-0.9.4/dubborequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-21 15:00:58.000000 dubborequests-0.9.4/dubborequests/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 15:00:58.000000 dubborequests-0.9.4/dubborequests/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-21 15:00:58.000000 dubborequests-0.9.4/dubborequests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:01:07.737528 dubborequests-0.9.4/dubborequests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-21 15:01:07.000000 dubborequests-0.9.4/dubborequests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 15:01:07.000000 dubborequests-0.9.4/dubborequests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:01:07.000000 dubborequests-0.9.4/dubborequests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 15:01:07.000000 dubborequests-0.9.4/dubborequests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 15:01:07.000000 dubborequests-0.9.4/dubborequests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 15:01:07.737528 dubborequests-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-21 15:00:58.000000 dubborequests-0.9.4/setup.py
```

### Comparing `dubborequests-0.9.3/PKG-INFO` & `dubborequests-0.9.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,153 @@
 Metadata-Version: 2.1
 Name: dubborequests
-Version: 0.9.3
+Version: 0.9.4
 Summary: Telnet command test dubbo
 Home-page: https://github.com/JokerChat/dubbo_requests
 Author: fang
 Author-email: 664616581@qq.com
 License: MIT
-Description: ### 一、安装（python版本建议3.7以上）
-        
-        ```bash
-        pip install dubborequests
-        ```
-        ### 二、升级包
-        ```bash
-        pip install --upgrade dubborequests
-        ```
-        ### 三、示例
-        
-        #### 获取dubbo服务详情
-        
-        ```python
-        # 导入
-        import dubborequests
-        from dubborequests.config import Config
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        # 获取dubbo服务详情
-        data = dubborequests.search('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 模糊查询dubbo服务
-        search_data = dubborequests.get_service_like('SsoEmpInfoService')
-        ```
-        
-        #### 获取服务下的所有方法
-        
-        ```python
-        # 导入
-        import dubborequests
-        from dubborequests.config import Config
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        # 获取dubbo服务下的所有方法
-        service_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 获取指定版本dubbo服务下的所有方法
-        service_data_by_version = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', version='2.0.0')
-        # 获取dubbo服务指定的方法
-        method_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
-        # 通过ip+端口获取dubbo服务下的所有方法（此方法无需配置zookeeper地址）
-        service_data1 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 通过ip+端口获取dubbo服务指定的方法（此方法无需配置zookeeper地址）
-        method_data2 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
-        ```
-        
-        #### 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
-        
-        ```python
-        import dubborequests
-        from dubborequests import Config
-        # 先配置zookeeper中心地址
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        service_name = "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService"
-        method_name = "login"
-        data = {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        # 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
-        res_data = dubborequests.zk_invoke(service_name, method_name, data)
-        # 如果想要指定版本的服务名，带上version即可
-        version = '2.0.0'
-        res_data_by_version = dubborequests.zk_invoke(service_name, method_name, data, version)
-        # 如果入参类型是java.lang.String
-        invoke_data1 = {
-                "account": "xxxx"
-            }
-        # 如果入参类型是java.lang.String, 但是这个String是由json转换而来的, 需要将json进行压缩转义进行传参
-        invoke_data2 = {
-                "listDto": "[{\"warehouseCode\":\"99999\",\"warehouseName\":\"zym仓库\",\"warehouseType\":1,\"warehouseSmallCategory\":\"1221\",\"province\":\"44\",\"city\":\"4401\",\"district\":\"440101\",\"warehouseAddress\":\"这是地址\",\"dataSource\":1,\"createTime\":\"2020-08-26 00:00:00\",\"townName\":\"乡镇名称\",\"villageName\":\"名称\"}]"
-            }
-        # 如果入参类型是java.util.List
-        invoke_data3 = {
-                "list_": ["数组的内容"]
-            }
-        # 如果入参类型是java.util.Map、java.util.HashMap或者自定义对象名(com.your.package.BeanName)
-        invoke_data4 = {
-                "map_": {
-                  "age":27,
-                  "name": "clearlove7"
-                }
-            }
-        # 如果无需入参类型, data为空dict即可
-        invoke_data5 = {}
-        # 组合入参类型1, java.lang.String、java.lang.String
-        invoke_data6 = {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        # 组合入参类型2, java.lang.String、java.util.List
-        invoke_data7 = {
-                "account": "xxxx",
-                "list_": ["数组的内容"]
-            }
-        # 组合入参类型3, cn.com.xxx.xxx.dto.xxx.ProductQuery、java.util.Map
-        invoke_data8 = {
-            "map1": {
-                "product": 10086,
-                "num": 1
-            },
-            "map2": {
-                "age": 27,
-                "name": "clearlove7"
-            }
-        }
-        # 如果入参类型是枚举
-        # 'ENUM' in param_type.upper() 主要判断逻辑是这个 
-        # 如需调整，可根据实际情况来
-        invoke_data9 = {
-                "name": "blue"
-            }
-        # 注意：
-        #1、len(data)必须等于方法入参个数
-        #2、data里面的key可以随意命名，data必须为dict类型
-        #3、data里面的key-value排序必须按照方法定义的入参顺序
-        # 详细可参照：https://github.com/thubbo/jmeter-plugins-for-apache-dubbo/wiki/ParameterComparisonTable
-        ```
-        
-        #### Telnet命令测试dubbo接口
-        
-        ```python
-        import dubborequests
-        invoke_data = {
-            "ip": 'xxxx',
-            "port": 7777,
-            "service_name": "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService",
-            "method_name": "login",
-            "data": {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        }
-         # Telnet命令测试dubbo接口
-        res_data = dubborequests.telnet_invoke(**invoke_data)
-        # 入参例子参考上面👆🏻
-        ```
-        ### 四、基于dubbo接口测试库转换成 http 便捷请求
-        项目地址：https://github.com/JokerChat/dubbo_fastapi
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### 一、安装（python版本建议3.9以上）
+
+```bash
+pip install dubborequests
+```
+### 二、升级包
+```bash
+pip install --upgrade dubborequests
+```
+### 三、示例
+
+#### 获取dubbo服务详情
+
+```python
+# 导入
+import dubborequests
+from dubborequests.config import Config
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+# 获取dubbo服务详情
+data = dubborequests.search('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 模糊查询dubbo服务
+search_data = dubborequests.get_service_like('SsoEmpInfoService')
+```
+
+#### 获取服务下的所有方法
+
+```python
+# 导入
+import dubborequests
+from dubborequests.config import Config
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+# 获取dubbo服务下的所有方法
+service_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 获取指定版本dubbo服务下的所有方法
+service_data_by_version = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', version='2.0.0')
+# 获取dubbo服务指定的方法
+method_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
+# 通过ip+端口获取dubbo服务下的所有方法（此方法无需配置zookeeper地址）
+service_data1 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 通过ip+端口获取dubbo服务指定的方法（此方法无需配置zookeeper地址）
+method_data2 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
+```
+
+#### 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
+
+```python
+import dubborequests
+from dubborequests import Config
+# 先配置zookeeper中心地址
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+service_name = "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService"
+method_name = "login"
+data = {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+# 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
+res_data = dubborequests.zk_invoke(service_name, method_name, data)
+# 如果想要指定版本的服务名，带上version即可
+version = '2.0.0'
+res_data_by_version = dubborequests.zk_invoke(service_name, method_name, data, version)
+# 如果入参类型是java.lang.String
+invoke_data1 = {
+        "account": "xxxx"
+    }
+# 如果入参类型是java.lang.String, 但是这个String是由json转换而来的, 需要将json进行压缩转义进行传参
+invoke_data2 = {
+        "listDto": "[{\"warehouseCode\":\"99999\",\"warehouseName\":\"zym仓库\",\"warehouseType\":1,\"warehouseSmallCategory\":\"1221\",\"province\":\"44\",\"city\":\"4401\",\"district\":\"440101\",\"warehouseAddress\":\"这是地址\",\"dataSource\":1,\"createTime\":\"2020-08-26 00:00:00\",\"townName\":\"乡镇名称\",\"villageName\":\"名称\"}]"
+    }
+# 如果入参类型是java.util.List
+invoke_data3 = {
+        "list_": ["数组的内容"]
+    }
+# 如果入参类型是java.util.Map、java.util.HashMap或者自定义对象名(com.your.package.BeanName)
+invoke_data4 = {
+        "map_": {
+          "age":27,
+          "name": "clearlove7"
+        }
+    }
+# 如果无需入参类型, data为空dict即可
+invoke_data5 = {}
+# 组合入参类型1, java.lang.String、java.lang.String
+invoke_data6 = {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+# 组合入参类型2, java.lang.String、java.util.List
+invoke_data7 = {
+        "account": "xxxx",
+        "list_": ["数组的内容"]
+    }
+# 组合入参类型3, cn.com.xxx.xxx.dto.xxx.ProductQuery、java.util.Map
+invoke_data8 = {
+    "map1": {
+        "product": 10086,
+        "num": 1
+    },
+    "map2": {
+        "age": 27,
+        "name": "clearlove7"
+    }
+}
+# 如果入参类型是枚举
+# 'ENUM' in param_type.upper() 主要判断逻辑是这个 
+# 如需调整，可根据实际情况来
+invoke_data9 = {
+        "name": "blue"
+    }
+# 注意：
+#1、len(data)必须等于方法入参个数
+#2、data里面的key可以随意命名，data必须为dict类型
+#3、data里面的key-value排序必须按照方法定义的入参顺序
+# 详细可参照：https://github.com/thubbo/jmeter-plugins-for-apache-dubbo/wiki/ParameterComparisonTable
+```
+
+#### Telnet命令测试dubbo接口
+
+```python
+import dubborequests
+invoke_data = {
+    "ip": 'xxxx',
+    "port": 7777,
+    "service_name": "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService",
+    "method_name": "login",
+    "data": {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+}
+ # Telnet命令测试dubbo接口
+res_data = dubborequests.telnet_invoke(**invoke_data)
+# 入参例子参考上面👆🏻
+```
+### 四、基于dubbo接口测试库转换成 http 便捷请求
+项目地址：https://github.com/JokerChat/dubbo_fastapi
+
```

### Comparing `dubborequests-0.9.3/README.md` & `dubborequests-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### 一、安装（python版本建议3.7以上）
+### 一、安装（python版本建议3.9以上）
 
 ```bash
 pip install dubborequests
 ```
 ### 二、升级包
 ```bash
 pip install --upgrade dubborequests
```

### Comparing `dubborequests-0.9.3/dubborequests/api.py` & `dubborequests-0.9.4/dubborequests/api.py`

 * *Files identical despite different names*

### Comparing `dubborequests-0.9.3/dubborequests/util.py` & `dubborequests-0.9.4/dubborequests/util.py`

 * *Files identical despite different names*

### Comparing `dubborequests-0.9.3/dubborequests.egg-info/PKG-INFO` & `dubborequests-0.9.4/dubborequests.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,153 @@
 Metadata-Version: 2.1
 Name: dubborequests
-Version: 0.9.3
+Version: 0.9.4
 Summary: Telnet command test dubbo
 Home-page: https://github.com/JokerChat/dubbo_requests
 Author: fang
 Author-email: 664616581@qq.com
 License: MIT
-Description: ### 一、安装（python版本建议3.7以上）
-        
-        ```bash
-        pip install dubborequests
-        ```
-        ### 二、升级包
-        ```bash
-        pip install --upgrade dubborequests
-        ```
-        ### 三、示例
-        
-        #### 获取dubbo服务详情
-        
-        ```python
-        # 导入
-        import dubborequests
-        from dubborequests.config import Config
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        # 获取dubbo服务详情
-        data = dubborequests.search('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 模糊查询dubbo服务
-        search_data = dubborequests.get_service_like('SsoEmpInfoService')
-        ```
-        
-        #### 获取服务下的所有方法
-        
-        ```python
-        # 导入
-        import dubborequests
-        from dubborequests.config import Config
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        # 获取dubbo服务下的所有方法
-        service_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 获取指定版本dubbo服务下的所有方法
-        service_data_by_version = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', version='2.0.0')
-        # 获取dubbo服务指定的方法
-        method_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
-        # 通过ip+端口获取dubbo服务下的所有方法（此方法无需配置zookeeper地址）
-        service_data1 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
-        # 通过ip+端口获取dubbo服务指定的方法（此方法无需配置zookeeper地址）
-        method_data2 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
-        ```
-        
-        #### 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
-        
-        ```python
-        import dubborequests
-        from dubborequests import Config
-        # 先配置zookeeper中心地址
-        Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
-        service_name = "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService"
-        method_name = "login"
-        data = {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        # 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
-        res_data = dubborequests.zk_invoke(service_name, method_name, data)
-        # 如果想要指定版本的服务名，带上version即可
-        version = '2.0.0'
-        res_data_by_version = dubborequests.zk_invoke(service_name, method_name, data, version)
-        # 如果入参类型是java.lang.String
-        invoke_data1 = {
-                "account": "xxxx"
-            }
-        # 如果入参类型是java.lang.String, 但是这个String是由json转换而来的, 需要将json进行压缩转义进行传参
-        invoke_data2 = {
-                "listDto": "[{\"warehouseCode\":\"99999\",\"warehouseName\":\"zym仓库\",\"warehouseType\":1,\"warehouseSmallCategory\":\"1221\",\"province\":\"44\",\"city\":\"4401\",\"district\":\"440101\",\"warehouseAddress\":\"这是地址\",\"dataSource\":1,\"createTime\":\"2020-08-26 00:00:00\",\"townName\":\"乡镇名称\",\"villageName\":\"名称\"}]"
-            }
-        # 如果入参类型是java.util.List
-        invoke_data3 = {
-                "list_": ["数组的内容"]
-            }
-        # 如果入参类型是java.util.Map、java.util.HashMap或者自定义对象名(com.your.package.BeanName)
-        invoke_data4 = {
-                "map_": {
-                  "age":27,
-                  "name": "clearlove7"
-                }
-            }
-        # 如果无需入参类型, data为空dict即可
-        invoke_data5 = {}
-        # 组合入参类型1, java.lang.String、java.lang.String
-        invoke_data6 = {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        # 组合入参类型2, java.lang.String、java.util.List
-        invoke_data7 = {
-                "account": "xxxx",
-                "list_": ["数组的内容"]
-            }
-        # 组合入参类型3, cn.com.xxx.xxx.dto.xxx.ProductQuery、java.util.Map
-        invoke_data8 = {
-            "map1": {
-                "product": 10086,
-                "num": 1
-            },
-            "map2": {
-                "age": 27,
-                "name": "clearlove7"
-            }
-        }
-        # 如果入参类型是枚举
-        # 'ENUM' in param_type.upper() 主要判断逻辑是这个 
-        # 如需调整，可根据实际情况来
-        invoke_data9 = {
-                "name": "blue"
-            }
-        # 注意：
-        #1、len(data)必须等于方法入参个数
-        #2、data里面的key可以随意命名，data必须为dict类型
-        #3、data里面的key-value排序必须按照方法定义的入参顺序
-        # 详细可参照：https://github.com/thubbo/jmeter-plugins-for-apache-dubbo/wiki/ParameterComparisonTable
-        ```
-        
-        #### Telnet命令测试dubbo接口
-        
-        ```python
-        import dubborequests
-        invoke_data = {
-            "ip": 'xxxx',
-            "port": 7777,
-            "service_name": "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService",
-            "method_name": "login",
-            "data": {
-                "account": "xxxx",
-                "password": "xxxx"
-            }
-        }
-         # Telnet命令测试dubbo接口
-        res_data = dubborequests.telnet_invoke(**invoke_data)
-        # 入参例子参考上面👆🏻
-        ```
-        ### 四、基于dubbo接口测试库转换成 http 便捷请求
-        项目地址：https://github.com/JokerChat/dubbo_fastapi
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### 一、安装（python版本建议3.9以上）
+
+```bash
+pip install dubborequests
+```
+### 二、升级包
+```bash
+pip install --upgrade dubborequests
+```
+### 三、示例
+
+#### 获取dubbo服务详情
+
+```python
+# 导入
+import dubborequests
+from dubborequests.config import Config
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+# 获取dubbo服务详情
+data = dubborequests.search('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 模糊查询dubbo服务
+search_data = dubborequests.get_service_like('SsoEmpInfoService')
+```
+
+#### 获取服务下的所有方法
+
+```python
+# 导入
+import dubborequests
+from dubborequests.config import Config
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+# 获取dubbo服务下的所有方法
+service_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 获取指定版本dubbo服务下的所有方法
+service_data_by_version = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', version='2.0.0')
+# 获取dubbo服务指定的方法
+method_data = dubborequests.list('cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
+# 通过ip+端口获取dubbo服务下的所有方法（此方法无需配置zookeeper地址）
+service_data1 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService')
+# 通过ip+端口获取dubbo服务指定的方法（此方法无需配置zookeeper地址）
+method_data2 = dubborequests.telnet_list('192.168.242.72', '30912', 'cn.com.xxx.sso.ehr.api.dubbo.SsoEmpInfoService', 'login')
+```
+
+#### 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
+
+```python
+import dubborequests
+from dubborequests import Config
+# 先配置zookeeper中心地址
+Config.zookeeper_url_list = ['192.168.240.15:2181', '192.168.240.15:2182', '192.168.240.15:2183']
+service_name = "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService"
+method_name = "login"
+data = {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+# 通过zookeeper获取服务的ip和端口, Telnet命令测试dubbo接口
+res_data = dubborequests.zk_invoke(service_name, method_name, data)
+# 如果想要指定版本的服务名，带上version即可
+version = '2.0.0'
+res_data_by_version = dubborequests.zk_invoke(service_name, method_name, data, version)
+# 如果入参类型是java.lang.String
+invoke_data1 = {
+        "account": "xxxx"
+    }
+# 如果入参类型是java.lang.String, 但是这个String是由json转换而来的, 需要将json进行压缩转义进行传参
+invoke_data2 = {
+        "listDto": "[{\"warehouseCode\":\"99999\",\"warehouseName\":\"zym仓库\",\"warehouseType\":1,\"warehouseSmallCategory\":\"1221\",\"province\":\"44\",\"city\":\"4401\",\"district\":\"440101\",\"warehouseAddress\":\"这是地址\",\"dataSource\":1,\"createTime\":\"2020-08-26 00:00:00\",\"townName\":\"乡镇名称\",\"villageName\":\"名称\"}]"
+    }
+# 如果入参类型是java.util.List
+invoke_data3 = {
+        "list_": ["数组的内容"]
+    }
+# 如果入参类型是java.util.Map、java.util.HashMap或者自定义对象名(com.your.package.BeanName)
+invoke_data4 = {
+        "map_": {
+          "age":27,
+          "name": "clearlove7"
+        }
+    }
+# 如果无需入参类型, data为空dict即可
+invoke_data5 = {}
+# 组合入参类型1, java.lang.String、java.lang.String
+invoke_data6 = {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+# 组合入参类型2, java.lang.String、java.util.List
+invoke_data7 = {
+        "account": "xxxx",
+        "list_": ["数组的内容"]
+    }
+# 组合入参类型3, cn.com.xxx.xxx.dto.xxx.ProductQuery、java.util.Map
+invoke_data8 = {
+    "map1": {
+        "product": 10086,
+        "num": 1
+    },
+    "map2": {
+        "age": 27,
+        "name": "clearlove7"
+    }
+}
+# 如果入参类型是枚举
+# 'ENUM' in param_type.upper() 主要判断逻辑是这个 
+# 如需调整，可根据实际情况来
+invoke_data9 = {
+        "name": "blue"
+    }
+# 注意：
+#1、len(data)必须等于方法入参个数
+#2、data里面的key可以随意命名，data必须为dict类型
+#3、data里面的key-value排序必须按照方法定义的入参顺序
+# 详细可参照：https://github.com/thubbo/jmeter-plugins-for-apache-dubbo/wiki/ParameterComparisonTable
+```
+
+#### Telnet命令测试dubbo接口
+
+```python
+import dubborequests
+invoke_data = {
+    "ip": 'xxxx',
+    "port": 7777,
+    "service_name": "cn.com.xxxxx.sso.ehr.api.dubbo.SsoEmpInfoService",
+    "method_name": "login",
+    "data": {
+        "account": "xxxx",
+        "password": "xxxx"
+    }
+}
+ # Telnet命令测试dubbo接口
+res_data = dubborequests.telnet_invoke(**invoke_data)
+# 入参例子参考上面👆🏻
+```
+### 四、基于dubbo接口测试库转换成 http 便捷请求
+项目地址：https://github.com/JokerChat/dubbo_fastapi
+
```

### Comparing `dubborequests-0.9.3/setup.py` & `dubborequests-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dubborequests",
-    version="0.9.3",
+    version="0.9.4",
     author="fang",
     author_email="664616581@qq.com",
     description="Telnet command test dubbo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JokerChat/dubbo_requests",
     packages=setuptools.find_packages(),
-    python_requires='>=3.7.0',
+    python_requires='>=3.9.0',
     install_requires=['kazoo'],
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

