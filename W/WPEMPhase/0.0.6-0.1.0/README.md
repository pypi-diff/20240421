# Comparing `tmp/WPEMPhase-0.0.6.tar.gz` & `tmp/WPEMPhase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPEMPhase-0.0.6.tar", last modified: Sat Apr 13 09:57:00 2024, max compression
+gzip compressed data, was "WPEMPhase-0.1.0.tar", last modified: Sun Apr 21 06:11:18 2024, max compression
```

## Comparing `WPEMPhase-0.0.6.tar` & `WPEMPhase-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:57:00.721643 WPEMPhase-0.0.6/
--rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-13 09:57:00.721430 WPEMPhase-0.0.6/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.0.6/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:57:00.719537 WPEMPhase-0.0.6/WPEMPhase/
--rw-r--r--   0 jacob      (501) staff       (20)    10131 2024-04-13 09:55:59.000000 WPEMPhase-0.0.6/WPEMPhase/CPICANN.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.0.6/WPEMPhase/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:57:00.720268 WPEMPhase-0.0.6/WPEMPhase/config/
--rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.0.6/WPEMPhase/config/strucs.csv
--rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.0.6/WPEMPhase/data_format.py
--rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.0.6/WPEMPhase/model.py
--rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.0.6/WPEMPhase/plot.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:57:00.720146 WPEMPhase-0.0.6/WPEMPhase.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-13 09:57:00.000000 WPEMPhase-0.0.6/WPEMPhase.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      315 2024-04-13 09:57:00.000000 WPEMPhase-0.0.6/WPEMPhase.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-13 09:57:00.000000 WPEMPhase-0.0.6/WPEMPhase.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       48 2024-04-13 09:57:00.000000 WPEMPhase-0.0.6/WPEMPhase.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       10 2024-04-13 09:57:00.000000 WPEMPhase-0.0.6/WPEMPhase.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-13 09:57:00.721689 WPEMPhase-0.0.6/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1179 2024-04-13 09:56:28.000000 WPEMPhase-0.0.6/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.016148 WPEMPhase-0.1.0/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-21 06:11:18.015950 WPEMPhase-0.1.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.1.0/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014078 WPEMPhase-0.1.0/WPEMPhase/
+-rw-r--r--   0 jacob      (501) staff       (20)     9815 2024-04-21 06:10:33.000000 WPEMPhase-0.1.0/WPEMPhase/CPICANN.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.1.0/WPEMPhase/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014806 WPEMPhase-0.1.0/WPEMPhase/config/
+-rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.1.0/WPEMPhase/config/strucs.csv
+-rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.1.0/WPEMPhase/data_format.py
+-rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.1.0/WPEMPhase/model.py
+-rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.1.0/WPEMPhase/plot.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014686 WPEMPhase-0.1.0/WPEMPhase.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      315 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       48 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       10 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-21 06:11:18.016191 WPEMPhase-0.1.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1179 2024-04-21 06:05:17.000000 WPEMPhase-0.1.0/setup.py
```

### Comparing `WPEMPhase-0.0.6/PKG-INFO` & `WPEMPhase-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.0.6
+Version: 0.1.0
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `WPEMPhase-0.0.6/WPEMPhase/CPICANN.py` & `WPEMPhase-0.1.0/WPEMPhase/CPICANN.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,111 @@
-# It is the phase identification module of WPEM.
+# This is the phase identification module of WPEM.
 
 import csv
 import os
 import datetime
 import pandas as pd
 import torch
 import numpy as np
 import sys
 import wget
-from .plot import _run 
+from .plot import _run
 import zipfile
 import pkg_resources
 from .data_format import convert_file
 from .model import CPICANN_main
 from art import text2art
 
-def PhaseIdentifier(FilePath,Task='single-phase',ElementsSystem='',ElementsContained='',ElementsExclude='',Device='cuda:0',):
+
+def PhaseIdentifier(FilePath, Task='single-phase', Model='default',ElementsSystem='', ElementsContained='', Device='cuda:0', ):
     """
     CPICANN : Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 
     Contributors : Shouyang Zhang & Bin Cao
     ================================================================
         Please feel free to open issues in the Github :
         https://github.com/WPEM/CPICANN
-        or 
+        or
         contact Mr.Bin Cao (bcao686@connect.hkust-gz.edu.cn)
-        in case of any problems/comments/suggestions in using the code. 
+        in case of any problems/comments/suggestions in using the code.
     ==================================================================
 
-    :param FilePath 
+    :param FilePath
 
     :param Task, type=str, default='single-phase'
         if Task = 'single-phase', CPICANN executes a single phase identification task
         if Task = 'di-phase', CPICANN executes a dual phase identification task
-    
+
+    :param Model, type=str, default='default'
+        if Model = 'noise_model', CPICANN executes a single phase identification by noise-contained model
+        if Model = 'bca_model', CPICANN executes a single phase identification by background-contained model
+
     :param ElementsSystem, type=str, default=''
         Specifies the elements to be included at least in the prediction, example: 'Fe'.
 
     :param ElementsContained, type=str, default=''
         Specifies the elements to be included, with at least one of them in the prediction, example: 'O_C_S'.
 
-    :param ElementsExclude, type=str, default=''
-        Specifies the elements to be excluded in the prediction, example: 'Fe_O'
-
     :param Device, type=str, default='cuda:0',
         Which device to run the CPICANN, example: 'cuda:0', 'cpu'.
 
     examples:
     from WPEMPhase import CPICANN
     CPICANN.PhaseIdentifier(FilePath='./single-phase',Device='cpu')
     """
-    
+
     extract_to_folder = pkg_resources.get_distribution('WPEMPhase').location
-    loc = os.path.join(extract_to_folder,'WPEMPhase')
-    # supply CIF files 
-    if os.path.isdir(os.path.join(loc,'strucs')) and os.path.isdir(os.path.join(loc,'pretrained')): pass
-    else: 
+    loc = os.path.join(extract_to_folder, 'WPEMPhase')
+    # supply CIF files
+    if os.path.isdir(os.path.join(loc, 'strucs')) and os.path.isdir(os.path.join(loc, 'pretrained')):
+        pass
+    else:
         print("This is the first time CPICANN is being executed on your computer, configuring...")
-        file_url = "https://figshare.com/ndownloader/files/45638907"
+        file_url = "https://figshare.com/ndownloader/files/45772149"
         _dir = os.path.join(loc, 'SystemFiles.zip')
         wget.download(file_url, _dir, bar=bar_progress)
         zipfile.ZipFile(_dir).extractall(loc)
         prefix_dir = os.path.join(loc, 'SystemFiles')
         zipfile.ZipFile(os.path.join(prefix_dir, 'strucs.zip')).extractall(loc)
         zipfile.ZipFile(os.path.join(prefix_dir, 'pretrained.zip')).extractall(loc)
 
-    
     os.makedirs('figs', exist_ok=True)
     now = datetime.datetime.now()
     formatted_date_time = now.strftime('%Y-%m-%d %H:%M:%S')
     print(text2art("CPICANN"))
     print('The phase identification module of WPEM')
     print('URL : https://github.com/WPEM/CPICANN')
-    print('Executed on :',formatted_date_time, ' | Have a great day.')  
-    print('='*80)
+    print('Executed on :', formatted_date_time, ' | Have a great day.')
+    print('=' * 80)
 
     # get annotation data for display purposeys = np.zeros(4500)
     annoMap, elemMap = get_anno_map(loc)
 
     # get specific element setting map
     elem_setting_map = get_elem_setting()
 
     # choose the model to be loaded
     if Task == 'single-phase':
-        load_path = os.path.join(loc,'pretrained','DPID_single-phase.pth') 
+        if Model == 'default':
+            load_path = os.path.join(loc, 'pretrained', 'CPICANN_single-phase.pth')
+        elif Model == 'noise_model':
+            load_path = os.path.join(loc, 'pretrained', 'CPICANN_single-phase_noise3.pth')
+        elif Model == 'bca_model':
+            load_path = os.path.join(loc, 'pretrained', 'CPICANN_single-phase_back3.pth')
     elif Task == 'di-phase':
-        load_path = os.path.join(loc,'pretrained','DPID_di-phase.pth')  
+        load_path = os.path.join(loc, 'pretrained', 'CPICANN_di-phase.pth')
     else:
         raise ValueError('invalid inf_mode: {}'.format(Task))
 
     # load model parameters
     model = CPICANN_main(embed_dim=128, num_classes=23073)
     if Device == 'cpu':
-        loaded = torch.load(load_path,map_location=torch.device('cpu'))
-    else: loaded = torch.load(load_path)
+        loaded = torch.load(load_path, map_location=torch.device('cpu'))
+    else:
+        loaded = torch.load(load_path)
     model.load_state_dict(loaded['model'])
     print('loaded model from {}'.format(load_path))
     if Device != 'cpu':
         model.to(Device)
     model.eval()
 
     # write the inference results to a csv file
@@ -124,16 +132,15 @@
             # use specific element setting
             logits = filter_elem(logits, elemMap, elem_setting)
         except KeyError:
             # use global element setting
             # filter by include elements
             logits = filter_elem(logits, elemMap,
                                  {'include_must': ElementsSystem,
-                                  'include_atLeastOne': ElementsContained,
-                                  'exclude': ElementsExclude})
+                                  'include_atLeastOne': ElementsContained})
 
         predList = []
         if Task == 'single-phase':
             pred = logits.argmax().item()
             info = annoMap[pred]
             predList.append(info)
             conf = torch.nn.functional.softmax(logits, dim=0).max().item()
@@ -147,82 +154,74 @@
             top5 = logits.topk(5)
 
             for i, (pred, conf) in enumerate(zip(top5[1], top5[0])):
                 if i >= 2 and conf < 0.1:
                     break
                 info = annoMap[pred.item()]
                 predList.append(info)
-                print('>>> pred rank {}'.format(i+1))
+                print('>>> pred rank {}'.format(i + 1))
                 print('pred cls_id : {}  confidence : {:.4f}%'.format(pred.item(), conf * 100))
                 print('pred cod_id : {}  formula : {}'.format(int(info[0]), info[2]))
                 print('pred space group No: {}    space group : {}'.format(info[5], info[4]))
-                dataWriter.writerow([FilePath, l, i+1, pred.item(), info[0], info[2], info[5], info[4]])
+                dataWriter.writerow([FilePath, l, i + 1, pred.item(), info[0], info[2], info[5], info[4]])
 
-        _run(l, data, predList,loc)
+        _run(l, data, predList, loc)
 
     dataFile.close()
 
     print('\ninference result saved in {}'.format(resFileName))
     print('inference figures saved at figs/')
     print('THE END')
     return True
 
 
-
 def inference(model, v, device):
     v = v / v.max() * 100
 
     v = torch.tensor(v, dtype=torch.float32).reshape(1, 1, -1)
     if device != 'cpu':
         v = v.to(device)
     with torch.no_grad():
         logits = model(v)
     return logits
 
 
 def filter_elem(logits, elemMap, elem_setting):
     include_must = elem_setting['include_must']
     include_atLeastOne = elem_setting['include_atLeastOne']
-    exclude = elem_setting['exclude']
 
     if include_must != "":
         exclude_index = get_index_by_include(elemMap, include_must)
         logits = filter_by_index(logits, exclude_index)
 
     if include_atLeastOne != "":
         exclude_index = get_index_by_include_atLeastOne(elemMap, include_atLeastOne)
         logits = filter_by_index(logits, exclude_index)
 
-    if exclude != "":
-        exclude_index = get_index_by_exclude(elemMap, exclude)
-        logits = filter_by_index(logits, exclude_index)
-
     return logits
 
 
 def get_anno_map(loc):
-    vs = pd.read_csv(os.path.join(loc,'config','strucs.csv')).values
+    vs = pd.read_csv(os.path.join(loc, 'config', 'strucs.csv')).values
     annos = {}
     elems = pd.DataFrame({'No': vs[:, 1], 'elem': vs[:, 3]})
     for v in vs:
         annos[v[1]] = v
     return annos, elems
 
 
 def get_elem_setting():
     try:
         vs = pd.read_csv('config/elem_setting.csv').values
         elem_setting_map = {}
         for v in vs:
             include_must = "" if str(v[1]) == 'nan' else v[1]
             include_atLeastOne = "" if str(v[2]) == 'nan' else v[2]
-            exclude = "" if str(v[3]) == 'nan' else v[3]
             elem_setting_map[v[0].strip()] = {'include_must': include_must,
-                                              'include_atLeastOne': include_atLeastOne,
-                                              'exclude': exclude}
+                                              'include_atLeastOne': include_atLeastOne}
     except FileNotFoundError:
         elem_setting_map = {}
     return elem_setting_map
 
 
 def get_index_by_include(elemMap, include):
     include = include.split('_')
@@ -252,35 +251,20 @@
                 excludeIndex[i] = 0
                 break
 
     excludeIndex = np.array(excludeIndex).nonzero()[0]
     return excludeIndex
 
 
-def get_index_by_exclude(elemMap, exclude):
-    exclude = set(exclude.split('_'))
-    if len(exclude) == 0:
-        return []
-
-    excludeIndex = [0] * len(elemMap)
-    for i, es in elemMap.values:
-        for e in es.split(' '):
-            if e in exclude:
-                excludeIndex[i] = 1
-                break
-
-    excludeIndex = np.array(excludeIndex).nonzero()[0]
-    return excludeIndex
-
-
 def filter_by_index(logits, index):
     if len(index) == 0:
         return logits
 
     logits[index] = -1e10
     return logits
 
+
 def bar_progress(current, total, width=80):
-  progress_message = "Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
-  # Don't use print() as it will print in new line every time.
-  sys.stdout.write("\r" + progress_message)
-  sys.stdout.flush()
+    progress_message = "Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
+    # Don't use print() as it will print in new line every time.
+    sys.stdout.write("\r" + progress_message)
+    sys.stdout.flush()
```

### Comparing `WPEMPhase-0.0.6/WPEMPhase/config/strucs.csv` & `WPEMPhase-0.1.0/WPEMPhase/config/strucs.csv`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.6/WPEMPhase/data_format.py` & `WPEMPhase-0.1.0/WPEMPhase/data_format.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.6/WPEMPhase/model.py` & `WPEMPhase-0.1.0/WPEMPhase/model.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.6/WPEMPhase/plot.py` & `WPEMPhase-0.1.0/WPEMPhase/plot.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.6/WPEMPhase.egg-info/PKG-INFO` & `WPEMPhase-0.1.0/WPEMPhase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.0.6
+Version: 0.1.0
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `WPEMPhase-0.0.6/setup.py` & `WPEMPhase-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='WPEMPhase',
-    version='0.0.6',
+    version='0.1.0',
     description="Crystallographic Phase Identifier of Convolutional self-Attention Neural Network",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='CaoBin',
     author_email='bcao@shu.edu.com',
     maintainer='CaoBin',
     maintainer_email='binjacobcao@gmail.com',
```

