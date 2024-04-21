# Comparing `tmp/drawdraw-0.0.7-py3-none-any.whl.zip` & `tmp/drawdraw-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1589 bytes, number of entries: 6
--rw-r--r--  2.0 unx      415 b- defN 24-Apr-21 10:02 grcalc/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      456 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/RECORD
-6 files, 1173 bytes uncompressed, 757 bytes compressed:  35.5%
+Zip file size: 1882 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1070 b- defN 24-Apr-21 10:18 grcalc/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 10:19 drawdraw-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 10:19 drawdraw-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:19 drawdraw-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 10:19 drawdraw-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      457 b- defN 24-Apr-21 10:19 drawdraw-0.0.8.dist-info/RECORD
+6 files, 1829 bytes uncompressed, 1050 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: grcalc/app.py
 Comment: 
 
-Filename: drawdraw-0.0.7.dist-info/LICENSE
+Filename: drawdraw-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: drawdraw-0.0.7.dist-info/METADATA
+Filename: drawdraw-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: drawdraw-0.0.7.dist-info/WHEEL
+Filename: drawdraw-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: drawdraw-0.0.7.dist-info/top_level.txt
+Filename: drawdraw-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: drawdraw-0.0.7.dist-info/RECORD
+Filename: drawdraw-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grcalc/app.py

```diff
@@ -1,19 +1,37 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
+def getscatter():
+  x_values = input("쉼표를 이용해 x값을 입력해주세요: ").split(',')
+  y_values = input("쉼표를 이용해 y값을 입력해주세요: ").split(',')
+  x_data = [float(x.strip()) for x in x_values]
+  y_data = [float(y.strip()) for y in y_values]
+
+  return x_data,y_data
+
 def scatter_plot(x_data,y_data,x_label='', y_label='', title=''):
     
     # scatter plot 그리기
     plt.scatter(x_data, y_data)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
     plt.title(title)
     plt.show()
 
+def getbox():
+  num_datasets = int(input("상자 그림을 그릴 데이터셋의 개수를 입력하세요: "))
+  data = []
+  for i in range(num_datasets):
+    dataset = input(f"데이터셋{i+1}의 값을 쉼표로 구분하여 입력하세요: ").split(',')
+    dataset = [float(d.strip()) for d in dataset]
+    data.append(dataset)
+
+  return data
+
 def box_plot(data,labels=None, title=''):
     
     # box plot 그리기
     plt.boxplot(data, labels=labels)
     plt.title(title)
     plt.show()
```

