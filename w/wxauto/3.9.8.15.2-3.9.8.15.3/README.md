# Comparing `tmp/wxauto-3.9.8.15.2.tar.gz` & `tmp/wxauto-3.9.8.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.2.tar", last modified: Tue Apr 16 07:35:38 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.3.tar", last modified: Sun Apr 21 11:49:24 2024, max compression
```

## Comparing `wxauto-3.9.8.15.2.tar` & `wxauto-3.9.8.15.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/
--rw-rw-rw-   0        0        0     3648 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/PKG-INFO
--rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/setup.cfg
--rw-rw-rw-   0        0        0      736 2024-04-16 02:16:13.000000 wxauto-3.9.8.15.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto/
--rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/color.py
--rw-rw-rw-   0        0        0    23156 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/languages.py
--rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.2/wxauto/utils.py
--rw-rw-rw-   0        0        0    23945 2024-04-16 02:16:44.000000 wxauto-3.9.8.15.2/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3648 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 07:35:38.000000 wxauto-3.9.8.15.2/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/
+-rw-rw-rw-   0        0        0     3648 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/setup.cfg
+-rw-rw-rw-   0        0        0      736 2024-04-21 11:48:17.000000 wxauto-3.9.8.15.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto/
+-rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.3/wxauto/__init__.py
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.3/wxauto/color.py
+-rw-rw-rw-   0        0        0    24466 2024-04-21 11:27:55.000000 wxauto-3.9.8.15.3/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.3/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.3/wxauto/languages.py
+-rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.3/wxauto/utils.py
+-rw-rw-rw-   0        0        0    26523 2024-04-21 11:48:31.000000 wxauto-3.9.8.15.3/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3648 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-21 11:49:24.000000 wxauto-3.9.8.15.3/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.2/PKG-INFO` & `wxauto-3.9.8.15.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.2
+Version: 3.9.8.15.3
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

### Comparing `wxauto-3.9.8.15.2/README.md` & `wxauto-3.9.8.15.3/README.md`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.2/setup.py` & `wxauto-3.9.8.15.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.2',
+    version='3.9.8.15.3',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `wxauto-3.9.8.15.2/wxauto/color.py` & `wxauto-3.9.8.15.3/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.2/wxauto/elements.py` & `wxauto-3.9.8.15.3/wxauto/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,24 +122,57 @@
     def _show(self):
         self.HWND = FindWindow(name=self.who, classname='ChatWnd')
         win32gui.ShowWindow(self.HWND, 1)
         win32gui.SetWindowPos(self.HWND, -1, 0, 0, 0, 0, 3)
         win32gui.SetWindowPos(self.HWND, -2, 0, 0, 0, 0, 3)
         self.UiaAPI.SwitchToThisWindow()
 
-    def SendMsg(self, msg):
+    def AtAll(self, msg=None):
+        """@所有人
+        
+        Args:
+            msg (str, optional): 要发送的文本消息
+        """
+        self._show()
+        if not self.editbox.HasKeyboardFocus:
+            self.editbox.Click(simulateMove=False)
+
+        self.editbox.SendKeys('@')
+        atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
+        if atwnd.Exists(maxSearchSeconds=0.1):
+            atwnd.ListItemControl(Name='所有人').Click(simulateMove=False)
+            if msg:
+                if not msg.startswith('\n'):
+                    msg = '\n' + msg
+                self.SendMsg(msg)
+            else:
+                self.editbox.SendKeys('{Enter}')
+
+    def SendMsg(self, msg, at=None):
         """发送文本消息
 
         Args:
             msg (str): 要发送的文本消息
+            at (str|list, optional): 要@的人，可以是一个人或多个人，格式为str或list，例如："张三"或["张三", "李四"]
         """
         self._show()
         if not self.editbox.HasKeyboardFocus:
             self.editbox.Click(simulateMove=False)
 
+        if at:
+            if isinstance(at, str):
+                at = [at]
+            for i in at:
+                self.editbox.SendKeys('@'+i)
+                atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
+                if atwnd.Exists(maxSearchSeconds=0.1):
+                    atwnd.SendKeys('{ENTER}')
+                    if msg and not msg.startswith('\n'):
+                        msg = '\n' + msg
+
         t0 = time.time()
         while True:
             if time.time() - t0 > 10:
                 raise TimeoutError(f'发送消息超时 --> {self.who} - {msg}')
             SetClipboardText(msg)
             self.editbox.SendKeys('{Ctrl}v')
             if self.editbox.GetValuePattern().Value:
```

### Comparing `wxauto-3.9.8.15.2/wxauto/languages.py` & `wxauto-3.9.8.15.3/wxauto/languages.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.2/wxauto/utils.py` & `wxauto-3.9.8.15.3/wxauto/utils.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.2/wxauto/wxauto.py` & `wxauto-3.9.8.15.3/wxauto/wxauto.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Cluic
-Update: 2024-03-21
-Version: 3.9.8.15
+Update: 2024-04-21
+Version: 3.9.8.15.3
 """
 
 import uiautomation as uia
 from .languages import *
 from .utils import *
 from .elements import *
 from .errors import *
@@ -217,27 +217,65 @@
                 raise TargetNotFoundError(f'未查询到目标：{who}')
             elif notfound == 'ignore':
                 return None
         chatname = firstresult.Name
         firstresult.Click(simulateMove=False)
         return chatname
     
-    def SendMsg(self, msg, who=None, clear=True):
+    def AtAll(self, msg=None, who=None):
+        """@所有人
+        
+        Args:
+            who (str, optional): 要发送给谁，如果为None，则发送到当前聊天页面。  *最好完整匹配，优先使用备注
+            msg (str, optional): 要发送的文本消息
+        """
+        if FindWindow(name=who, classname='ChatWnd'):
+            chat = ChatWnd(who, self.language)
+            chat.AtAll(msg)
+            return None
+        
+        self._show()
+        if who:
+            try:
+                editbox = self.ChatBox.EditControl(searchDepth=10)
+                if who in self.CurrentChat() and who in editbox.Name:
+                    pass
+                else:
+                    self.ChatWith(who)
+                    editbox = self.ChatBox.EditControl(Name=who, searchDepth=10)
+            except:
+                self.ChatWith(who)
+                editbox = self.ChatBox.EditControl(Name=who, searchDepth=10)
+        else:
+            editbox = self.ChatBox.EditControl(searchDepth=10)
+        editbox.SendKeys('@')
+        atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
+        if atwnd.Exists(maxSearchSeconds=0.1):
+            atwnd.ListItemControl(Name='所有人').Click(simulateMove=False)
+            if msg:
+                if not msg.startswith('\n'):
+                    msg = '\n' + msg
+                self.SendMsg(msg, who=who, clear=False)
+            else:
+                editbox.SendKeys('{Enter}')
+
+    def SendMsg(self, msg, who=None, clear=True, at=None):
         """发送文本消息
 
         Args:
             msg (str): 要发送的文本消息
             who (str): 要发送给谁，如果为None，则发送到当前聊天页面。  *最好完整匹配，优先使用备注
             clear (bool, optional): 是否清除原本的内容，
+            at (str|list, optional): 要@的人，可以是一个人或多个人，格式为str或list，例如："张三"或["张三", "李四"]
         """
-        if who in self.listen:
-            chat = self.listen[who]
-            chat.SendMsg(msg)
+        if FindWindow(name=who, classname='ChatWnd'):
+            chat = ChatWnd(who, self.language)
+            chat.SendMsg(msg, at=at)
             return None
-        if not msg:
+        if not msg and not at:
             return None
         if who:
             try:
                 editbox = self.ChatBox.EditControl(searchDepth=10)
                 if who in self.CurrentChat() and who in editbox.Name:
                     pass
                 else:
@@ -250,36 +288,48 @@
             editbox = self.ChatBox.EditControl(searchDepth=10)
         if clear:
             editbox.SendKeys('{Ctrl}a', waitTime=0)
         self._show()
         if not editbox.HasKeyboardFocus:
             editbox.Click(simulateMove=False)
         
-        t0 = time.time()
-        while True:
-            if time.time() - t0 > 10:
-                raise TimeoutError(f'发送消息超时 --> {editbox.Name} - {msg}')
-            SetClipboardText(msg)
-            editbox.SendKeys('{Ctrl}v')
-            if editbox.GetValuePattern().Value:
-                break
+        if at:
+            if isinstance(at, str):
+                at = [at]
+            for i in at:
+                editbox.SendKeys('@'+i)
+                atwnd = self.UiaAPI.PaneControl(ClassName='ChatContactMenu')
+                if atwnd.Exists(maxSearchSeconds=0.1):
+                    atwnd.SendKeys('{ENTER}')
+                    if msg and not msg.startswith('\n'):
+                        msg = '\n' + msg
+
+        if msg:
+            t0 = time.time()
+            while True:
+                if time.time() - t0 > 10:
+                    raise TimeoutError(f'发送消息超时 --> {editbox.Name} - {msg}')
+                SetClipboardText(msg)
+                editbox.SendKeys('{Ctrl}v')
+                if editbox.GetValuePattern().Value:
+                    break
         editbox.SendKeys('{Enter}')
         
     def SendFiles(self, filepath, who=None):
         """向当前聊天窗口发送文件
         
         Args:
             filepath (str|list): 要复制文件的绝对路径  
             who (str): 要发送给谁，如果为None，则发送到当前聊天页面。  *最好完整匹配，优先使用备注
             
         Returns:
             bool: 是否成功发送文件
         """
-        if who in self.listen:
-            chat = self.listen[who]
+        if FindWindow(name=who, classname='ChatWnd'):
+            chat = ChatWnd(who, self.language)
             chat.SendFiles(filepath)
             return None
         filelist = []
         if isinstance(filepath, str):
             if not os.path.exists(filepath):
                 Warnings.lightred(f'未找到文件：{filepath}，无法成功发送', stacklevel=2)
                 return False
@@ -493,14 +543,25 @@
         if keywords:
             contactwnd.Search(keywords)
         friends = contactwnd.GetAllFriends()
         contactwnd.Close()
         self.SwitchToChat()
         return friends
     
+    def GetAllListenChat(self):
+        """获取所有监听对象"""
+        return self.listen
+    
+    def RemoveListenChat(self, who):
+        """移除监听对象"""
+        if who in self.listen:
+            del self.listen[who]
+        else:
+            Warnings.lightred(f'未找到监听对象：{who}', stacklevel=2)
+    
 class WeChatFiles:
     def __init__(self, language='cn') -> None:
         self.language = language
         self.api = uia.WindowControl(ClassName='FileListMgrWnd', searchDepth=1)
         MainControl3 = [i for i in self.api.GetChildren() if not i.ClassName][0]
         self.FileBox ,self.Search ,self.SessionBox = MainControl3.GetChildren()
```

### Comparing `wxauto-3.9.8.15.2/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.3/wxauto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.2
+Version: 3.9.8.15.3
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

