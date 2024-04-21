# Comparing `tmp/glook-0.1.3-py3-none-any.whl.zip` & `tmp/glook-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16847 bytes, number of entries: 12
+Zip file size: 17303 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-16 17:28 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 17:22 glook/pages/1_General_Data_Insights.py
 -rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-16 16:59 glook/pages/3_Bivariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7647 b- defN 24-Apr-16 17:15 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     5001 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      967 b- defN 24-Apr-21 08:15 glook-0.1.3.dist-info/RECORD
-12 files, 46580 bytes uncompressed, 15221 bytes compressed:  67.3%
+-rw-rw-rw-  2.0 fat     6311 b- defN 24-Apr-21 09:15 glook-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-21 09:15 glook-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-21 09:15 glook-0.1.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-21 09:15 glook-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      967 b- defN 24-Apr-21 09:15 glook-0.1.4.dist-info/RECORD
+12 files, 47890 bytes uncompressed, 15677 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.1.3.dist-info/METADATA
+Filename: glook-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.1.3.dist-info/WHEEL
+Filename: glook-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.1.3.dist-info/entry_points.txt
+Filename: glook-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.1.3.dist-info/top_level.txt
+Filename: glook-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.1.3.dist-info/RECORD
+Filename: glook-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `glook-0.1.3.dist-info/METADATA` & `glook-0.1.4.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.1.3
+Version: 0.1.4
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
@@ -53,31 +53,53 @@
 ## Creating a New Conda Environment
 
 To create a new conda environment, follow these steps:
 
 1. **Install Conda**:
    If you don't have conda installed, you can download and install it from the [Anaconda website](https://www.anaconda.com/products/distribution).
 
-2. **Open a Anaconda Pprompt**:
-   Open a Anaconda Pprompt (or Anaconda Terminal) on your system.
+2. **Open a Anaconda Prompt**:
+   Open a Anaconda Prompt (or Anaconda Terminal) on your system.
 
 3. **Create a New Environment**:
    To create a new conda environment, use the following command. Replace `my_env_name` with your desired environment name.
-
+- Support Python versions are > 3.8
 ```bash
 conda create --name my_env_name python=3.8
 ```
 
 4. **Activate the Environment**:
     After creating the environment, activate it with the following command:
-
 ```bash
 conda activate my_env_name
 ```
 
+## OR
+## Create a New Virtual Environment with `venv`
+If you prefer using Python's built-in `venv` module, here's how to create a virtual environment:
+
+1. **Check Your Python Installation**:
+   Ensure you have Python installed on your system. You can check by running:
+   - Support Python versions are > 3.8
+```bash
+python --version
+```
+
+2. **Create a Virtual Environment**:
+Use the following command to create a new virtual environment. Replace `my_env_name` with your desired environment name.
+```bash
+python -m venv my_env_name
+```
+
+3. **Activate the Environment**:
+After creating the virtual environment, activate it using the appropriate command for your operating system:
+```bash
+my_env_name\Scripts\activate
+```
+
 ## Installation
 
 You can install glook using pip:
 
 ```bash
 pip install glook
 ```
@@ -88,25 +110,36 @@
 
 ```bash
 glook
 ```
 
 The glook application GUI will launch, allowing you to perform Auto EDA on your dataset interactively.
 
+<img width="960" alt="image" src="https://github.com/gaurang157/glook/assets/148379526/668aaa96-5883-49eb-aa85-4852df92233a">
+
+
 ## Features
 
+- General Data Insights
+      ![image](https://github.com/gaurang157/glook/assets/148379526/468e9ced-c13c-4e5e-b6ab-27bb7a58da33)
+- Correlation Coefficient Heatmap
+      ![image](https://github.com/gaurang157/glook/assets/148379526/228dc42a-61a5-4924-a2ec-3fa9b4c54f75)
+      
+
 ### Univariate Analysis
 - Visualize distributions of individual columns using:
   - Histograms
   - Box plots
   - Q-Q plot
+- Statistical Calculations:
+   ![image](https://github.com/gaurang157/glook/assets/148379526/4d9bb69b-c0f5-4e57-8a42-6de58af9a5e0)
+
 
 
 ### Bivariate Analysis
-- Correlation Plot
 - Explore relationships between two columns using:
   - Scatter plots
   - Line plots
   - Bar plots
   - Histograms
   - Box plots
   - Violin plots
```

## Comparing `glook-0.1.3.dist-info/RECORD` & `glook-0.1.4.dist-info/RECORD`

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
-glook-0.1.3.dist-info/METADATA,sha256=OBUhFKekOcuNdfhovJS8mKTXqQjyOmr8ljN8T8zTkg8,5001
-glook-0.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-0.1.3.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-0.1.3.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-0.1.3.dist-info/RECORD,,
+glook-0.1.4.dist-info/METADATA,sha256=2i7c9OtkH3mHiLpgZuaXl21sfyO0zns-UNtA5V4EwQ8,6311
+glook-0.1.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-0.1.4.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-0.1.4.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-0.1.4.dist-info/RECORD,,
```

