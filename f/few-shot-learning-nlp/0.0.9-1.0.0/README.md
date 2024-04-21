# Comparing `tmp/few_shot_learning_nlp-0.0.9.tar.gz` & `tmp/few_shot_learning_nlp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "few_shot_learning_nlp-0.0.9.tar", last modified: Sat Apr 20 14:37:10 2024, max compression
+gzip compressed data, was "few_shot_learning_nlp-1.0.0.tar", last modified: Sun Apr 21 15:44:05 2024, max compression
```

## Comparing `few_shot_learning_nlp-0.0.9.tar` & `few_shot_learning_nlp-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.546561 few_shot_learning_nlp-0.0.9/
--rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.9/LICENSE
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:37:10.545556 few_shot_learning_nlp-0.0.9/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)       23 2024-04-20 13:01:16.000000 few_shot_learning_nlp-0.0.9/README.md
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.518555 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/__init__.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.532561 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     8311 2024-04-20 13:32:48.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFit.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)     3454 2024-04-20 13:35:48.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:08:53.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/__init__.py
--rw-r--r--   0 pedro.silva (10822) users    (30000)     3163 2024-04-20 14:34:21.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/utils.py
-drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:37:10.534560 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/
--rw-r--r--   0 pedro.silva (10822) users    (30000)     5735 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/PKG-INFO
--rw-r--r--   0 pedro.silva (10822) users    (30000)      498 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)     2914 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/requires.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-20 14:37:10.000000 few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/top_level.txt
--rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-20 14:37:10.547558 few_shot_learning_nlp-0.0.9/setup.cfg
--rw-r--r--   0 pedro.silva (10822) users    (30000)      721 2024-04-20 14:37:02.000000 few_shot_learning_nlp-0.0.9/setup.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-21 15:44:05.245327 few_shot_learning_nlp-1.0.0/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    35149 2024-04-20 13:01:16.000000 few_shot_learning_nlp-1.0.0/LICENSE
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    10137 2024-04-21 15:44:05.243328 few_shot_learning_nlp-1.0.0/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     4471 2024-04-21 15:42:32.000000 few_shot_learning_nlp-1.0.0/README.md
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-21 15:44:05.201369 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 13:54:41.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/__init__.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-21 15:44:05.220339 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 16:48:24.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/__init__.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     6644 2024-04-21 15:12:10.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/bio_technique.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     5408 2024-04-20 17:03:37.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/bio_technique_dataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     7593 2024-04-20 17:01:40.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/image_dataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     8877 2024-04-21 09:08:34.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_ner_image_documents/splitter.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-21 15:44:05.230331 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        0 2024-04-20 14:08:53.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/__init__.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    11032 2024-04-20 15:34:29.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/pattern_exploiting.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2842 2024-04-20 15:29:14.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/pattern_exploiting_dataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    10870 2024-04-20 16:02:24.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/setfit.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     3454 2024-04-20 15:30:22.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/setfit_dataset.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2953 2024-04-20 15:01:10.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/loss.py
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     3156 2024-04-20 14:40:08.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/utils.py
+drwxr-xr-x   0 pedro.silva (10822) users    (30000)        0 2024-04-21 15:44:05.232335 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/
+-rw-r--r--   0 pedro.silva (10822) users    (30000)    10137 2024-04-21 15:44:05.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     1030 2024-04-21 15:44:05.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)        1 2024-04-21 15:44:05.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)     2851 2024-04-21 15:44:05.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/requires.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       22 2024-04-21 15:44:05.000000 few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/top_level.txt
+-rw-r--r--   0 pedro.silva (10822) users    (30000)       38 2024-04-21 15:44:05.245336 few_shot_learning_nlp-1.0.0/setup.cfg
+-rw-r--r--   0 pedro.silva (10822) users    (30000)      799 2024-04-21 15:44:02.000000 few_shot_learning_nlp-1.0.0/setup.py
```

### Comparing `few_shot_learning_nlp-0.0.9/LICENSE` & `few_shot_learning_nlp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFit.py` & `few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/setfit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from sentence_transformers import SentenceTransformer, losses
 import torch
 from tqdm import tqdm
 from torch.utils.data import DataLoader
 from torcheval.metrics.functional import binary_f1_score, multiclass_confusion_matrix, multiclass_f1_score
 from copy import deepcopy
-from typing import List
+from typing import List, Tuple
 from IPython.display import clear_output
+import pandas as pd
 
 class SetFitTrainer():
     def __init__(
         self,
         embedding_model ,
         classifier_model : torch.nn.Module,
-        dataset_name : str,
-        model_name : str,
         num_classes : int,
+        dataset_name : str = None,
+        model_name : str = None,
         device : str ='cuda' ,
     ) -> None:
         self.embedding_model = embedding_model.to(device)
         self.device = device
         self.dataset_name = dataset_name
         self.classifier_model = classifier_model.to(device)
         self.num_classes = num_classes
@@ -87,15 +88,15 @@
                         y_true_val, 
                         torch.tensor([y_true]).to(self.device)
                     ])
             
             conf_matrix= multiclass_confusion_matrix(
                 y_pred_val.to(torch.int64),
                 y_true_val.to(torch.int64),
-                num_classes=self.num_classes
+                num_classes=2
             )
             
             f1 = binary_f1_score(
                 y_pred_val,
                 y_true_val,
             )
             
@@ -233,7 +234,64 @@
 
             clear_output()
             print(f"---------Epoch: {epoch}-----------")
             print(f'f1 score: {f1.item()}')
             print(conf_matrix)
 
         return self.history, self.embedding_model, self.best_clf
+
+    def test(
+        self,
+        test_df: pd.DataFrame,
+        embedding_model: SentenceTransformer = None,
+        clf: torch.nn.Module = None
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Test the performance of the trained models on the provided test dataset.
+
+        Args:
+            test_df (pd.DataFrame): The DataFrame containing the test dataset with 'text' and 'label' columns.
+            embedding_model (SentenceTransformer, optional): The SentenceTransformer model for text embedding. 
+                If None, the best trained embedding model will be used. Defaults to None.
+            clf (torch.nn.Module, optional): The trained classifier model. 
+                If None, the best trained classifier will be used. Defaults to None.
+
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: A tuple containing the true labels and predicted labels for the test dataset.
+
+        Notes:
+            - Ensure that the test dataset DataFrame contains 'text' and 'label' columns representing the text samples and their corresponding labels.
+            - If `embedding_model` is None, the method will use the best trained embedding model stored in the class attribute `best_model`.
+            - If `clf` is None, the method will use the best trained classifier stored in the class attribute `best_clf`.
+            - The method iterates through the test dataset, computes embeddings for each text sample, and predicts the labels using the classifier.
+            - The predicted labels and true labels are returned as torch tensors.
+        """
+        if embedding_model is not None:
+            self.best_model = embedding_model
+
+        if clf is not None:
+            self.best_clf = clf
+
+        y_pred_test = torch.tensor([],device=self.device)
+        y_true_test = torch.tensor([],device=self.device)
+
+
+        for i in tqdm(range(len(test_df['label']))):
+            text = test_df['text'][i]
+
+            with torch.no_grad():
+                embedding = self.best_model.encode(text, convert_to_tensor=True)
+
+                y_pred = self.best_clf(embedding)\
+                    .argmax()
+                
+                y_pred_test = torch.cat([
+                    y_pred_test, 
+                    torch.tensor([y_pred]).to( self.device)
+                ])
+
+                y_true_test = torch.cat([
+                    y_true_test, 
+                    torch.tensor([test_df['label'][i]]).to(self.device)
+                ])
+        
+        return y_true_test, y_pred_test
```

### Comparing `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/fewShotTextClassification/SetFitDataset.py` & `few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/few_shot_text_classification/setfit_dataset.py`

 * *Files identical despite different names*

### Comparing `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp/utils.py` & `few_shot_learning_nlp-1.0.0/few_shot_learning_nlp/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "label" : [],
         "text": []
     }
 
     class_proportion = df['label'].value_counts()/len(df)
 
     # generating train data
-    for label in range(classes):
+    for label in classes:
         n = len(indexes_dict[label])
 
         if isinstance(train_size, int):
             size = int(class_proportion[label] * train_size)
             
         else:
             size = int(train_size * n)
```

### Comparing `few_shot_learning_nlp-0.0.9/few_shot_learning_nlp.egg-info/requires.txt` & `few_shot_learning_nlp-1.0.0/few_shot_learning_nlp.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 filelock==3.12.4
 fonttools==4.42.1
 frozenlist==1.4.0
 fsspec==2023.6.0
 fvcore==0.1.5.post20221221
 greenlet==3.0.1
 grpcio==1.58.0
-gym==0.26.2
-gym-notices==0.0.8
-gymnasium==0.29.1
 h5py==3.10.0
 huggingface-hub==0.20.2
 hydra-core==1.3.2
 idna==3.4
 imageio==2.32.0
 imageio-ffmpeg==0.4.9
 importlib-metadata==6.8.0
@@ -103,15 +100,14 @@
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pyarrow==13.0.0
 pyarrow-hotfix==0.6
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
 pycocotools==2.0.7
-pygame==2.5.2
 Pygments==2.16.1
 pyparsing==3.1.1
 python-dateutil==2.8.2
 pytz==2023.3.post1
 PyYAML==6.0.1
 pyzmq==25.1.1
 regex==2023.8.8
```

### Comparing `few_shot_learning_nlp-0.0.9/setup.py` & `few_shot_learning_nlp-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from requirements import REQUIRED_PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="few-shot-learning-nlp",
-    version="0.0.9",
+    version="1.0.0",
     author="Pedro Silva",
     author_email="pedrolmssilva@gmail.com",
-    description="A small example package",
+    description="This library provides tools and utilities for Few Shot Learning in Natural Language Processing (NLP).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peulsilva/few-shot-learning-nlp",
     packages=setuptools.find_packages(),
     install_requires = REQUIRED_PACKAGES,
     classifiers=[
         "Programming Language :: Python :: 3",
```

