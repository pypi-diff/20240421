# Comparing `tmp/drawdraw-0.0.4-py3-none-any.whl.zip` & `tmp/drawdraw-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1554 bytes, number of entries: 6
--rw-r--r--  2.0 unx      338 b- defN 24-Apr-21 07:37 grcalc/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 07:38 drawdraw-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 07:38 drawdraw-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 07:38 drawdraw-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 07:38 drawdraw-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      456 b- defN 24-Apr-21 07:38 drawdraw-0.0.4.dist-info/RECORD
-6 files, 1096 bytes uncompressed, 722 bytes compressed:  34.1%
+Zip file size: 1891 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-21 09:20 grcalc/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 09:20 drawdraw-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 09:20 drawdraw-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 09:20 drawdraw-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 09:20 drawdraw-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      457 b- defN 24-Apr-21 09:20 drawdraw-0.0.5.dist-info/RECORD
+6 files, 1888 bytes uncompressed, 1059 bytes compressed:  43.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: grcalc/app.py
 Comment: 
 
-Filename: drawdraw-0.0.4.dist-info/LICENSE
+Filename: drawdraw-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: drawdraw-0.0.4.dist-info/METADATA
+Filename: drawdraw-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: drawdraw-0.0.4.dist-info/WHEEL
+Filename: drawdraw-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: drawdraw-0.0.4.dist-info/top_level.txt
+Filename: drawdraw-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: drawdraw-0.0.4.dist-info/RECORD
+Filename: drawdraw-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grcalc/app.py

```diff
@@ -1,15 +1,33 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-def scatter_plot(x_data, y_data, x_label='', y_label='', title=''):
-  plt.scatter(x_data, y_data)
-  plt.xlabel(x_label)
-  plt.ylabel(y_label)
-  plt.title(title)
-  plt.show()
+def scatter_plot(x_label='', y_label='', title=''):
+   
+    # 사용자로부터 데이터 입력 받기
+    x_values = input("x값을 입력해주세요(값 사이에 ,를 넣어주세요): ").split(',')
+    y_values = input("y값을 입력해주세요(값 사이에 ,를 넣어주세요): ").split(',')
+    x_data = [float(x.strip()) for x in x_values]
+    y_data = [float(y.strip()) for y in y_values]
+    
+    # scatter plot 그리기
+    plt.scatter(x_data, y_data)
+    plt.xlabel(x_label)
+    plt.ylabel(y_label)
+    plt.title(title)
+    plt.show()
 
-def box_plot(data, labels=None, title=''):
-  plt.boxplot(data, labels=labels)
-  plt.title(title)
-  plt.show()
+def box_plot(labels=None, title=''):
+    
+    # 사용자로부터 데이터 입력 받기
+    num_datasets = int(input("boxplot을 위한 데이터셋의 수를 입력하세요: "))
+    data = []
+    for i in range(num_datasets):
+        dataset = input(f"쉼표로 구분하여 데이터셋 {i+1} 을 입력하세요: ").split(',')
+        dataset = [float(d.strip()) for d in dataset]
+        data.append(dataset)
+    
+    # box plot 그리기
+    plt.boxplot(data, labels=labels)
+    plt.title(title)
+    plt.show()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

