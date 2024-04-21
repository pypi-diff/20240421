# Comparing `tmp/drawdraw-0.1.0-py3-none-any.whl.zip` & `tmp/drawdraw-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1884 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1062 b- defN 24-Apr-21 10:40 grcalc/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 10:41 drawdraw-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 10:41 drawdraw-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:41 drawdraw-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 10:41 drawdraw-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 24-Apr-21 10:41 drawdraw-0.1.0.dist-info/RECORD
-6 files, 1821 bytes uncompressed, 1052 bytes compressed:  42.2%
+Zip file size: 1889 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1098 b- defN 24-Apr-21 12:26 grcalc/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 12:27 drawdraw-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 12:27 drawdraw-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 12:27 drawdraw-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 12:27 drawdraw-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      457 b- defN 24-Apr-21 12:27 drawdraw-0.1.1.dist-info/RECORD
+6 files, 1857 bytes uncompressed, 1057 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: grcalc/app.py
 Comment: 
 
-Filename: drawdraw-0.1.0.dist-info/LICENSE
+Filename: drawdraw-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: drawdraw-0.1.0.dist-info/METADATA
+Filename: drawdraw-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: drawdraw-0.1.0.dist-info/WHEEL
+Filename: drawdraw-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: drawdraw-0.1.0.dist-info/top_level.txt
+Filename: drawdraw-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: drawdraw-0.1.0.dist-info/RECORD
+Filename: drawdraw-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grcalc/app.py

```diff
@@ -1,37 +1,37 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 def getscatter():
-  x_values = input("쉼표를 이용해 x값을 입력해주세요: ").split(',')
-  y_values = input("쉼표를 이용해 y값을 입력해주세요: ").split(',')
-  x_data = [float(x.strip()) for x in x_values]
-  y_data = [float(y.strip()) for y in y_values]
+    x_values = input("쉼표를 이용해 x값을 입력해주세요: ").split(',')
+    y_values = input("쉼표를 이용해 y값을 입력해주세요: ").split(',')
+    x_data = [float(x.strip()) for x in x_values]
+    y_data = [float(y.strip()) for y in y_values]
 
-  return x_data,y_data
+    return x_data, y_data
 
 def scatter_plot(x_data,y_data,x_label='', y_label='', title=''):
 
     # scatter plot 그리기
     plt.scatter(x_data, y_data)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
     plt.title(title)
     plt.show()
 
 def getbox():
-  num_datasets = int(input("상자 그림을 그릴 데이터셋의 개수를 입력하세요: "))
-  data = []
-  for i in range(num_datasets):
-    dataset = input(f"데이터셋{i+1}의 값을 쉼표로 구분하여 입력하세요: ").split(',')
-    dataset = [float(d.strip()) for d in dataset]
-    data.append(dataset)
-
-  return data
+    num_datasets = int(input("상자 그림을 그릴 데이터셋의 개수를 입력하세요: "))
+    data = []
+    for i in range(num_datasets):
+        dataset = input(f"데이터셋 {i+1}의 값을 쉼표로 구분하여 입력하세요: ").split(',')
+        dataset = [float(d.strip()) for d in dataset]
+        data.append(dataset)
 
+    return data
+    
 def box_plot(data,labels=None, title=''):
 
     # box plot 그리기
     plt.boxplot(data, labels=labels)
     plt.title(title)
     plt.show()
```

