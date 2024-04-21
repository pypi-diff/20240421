# Comparing `tmp/lamda-7.60.tar.gz` & `tmp/lamda-7.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lamda-7.60.tar", last modified: Sat Apr  6 05:46:10 2024, max compression
+gzip compressed data, was "dist/lamda-7.65.tar", last modified: Sun Apr 21 03:11:32 2024, max compression
```

## Comparing `lamda-7.60.tar` & `lamda-7.65.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-04-06 05:46:10.540284 lamda-7.60/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4341 2024-04-06 02:54:54.000000 lamda-7.60/README.md
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.536284 lamda-7.60/lamda/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      205 2024-04-06 05:37:37.000000 lamda-7.60/lamda/__init__.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)      894 2023-12-11 03:08:30.000000 lamda-7.60/lamda/bcast.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    74749 2024-04-04 10:11:38.000000 lamda-7.60/lamda/client.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     3167 2023-03-16 03:06:14.000000 lamda-7.60/lamda/const.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1603 2023-12-11 03:24:23.000000 lamda-7.60/lamda/exceptions.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.536284 lamda-7.60/lamda/google/
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/google/protobuf/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     5916 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/any.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     7734 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/api.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/google/protobuf/compiler/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8754 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/compiler/plugin.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    37969 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/descriptor.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4895 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/duration.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2429 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/empty.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8185 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/field_mask.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2341 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/source_context.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     3778 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/struct.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6459 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/timestamp.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6126 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/type.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4042 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/wrappers.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/rpc/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2393 2024-03-17 15:58:16.000000 lamda-7.60/lamda/rpc/application.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      430 2024-01-06 00:45:44.000000 lamda-7.60/lamda/rpc/debug.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      710 2024-01-06 00:45:39.000000 lamda-7.60/lamda/rpc/file.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      391 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/policy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2672 2024-01-13 06:01:07.000000 lamda-7.60/lamda/rpc/proxy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    12143 2024-03-29 03:25:45.000000 lamda-7.60/lamda/rpc/services.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      478 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/settings.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      609 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/shell.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2046 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/status.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      393 2023-12-11 03:09:19.000000 lamda-7.60/lamda/rpc/storage.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      434 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/types.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    19642 2024-04-04 09:53:04.000000 lamda-7.60/lamda/rpc/uiautomator.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1299 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/util.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1935 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/wifi.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1007 2023-12-11 03:11:52.000000 lamda-7.60/lamda/types.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda.egg-info/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1062 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/not-zip-safe
--rw-r--r--   0 whoami    (4096) whoami    (4096)      229 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/requires.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        6 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/top_level.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)       38 2024-04-06 05:46:10.540284 lamda-7.60/setup.cfg
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1635 2024-03-05 09:30:03.000000 lamda-7.60/setup.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-04-21 03:11:32.624092 lamda-7.65/PKG-INFO
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4295 2024-04-14 04:55:14.000000 lamda-7.65/README.md
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.620092 lamda-7.65/lamda/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      205 2024-04-21 03:02:42.000000 lamda-7.65/lamda/__init__.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      894 2023-12-11 03:08:30.000000 lamda-7.65/lamda/bcast.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    73463 2024-04-08 07:40:06.000000 lamda-7.65/lamda/client.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     3167 2023-03-16 03:06:14.000000 lamda-7.65/lamda/const.py
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1603 2023-12-11 03:24:23.000000 lamda-7.65/lamda/exceptions.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.620092 lamda-7.65/lamda/google/
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/google/protobuf/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     5916 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/any.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     7734 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/api.proto
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/google/protobuf/compiler/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     8754 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/compiler/plugin.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    37969 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/descriptor.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4895 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/duration.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2429 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/empty.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     8185 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/field_mask.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2341 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/source_context.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     3778 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/struct.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     6459 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/timestamp.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     6126 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/type.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     4042 2022-10-31 08:21:43.000000 lamda-7.65/lamda/google/protobuf/wrappers.proto
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda/rpc/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2393 2024-03-17 15:58:16.000000 lamda-7.65/lamda/rpc/application.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      327 2024-04-08 07:34:20.000000 lamda-7.65/lamda/rpc/debug.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      710 2024-01-06 00:45:39.000000 lamda-7.65/lamda/rpc/file.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      391 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/policy.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2672 2024-01-13 06:01:07.000000 lamda-7.65/lamda/rpc/proxy.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    11708 2024-04-08 07:39:31.000000 lamda-7.65/lamda/rpc/services.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      478 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/settings.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      609 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/shell.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     2046 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/status.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      393 2023-12-11 03:09:19.000000 lamda-7.65/lamda/rpc/storage.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      434 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/types.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)    19642 2024-04-04 09:53:04.000000 lamda-7.65/lamda/rpc/uiautomator.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1299 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/util.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1935 2024-01-10 15:26:13.000000 lamda-7.65/lamda/rpc/wifi.proto
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1007 2023-12-11 03:11:52.000000 lamda-7.65/lamda/types.py
+drwxrwxr-x   0 whoami    (1000) whoami    (1000)        0 2024-04-21 03:11:32.624092 lamda-7.65/lamda.egg-info/
+-rw-r--r--   0 whoami    (1000) whoami    (1000)      949 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/PKG-INFO
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)     1062 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/SOURCES.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/dependency_links.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        1 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/not-zip-safe
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)      229 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/requires.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)        6 2024-04-21 03:11:32.000000 lamda-7.65/lamda.egg-info/top_level.txt
+-rw-rw-r--   0 whoami    (1000) whoami    (1000)       38 2024-04-21 03:11:32.624092 lamda-7.65/setup.cfg
+-rw-r--r--   0 whoami    (1000) whoami    (1000)     1635 2024-03-05 09:30:03.000000 lamda-7.65/setup.py
```

### Comparing `lamda-7.60/PKG-INFO` & `lamda-7.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.60
+Version: 7.65
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.60/README.md` & `lamda-7.65/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 <p align="center">
 <img src="image/wx.png" alt="公众号" width="234">
 </p>
 <p align="center"><small>关注公众号查看视频教程以及更多使用方法</small><br><small><b>知识应该是共享的，我们不会要求你为相关知识付费</b></small><br><br><small><a href="https://space.bilibili.com/1964784386/video">BILIBILI 同步发布</a></small><br><small>文字版文档请查看<a href="https://github.com/rev1si0n/lamda/wiki">使用文档</a></small></small>
 </p>
 
 
-经过超 500 台设备的稳定生产环境考验，具有近乎商业级软件的质量和稳定性，仅需 root 权限即可正常运行。具备 ARM/X86 全架构，安卓 6.0-14 的广泛兼容性，支持模拟器、真机、云手机、 WSA（Windows Subsystem for Android™️）、无头开发板以及 Redroid。提供大量可编程接口，支持界面布局检视、获取/重放系统中最近的 Activity、唤起应用的 Activity 等功能。除此之外，它支持大文件上传下载，远程桌面，以及UI自动化编程接口，点击、截图、获取界面元素、执行 shell 命令、设备状态、资源读取、系统配置、属性读写、一键中间人等，可通过 SSH 或内置 ADB 登录设备终端。具备 socks5、OpenVPN 代理并可通过接口轻松设置根证书，实现中间人攻击，以及 Frida、IDA 等工具等等，同时支持定时任务、Magisk开机自启动，你可以在任何地方通过网络连接运行着 LAMDA 设备。
+经过超 500 台设备的稳定生产环境考验，具有近乎商业级软件的质量和稳定性，仅需 root 权限即可正常运行。具备 ARM/X86 全架构，安卓 6.0-14 的广泛兼容性，支持模拟器、真机、云手机、 WSA（Windows Subsystem for Android™️）、无头开发板以及 Redroid。提供大量可编程接口，支持界面布局检视、获取/重放系统中最近的 Activity、唤起应用的 Activity 等功能。除此之外，它支持大文件上传下载，远程桌面，以及UI自动化编程接口，点击、截图、获取界面元素、执行 shell 命令、设备状态、资源读取、系统配置、属性读写、一键中间人等，可通过 SSH 或内置 ADB 登录设备终端。具备 socks5、OpenVPN 代理并可通过接口轻松设置系统证书及中间人，同时支持定时任务、Magisk开机自启动，你可以在任何地方通过网络连接运行着 LAMDA 设备。
 
 ![动图演示](image/demo.gif)
 
 ## 一键中间人流量分析
 
 支持常规以及国际APP流量分析，DNS流量分析，得益于 [mitmproxy flow hook](https://docs.mitmproxy.org/stable/api/events.html)，你可以对任何请求做到最大限度的掌控，mitmproxy 功能足够丰富，你可以使用 Python 脚本实时修改或者捕获应用的请求，也可以通过其 `Export` 选项导出特定请求的 `curl` 命令或者 `HTTPie` 命令，分析重放、拦截修改、功能组合足以替代你用过的任何此类商业/非商业软件。如果你仍不清楚 mitmproxy 是什么以及其具有的能力，请务必先查找相关文档，因为 LAMDA 将会使用 mitmproxy 为你展现应用请求。
```

#### html2text {}

```diff
@@ -29,17 +29,15 @@
 Subsystem for Androidâ¢ï¸ï¼ãæ å¤´å¼åæ¿ä»¥å
 Redroidãæä¾å¤§éå¯ç¼ç¨æ¥å£ï¼æ¯æçé¢å¸å±æ£è§ãè·å/
 éæ¾ç³»ç»ä¸­æè¿ç Activityãå¤èµ·åºç¨ç Activity
 ç­åè½ãé¤æ­¤ä¹å¤ï¼å®æ¯æå¤§æä»¶ä¸ä¼ ä¸è½½ï¼è¿ç¨æ¡é¢ï¼ä»¥åUIèªå¨åç¼ç¨æ¥å£ï¼ç¹å»ãæªå¾ãè·åçé¢åç´ ãæ§è¡
 shell
 å½ä»¤ãè®¾å¤ç¶æãèµæºè¯»åãç³»ç»éç½®ãå±æ§è¯»åãä¸é®ä¸­é´äººç­ï¼å¯éè¿
 SSH æåç½® ADB ç»å½è®¾å¤ç»ç«¯ãå·å¤ socks5ãOpenVPN
-ä»£çå¹¶å¯éè¿æ¥å£è½»æ¾è®¾ç½®æ ¹è¯ä¹¦ï¼å®ç°ä¸­é´äººæ»å»ï¼ä»¥å
-FridaãIDA
-ç­å·¥å·ç­ç­ï¼åæ¶æ¯æå®æ¶ä»»å¡ãMagiskå¼æºèªå¯å¨ï¼ä½ å¯ä»¥å¨ä»»ä½å°æ¹éè¿ç½ç»è¿æ¥è¿è¡ç
+ä»£çå¹¶å¯éè¿æ¥å£è½»æ¾è®¾ç½®ç³»ç»è¯ä¹¦åä¸­é´äººï¼åæ¶æ¯æå®æ¶ä»»å¡ãMagiskå¼æºèªå¯å¨ï¼ä½ å¯ä»¥å¨ä»»ä½å°æ¹éè¿ç½ç»è¿æ¥è¿è¡ç
 LAMDA è®¾å¤ã ![å¨å¾æ¼ç¤º](image/demo.gif) ## ä¸é®ä¸­é´äººæµéåæ
 æ¯æå¸¸è§ä»¥åå½éAPPæµéåæï¼DNSæµéåæï¼å¾çäº
 [mitmproxy flow hook](https://docs.mitmproxy.org/stable/api/
 events.html)ï¼ä½ å¯ä»¥å¯¹ä»»ä½è¯·æ±åå°æå¤§éåº¦çææ§ï¼mitmproxy
 åè½è¶³å¤ä¸°å¯ï¼ä½ å¯ä»¥ä½¿ç¨ Python
 èæ¬å®æ¶ä¿®æ¹æèæè·åºç¨çè¯·æ±ï¼ä¹å¯ä»¥éè¿å¶ `Export`
 éé¡¹å¯¼åºç¹å®è¯·æ±ç `curl` å½ä»¤æè `HTTPie`
```

### Comparing `lamda-7.60/lamda/bcast.proto` & `lamda-7.65/lamda/bcast.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/client.py` & `lamda-7.65/lamda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1369,72 +1369,26 @@
         return r.value
     def is_android_debug_bridge_running(self):
         """
         远端 adb daemon 是否在运行
         """
         r = self.stub.isAndroidDebugBridgeRunning(protos.Empty())
         return r.value
-    def is_ida_running(self):
-        """
-        IDA 服务端是否在运行
-        """
-        r = self.stub.isIDARunning(protos.Empty())
-        return r.value
-    def is_ida64_running(self):
-        """
-        IDA64 服务端是否在运行
-        """
-        r = self.stub.isIDA64Running(protos.Empty())
-        return r.value
     def start_android_debug_bridge(self):
         """
         启动内置 adbd (默认随框架启动)
         """
         r = self.stub.startAndroidDebugBridge(protos.Empty())
         return r.value
-    def start_ida(self, port=23932, **env):
-        """
-        启动 IDA 服务端
-        """
-        req = protos.IDAConfigRequest(port=port)
-        req.environment.update(env)
-        r = self.stub.startIDA(req)
-        return r.value
-    def start_ida64(self, port=23964, **env):
-        """
-        启动 IDA64 服务端
-        """
-        req = protos.IDAConfigRequest(port=port)
-        req.environment.update(env)
-        r = self.stub.startIDA64(req)
-        return r.value
     def stop_android_debug_bridge(self):
         """
         停止内置 adb daemon
         """
         r = self.stub.stopAndroidDebugBridge(protos.Empty())
         return r.value
-    def set_debuggable(self):
-        """
-        设置系统为 debuggable
-        """
-        r = self.stub.setDebuggable(protos.Empty())
-        return r.value
-    def stop_ida(self):
-        """
-        停止 IDA 服务端
-        """
-        r = self.stub.stopIDA(protos.Empty())
-        return r.value
-    def stop_ida64(self):
-        """
-        停止 IDA64 服务端
-        """
-        r = self.stub.stopIDA64(protos.Empty())
-        return r.value
 
 
 class SettingsStub(BaseServiceStub):
     def _put(self, group, name, value):
         req = protos.SettingsRequest(group=group, name=name,
                                             value=value)
         r = self.stub.putSettings(req)
```

### Comparing `lamda-7.60/lamda/const.py` & `lamda-7.65/lamda/const.py`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/exceptions.py` & `lamda-7.65/lamda/exceptions.py`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/any.proto` & `lamda-7.65/lamda/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/api.proto` & `lamda-7.65/lamda/google/protobuf/api.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/compiler/plugin.proto` & `lamda-7.65/lamda/google/protobuf/compiler/plugin.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/descriptor.proto` & `lamda-7.65/lamda/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/duration.proto` & `lamda-7.65/lamda/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/empty.proto` & `lamda-7.65/lamda/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/field_mask.proto` & `lamda-7.65/lamda/google/protobuf/field_mask.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/source_context.proto` & `lamda-7.65/lamda/google/protobuf/source_context.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/struct.proto` & `lamda-7.65/lamda/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/timestamp.proto` & `lamda-7.65/lamda/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/type.proto` & `lamda-7.65/lamda/google/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/google/protobuf/wrappers.proto` & `lamda-7.65/lamda/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/application.proto` & `lamda-7.65/lamda/rpc/application.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/file.proto` & `lamda-7.65/lamda/rpc/file.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/proxy.proto` & `lamda-7.65/lamda/rpc/proxy.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/services.proto` & `lamda-7.65/lamda/rpc/services.proto`

 * *Files 1% similar despite different names*

```diff
@@ -48,29 +48,21 @@
     rpc isInstalled(ApplicationRequest) returns (Boolean) {}
 
     rpc addToDozeModeWhiteList(ApplicationRequest) returns (Boolean) {}
     rpc removeFromDozeModeWhiteList(ApplicationRequest) returns (Boolean) {}
 }
 
 service Debug {
-    rpc isIDARunning(google.protobuf.Empty) returns (Boolean) {}
-    rpc isIDA64Running(google.protobuf.Empty) returns (Boolean) {}
     rpc isAndroidDebugBridgeRunning(google.protobuf.Empty) returns (Boolean) {}
 
     rpc installADBPubKey(ADBDConfigRequest) returns (Boolean) {}
     rpc uninstallADBPubKey(ADBDConfigRequest) returns (Boolean) {}
 
-    rpc startIDA(IDAConfigRequest) returns (Boolean) {}
-    rpc startIDA64(IDAConfigRequest) returns (Boolean) {}
     rpc startAndroidDebugBridge(google.protobuf.Empty) returns (Boolean) {}
-
-    rpc stopIDA(google.protobuf.Empty) returns (Boolean) {}
-    rpc stopIDA64(google.protobuf.Empty) returns (Boolean) {}
     rpc stopAndroidDebugBridge(google.protobuf.Empty) returns (Boolean) {}
-    rpc setDebuggable(google.protobuf.Empty) returns (Boolean) {}
 }
 
 service Proxy {
     rpc isOpenVPNRunning(google.protobuf.Empty) returns (Boolean) {}
     rpc isGproxyRunning(google.protobuf.Empty) returns (Boolean) {}
     rpc stopOpenVPN(google.protobuf.Empty) returns (Boolean) {}
     rpc stopGproxy(google.protobuf.Empty) returns (Boolean) {}
```

### Comparing `lamda-7.60/lamda/rpc/shell.proto` & `lamda-7.65/lamda/rpc/shell.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/status.proto` & `lamda-7.65/lamda/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/uiautomator.proto` & `lamda-7.65/lamda/rpc/uiautomator.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/util.proto` & `lamda-7.65/lamda/rpc/util.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/rpc/wifi.proto` & `lamda-7.65/lamda/rpc/wifi.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda/types.py` & `lamda-7.65/lamda/types.py`

 * *Files identical despite different names*

### Comparing `lamda-7.60/lamda.egg-info/PKG-INFO` & `lamda-7.65/lamda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.60
+Version: 7.65
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.60/lamda.egg-info/SOURCES.txt` & `lamda-7.65/lamda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lamda-7.60/setup.py` & `lamda-7.65/setup.py`

 * *Files identical despite different names*

