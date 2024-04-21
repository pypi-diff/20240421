# Comparing `tmp/glook-0.1.2-py3-none-any.whl.zip` & `tmp/glook-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16527 bytes, number of entries: 12
+Zip file size: 16847 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-16 17:28 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 17:22 glook/pages/1_General_Data_Insights.py
 -rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-16 16:59 glook/pages/3_Bivariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7647 b- defN 24-Apr-16 17:15 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     4221 b- defN 24-Apr-16 18:54 glook-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 18:54 glook-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-16 18:54 glook-0.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-16 18:54 glook-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      967 b- defN 24-Apr-16 18:54 glook-0.1.2.dist-info/RECORD
-12 files, 45800 bytes uncompressed, 14901 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     5001 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      967 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/RECORD
+12 files, 46580 bytes uncompressed, 15221 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.1.2.dist-info/METADATA
+Filename: glook-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.1.2.dist-info/WHEEL
+Filename: glook-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.1.2.dist-info/entry_points.txt
+Filename: glook-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.1.2.dist-info/top_level.txt
+Filename: glook-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.1.2.dist-info/RECORD
+Filename: glook-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `glook-0.1.2.dist-info/METADATA` & `glook-0.1.3.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.1.2
+Version: 0.1.3
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
@@ -41,17 +41,42 @@
 
 
 ![G-Look](https://raw.githubusercontent.com/gaurang157/glook/main/assets/pixelcut-export.png)
 # G-Look: Auto EDA
 
 glook is a Python library that provides a graphical user interface (GUI) for Automated Exploratory Data Analysis (Auto EDA). With glook, you can easily visualize and analyze your dataset's characteristics, distributions, and relationships.
 
-## Before Installation
+## ⚠️ **BEFORE INSTALLATION** ⚠️
 
-Before installing glook, it's suggested to create a new Python environment to avoid any potential conflicts with your current environment.
+**Before installing glook, it's strongly recommended to create a new Python environment to avoid potential conflicts with your current environment.**
+
+
+## Creating a New Conda Environment
+
+To create a new conda environment, follow these steps:
+
+1. **Install Conda**:
+   If you don't have conda installed, you can download and install it from the [Anaconda website](https://www.anaconda.com/products/distribution).
+
+2. **Open a Anaconda Pprompt**:
+   Open a Anaconda Pprompt (or Anaconda Terminal) on your system.
+
+3. **Create a New Environment**:
+   To create a new conda environment, use the following command. Replace `my_env_name` with your desired environment name.
+
+```bash
+conda create --name my_env_name python=3.8
+```
+
+4. **Activate the Environment**:
+    After creating the environment, activate it with the following command:
+
+```bash
+conda activate my_env_name
+```
 
 ## Installation
 
 You can install glook using pip:
 
 ```bash
 pip install glook
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `glook-0.1.2.dist-info/RECORD` & `glook-0.1.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 glook/GLook.py,sha256=qNCnTY0f4myhVXkZHf1mMgpN4yfHCaVXq4uz4uC85_s,3200
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
 glook/pages/1_General_Data_Insights.py,sha256=btHs2krtxH-H2MdX_x0hLnp8NR38dYvNnVdnNNjZosc,3698
 glook/pages/2_Univariate_Analysis.py,sha256=iQd1MsSFCdtIFU6coQBN-T9FWTVoVUA_Baf1evwjanA,17728
 glook/pages/3_Bivariate_Analysis.py,sha256=_eUSH35csf_Uljg9HvW7szmfXjrgNwrsVJA0gLMDNEA,7813
 glook/pages/4_Trivariate_Analysis.py,sha256=VPttBFaeegQUdCWH2OodwmX0Vn4B-4bnaLAKZErTgog,7647
-glook-0.1.2.dist-info/METADATA,sha256=BozQbmVpzZ953cbo8DYL2AcJRXIvC9c0PNjn6_uDCoQ,4221
-glook-0.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-0.1.2.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-0.1.2.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-0.1.2.dist-info/RECORD,,
+glook-0.1.3.dist-info/METADATA,sha256=OBUhFKekOcuNdfhovJS8mKTXqQjyOmr8ljN8T8zTkg8,5001
+glook-0.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-0.1.3.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-0.1.3.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-0.1.3.dist-info/RECORD,,
```

