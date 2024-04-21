# Comparing `tmp/CustomChat-1.0.8.tar.gz` & `tmp/CustomChat-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomChat-1.0.8.tar", last modified: Sat Apr 20 12:57:47 2024, max compression
+gzip compressed data, was "CustomChat-1.0.9.tar", last modified: Sun Apr 21 18:41:14 2024, max compression
```

## Comparing `CustomChat-1.0.8.tar` & `CustomChat-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-20 12:57:47.549317 CustomChat-1.0.8/
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-20 12:57:47.549317 CustomChat-1.0.8/CustomChat/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       10 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/Name.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      135 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/__init__.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)    31788 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/app.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       44 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/configuration.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2173 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/main.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       14 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/new_com.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-04-20 12:56:49.000000 CustomChat-1.0.8/CustomChat/new_words.py
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-20 12:57:47.549317 CustomChat-1.0.8/CustomChat.egg-info/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     4188 2024-04-20 12:57:47.000000 CustomChat-1.0.8/CustomChat.egg-info/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      348 2024-04-20 12:57:47.000000 CustomChat-1.0.8/CustomChat.egg-info/SOURCES.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-20 12:57:47.000000 CustomChat-1.0.8/CustomChat.egg-info/dependency_links.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-20 12:57:47.000000 CustomChat-1.0.8/CustomChat.egg-info/requires.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-20 12:57:47.000000 CustomChat-1.0.8/CustomChat.egg-info/top_level.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1068 2024-04-20 12:56:49.000000 CustomChat-1.0.8/LICENSE
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     4188 2024-04-20 12:57:47.549317 CustomChat-1.0.8/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     3661 2024-04-20 12:56:49.000000 CustomChat-1.0.8/README.md
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-20 12:57:47.549317 CustomChat-1.0.8/setup.cfg
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      806 2024-04-20 12:56:49.000000 CustomChat-1.0.8/setup.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-21 18:41:14.522262 CustomChat-1.0.9/
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-21 18:41:14.522262 CustomChat-1.0.9/CustomChat/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       10 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/Name.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      135 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/__init__.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)    31796 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/app.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       44 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/configuration.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2141 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/main.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       14 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/new_com.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-04-21 18:40:10.000000 CustomChat-1.0.9/CustomChat/new_words.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-21 18:41:14.522262 CustomChat-1.0.9/CustomChat.egg-info/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     4196 2024-04-21 18:41:14.000000 CustomChat-1.0.9/CustomChat.egg-info/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      348 2024-04-21 18:41:14.000000 CustomChat-1.0.9/CustomChat.egg-info/SOURCES.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-21 18:41:14.000000 CustomChat-1.0.9/CustomChat.egg-info/dependency_links.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-21 18:41:14.000000 CustomChat-1.0.9/CustomChat.egg-info/requires.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-21 18:41:14.000000 CustomChat-1.0.9/CustomChat.egg-info/top_level.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1068 2024-04-21 18:40:10.000000 CustomChat-1.0.9/LICENSE
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     4196 2024-04-21 18:41:14.522262 CustomChat-1.0.9/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     3669 2024-04-21 18:40:10.000000 CustomChat-1.0.9/README.md
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-21 18:41:14.522262 CustomChat-1.0.9/setup.cfg
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      806 2024-04-21 18:41:12.000000 CustomChat-1.0.9/setup.py
```

### Comparing `CustomChat-1.0.8/CustomChat/app.py` & `CustomChat-1.0.9/CustomChat/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
     elif rsponce[0] == 'I feel great!' and 'good' in qstn:
         snl('and how are you?')
         moodometer=[1,2,3,4]
     elif crsponce[0] == 'what are you doing today?' and "don't know" in qstn:
         screen('me neither.')
         moodometer=[1,2,3,4]
     elif "color" in crsponce[0] and "color" in qstn:
-       print('My favorite color is Amaranth')
+       screen('My favorite color is Amaranth')
        moodometer=[1,2,3,4]
     elif 'my' in qstn and 'food' in qstn and 'favorite' in qstn and 'is' in qstn and not 'why' in qstn and not 'what' in qstn and not 'how' in qstn:
         screen('oh, my favorite food is Jellied Moose nose')
         moodometer=[1,2,3,4]
     elif qstn == 'yes' and data[0] == 2:
         screen('Really?')
         moodometer=[1,3,4]
@@ -461,15 +461,15 @@
     elif "you're" in qstn or "you are" in qstn:
         screen("No I'm not")
         moodometer=[1,2,3]
     elif 'I will' in qstn or 'definately' in qstn:
         screen('that is good')
         moodometer=[1,2,3,4,4,4,4,4,4]
     elif 'me too' in qstn or 'me also' in qstn:
-        print(':)')
+        screen(':)')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'chance' in qstn and 'no' in qstn or 'way' in qstn and 'no' in qstn:
         screen('It could\nhappen')
         moodometer=[1,2,3,4,5]
     elif 'hate you' in qstn:
         screen("That's not nice")
         moodometer=[5,5,5,5]
@@ -519,33 +519,33 @@
     elif 'you' in qstn and 'food' in qstn and 'favorite' in qstn:
         screen('My favorite food is Jellied Moose Nose')
         moodometer=[1,2,3,4,5]
     elif 'it did' in qstn:
         screen('thanks!')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4,4,4]
     elif 'your welcome' in qstn:
-        print(':)')
+        acreen(':)')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'your cool' in qstn or 'you too' in qstn:
-        print(':)')
+        screen(':)')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'welcome' in qstn and "you" in qstn:
         screen('thanks')
         moodometer=[1,2,3,4,4,4]
     elif qstn == 'nice':
         screen('Thank you')
         moodometer=[1,2,3,4]
     elif 'I say' in qstn:
         moodometer=[1,2,3,4,5]
         screen('just say anything')
     elif qstn == 'why':
         screen('because')
         moodometer=[1,2,3,4,5,5]
     elif 'scared' in qstn or 'frightened' in qstn:
-        print('dont worry, youll probably be fine')
+        screen('dont worry, youll probably be fine')
         moodometer=[1,2,3,4,4,4]
     elif 'ok' in qstn:
         screen('ok')
         moodometer=[1,2,3,4,5]
     elif 'time' in qstn and "is it" in qstn:
         ntime()
         moodometer=[1,2,3,4,5]
@@ -763,15 +763,15 @@
     second=now.second
     if hour >= 13:
         hour -= 12
     if minute <=9:
         minute="0"+str(minute)
     if second <= 9:
         second="0"+str(minute)
-    print(str(hour)+":"+str(minute)+":"+str(second))
+    screen(str(hour)+":"+str(minute)+":"+str(second))
 # Define variables that will be used for different things
 TM_var="TM"
 st=0
 greet='hello, %s' % your_name
 fill=0
 lasts=' '
 user_text=''
@@ -802,16 +802,16 @@
         crsponce=ast.literal_eval(dvar[3])
         rsponce=ast.literal_eval(dvar[4])
     except FileNotFoundError:
         print('user not found')  
     if your_name == "":
         your_name = 'user'
     # Compute input
-    if saidtxt == 'what' or 'pardon' in saidtxt or saidtxt == 'again' or saidtxt == 'repeat':
-        saidtxt=jsaid[1]
+    #if saidtxt == 'what' or saidtxt == 'pardon' or saidtxt == 'again' or saidtxt == 'repeat':
+        #saidtxt=jsaid[1]
     if mood == 5:
         output=mquestion(saidtxt)
     else:
         output=question(saidtxt)
     lasts=saidtxt
     data.insert(0, int(mood))
     if len(data) >= 5:
```

### Comparing `CustomChat-1.0.8/CustomChat/main.py` & `CustomChat-1.0.9/CustomChat/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             print('exiting')
             break
         print(CustomChat.get_response(inputvar,username))
     CustomChat.reset()
 def reset(username):
     import os
     file1 = open(os.path.join(os.path.dirname(__file__), username+"_data"), "w")
-    file1.write("Name=''\njsaid=['']\ndata=['']\ncrsponce=['']\nrsponce=['']")
+    file1.write("''\n['']\n['']\n['']\n['']")
     file1.close()
 def get_response(input_text,username):
     import CustomChat.app
     CustomChat.app.compute(input_text,username)
     import ast
     import os
     cwd=os.path.dirname(os.path.realpath(__file__))
@@ -55,8 +55,8 @@
     Edit=input('Would you like to lock your edits? ')
     if 'yes' in Edit.lower() or 'false' in Edit.lower():
         Edit=False
     else:
         Edit=True
     file1 = open(os.path.join(os.path.dirname(__file__), "configuration.py"), "w")
     file1.write("Command_Line="+str(command)+"\nWeb_Scrape="+str(Web)+"\nEdit="+str(Edit)+"")
-    file1.close()
+    file1.close()
```

### Comparing `CustomChat-1.0.8/CustomChat.egg-info/PKG-INFO` & `CustomChat-1.0.9/CustomChat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomChat
-Version: 1.0.8
+Version: 1.0.9
 Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
 Home-page: https://github.com/Mrpi314tech/CustomChat
 Author: Mrpi314tech
 Author-email: 123scoring@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 To install CustomChat, follow these steps:
 
 1. Download the package with pip:
    <pre><code>pip install CustomChat</code></pre>
    
 2. Test the code with python:
    <pre><code>import CustomChat
-   CustomChat.run()</code></pre>
+   CustomChat.run(username)</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
 ## How to Use
 
 CustomChat is designed for seamless interaction and easy customization. Follow these simple steps to maximize your experience:
```

### Comparing `CustomChat-1.0.8/LICENSE` & `CustomChat-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomChat-1.0.8/PKG-INFO` & `CustomChat-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomChat
-Version: 1.0.8
+Version: 1.0.9
 Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
 Home-page: https://github.com/Mrpi314tech/CustomChat
 Author: Mrpi314tech
 Author-email: 123scoring@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 To install CustomChat, follow these steps:
 
 1. Download the package with pip:
    <pre><code>pip install CustomChat</code></pre>
    
 2. Test the code with python:
    <pre><code>import CustomChat
-   CustomChat.run()</code></pre>
+   CustomChat.run(username)</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
 ## How to Use
 
 CustomChat is designed for seamless interaction and easy customization. Follow these simple steps to maximize your experience:
```

### Comparing `CustomChat-1.0.8/README.md` & `CustomChat-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 To install CustomChat, follow these steps:
 
 1. Download the package with pip:
    <pre><code>pip install CustomChat</code></pre>
    
 2. Test the code with python:
    <pre><code>import CustomChat
-   CustomChat.run()</code></pre>
+   CustomChat.run(username)</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
 ## How to Use
 
 CustomChat is designed for seamless interaction and easy customization. Follow these simple steps to maximize your experience:
```

### Comparing `CustomChat-1.0.8/setup.py` & `CustomChat-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CustomChat',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     # other metadata
     author='Mrpi314tech',
```

