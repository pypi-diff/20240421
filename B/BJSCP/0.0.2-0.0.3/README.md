# Comparing `tmp/BJSCP-0.0.2-py3-none-any.whl.zip` & `tmp/BJSCP-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4956 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     4785 b- defN 24-Apr-20 08:46 BJSCP/CP.py
--rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-20 10:19 BJSCP/__init__.py
+Zip file size: 5308 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     5677 b- defN 24-Apr-21 08:27 BJSCP/CP.py
+-rw-rw-rw-  2.0 fat      172 b- defN 24-Apr-21 08:27 BJSCP/__init__.py
 -rw-rw-rw-  2.0 fat     4785 b- defN 24-Apr-20 08:46 BJSCP/build/lib/CP.py
--rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-20 10:20 BJSCP-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      539 b- defN 24-Apr-20 10:20 BJSCP-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 10:20 BJSCP-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-20 10:20 BJSCP-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      593 b- defN 24-Apr-20 10:20 BJSCP-0.0.2.dist-info/RECORD
-8 files, 12027 bytes uncompressed, 3930 bytes compressed:  67.3%
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-21 08:29 BJSCP-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      539 b- defN 24-Apr-21 08:29 BJSCP-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 08:29 BJSCP-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-21 08:29 BJSCP-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      593 b- defN 24-Apr-21 08:29 BJSCP-0.0.3.dist-info/RECORD
+8 files, 12950 bytes uncompressed, 4282 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: BJSCP/__init__.py
 Comment: 
 
 Filename: BJSCP/build/lib/CP.py
 Comment: 
 
-Filename: BJSCP-0.0.2.dist-info/LICENSE
+Filename: BJSCP-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: BJSCP-0.0.2.dist-info/METADATA
+Filename: BJSCP-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: BJSCP-0.0.2.dist-info/WHEEL
+Filename: BJSCP-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: BJSCP-0.0.2.dist-info/top_level.txt
+Filename: BJSCP-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: BJSCP-0.0.2.dist-info/RECORD
+Filename: BJSCP-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BJSCP/CP.py

```diff
@@ -133,7 +133,38 @@
     if ioPath is None:
         ioPath = os.path.dirname(filename)
 
     for file in os.listdir(ioPath):
         if re.match("\\w+\\."+__in_ext__, file):
             ioFile = ioPath + '/' + dropExtension(file, "." + __in_ext__)
             test(filename, ioFileName=ioFile, timeout=timeout, verbose=verbose)
+
+
+def makeSampleFile(filename: str, text: str):
+    fout = open(filename, "w")
+    fout.write(text)
+    fout.close()
+
+
+def loadSample(verbose: bool = True):
+    dirName = "SampleData"
+    os.makedirs(dirName, exist_ok=True)
+
+    # source file
+    makeSampleFile(dirName + "/test.py", """
+a = int(input())
+b = int(input())
+
+print(f"a + b = {a + b}")
+    """)
+    # test file 0: expected pass
+    makeSampleFile(dirName + "/test0.in", "3\n4")
+    makeSampleFile(dirName + "/test0.ans", "a + b = 7")
+    # test file 1: expected fail
+    makeSampleFile(dirName + "/test1.in", "1\n1")
+    makeSampleFile(dirName + "/test1.ans", "a + b = 5")
+    # test file 2: expected pass
+    makeSampleFile(dirName + "/test2.in", "2\n1")
+    makeSampleFile(dirName + "/test2.ans", "a + b = 3")
+
+    if(verbose):
+        print("SampleData가 성공적으로 생성되었습니다.")
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## BJSCP/__init__.py

```diff
@@ -1,4 +1,5 @@
 from BJSCP.CP import test, testAll, execute, executeAll
 from BJSCP.CP import __in_ext__, __out_ext__, __ans_ext__
+from BJSCP.CP import loadSample
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `BJSCP-0.0.2.dist-info/LICENSE` & `BJSCP-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `BJSCP-0.0.2.dist-info/METADATA` & `BJSCP-0.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: BJSCP
-Version: 0.0.2
+Version: 0.0.3
 Summary: Helper for competitive programming
 Home-page: https://github.com/hashilyze/CompetitiveProgramming
 Download-URL: https://github.com/hashilyze/CompetitiveProgramming
 Author: JUNSU BAE
-Author-email: hashilyze@gmail.com
+Author-email: jsbae1023@gmail.com
 Keywords: BJS,CP,BJSCP,Competitive,CompetitiveProgramming
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
```

