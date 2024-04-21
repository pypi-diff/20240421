# Comparing `tmp/drawdraw-0.0.6-py3-none-any.whl.zip` & `tmp/drawdraw-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1894 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1148 b- defN 24-Apr-21 09:44 grcalc/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 09:48 drawdraw-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 09:48 drawdraw-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 09:48 drawdraw-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 09:48 drawdraw-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 24-Apr-21 09:48 drawdraw-0.0.6.dist-info/RECORD
-6 files, 1907 bytes uncompressed, 1062 bytes compressed:  44.3%
+Zip file size: 1589 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      415 b- defN 24-Apr-21 10:02 grcalc/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      456 b- defN 24-Apr-21 10:02 drawdraw-0.0.7.dist-info/RECORD
+6 files, 1173 bytes uncompressed, 757 bytes compressed:  35.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: grcalc/app.py
 Comment: 
 
-Filename: drawdraw-0.0.6.dist-info/LICENSE
+Filename: drawdraw-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: drawdraw-0.0.6.dist-info/METADATA
+Filename: drawdraw-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: drawdraw-0.0.6.dist-info/WHEEL
+Filename: drawdraw-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: drawdraw-0.0.6.dist-info/top_level.txt
+Filename: drawdraw-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: drawdraw-0.0.6.dist-info/RECORD
+Filename: drawdraw-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grcalc/app.py

```diff
@@ -1,33 +1,19 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 def scatter_plot(x_data,y_data,x_label='', y_label='', title=''):
-   
-    # 사용자로부터 데이터 입력 받기
-    x_values = input("x값을 입력해주세요(값 사이에 ,를 넣어주세요): ").split(',')
-    y_values = input("y값을 입력해주세요(값 사이에 ,를 넣어주세요): ").split(',')
-    x_data = [float(x.strip()) for x in x_values]
-    y_data = [float(y.strip()) for y in y_values]
     
     # scatter plot 그리기
     plt.scatter(x_data, y_data)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
     plt.title(title)
     plt.show()
 
 def box_plot(data,labels=None, title=''):
     
-    # 사용자로부터 데이터 입력 받기
-    num_datasets = int(input("boxplot을 위한 데이터셋의 수를 입력하세요: "))
-    data = []
-    for i in range(num_datasets):
-        dataset = input(f"쉼표로 구분하여 데이터셋 {i+1} 을 입력하세요: ").split(',')
-        dataset = [float(d.strip()) for d in dataset]
-        data.append(dataset)
-    
     # box plot 그리기
     plt.boxplot(data, labels=labels)
     plt.title(title)
     plt.show()
```

