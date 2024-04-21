# Comparing `tmp/recs-searcher-0.0.8.tar.gz` & `tmp/recs-searcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recs-searcher-0.0.8.tar", last modified: Thu Mar 21 16:39:02 2024, max compression
+gzip compressed data, was "recs-searcher-0.0.9.tar", last modified: Sun Apr 21 15:21:54 2024, max compression
```

## Comparing `recs-searcher-0.0.8.tar` & `recs-searcher-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.112092 recs-searcher-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2019 2024-03-21 16:39:02.111094 recs-searcher-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2024-03-21 10:34:47.000000 recs-searcher-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:01.959094 recs-searcher-0.0.8/recs_searcher/
--rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:01.981092 recs-searcher-0.0.8/recs_searcher/api/
--rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.0.8/recs_searcher/api/__init__.py
--rw-rw-rw-   0        0        0     6652 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/api/api.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:01.998095 recs-searcher-0.0.8/recs_searcher/augmentation/
--rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.0.8/recs_searcher/augmentation/__init__.py
--rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.0.8/recs_searcher/augmentation/_actions.py
--rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.0.8/recs_searcher/augmentation/_base.py
--rw-rw-rw-   0        0        0     3283 2024-03-21 12:34:55.000000 recs-searcher-0.0.8/recs_searcher/augmentation/_char_aug.py
--rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.0.8/recs_searcher/augmentation/_word_aug.py
--rw-rw-rw-   0        0        0    10878 2024-03-21 10:46:13.000000 recs-searcher-0.0.8/recs_searcher/base.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.007093 recs-searcher-0.0.8/recs_searcher/dataset/
--rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/dataset/__init__.py
--rw-rw-rw-   0        0        0     1112 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/dataset/_base.py
--rw-rw-rw-   0        0        0     5723 2024-03-21 15:15:56.000000 recs-searcher-0.0.8/recs_searcher/dataset/_dataframes.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.060093 recs-searcher-0.0.8/recs_searcher/dataset/data/
--rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/__init__.py
--rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/address_krasnoyarsk.csv
--rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/city_russia.csv
--rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/company_russia.csv
--rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/exoplanets.csv
--rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/medical_supplies.csv
--rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/mobile_phones.csv
--rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/russian_dictionary.csv
--rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.0.8/recs_searcher/dataset/data/video_games.csv
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.067095 recs-searcher-0.0.8/recs_searcher/embeddings/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/embeddings/__init__.py
--rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/embeddings/_base.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.075094 recs-searcher-0.0.8/recs_searcher/explain/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/explain/__init__.py
--rw-rw-rw-   0        0        0     2558 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/explain/_base.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.083097 recs-searcher-0.0.8/recs_searcher/preprocessing/
--rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.0.8/recs_searcher/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     5679 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/preprocessing/_base_clear.py
--rw-rw-rw-   0        0        0     2154 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/preprocessing/_base_normalize.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.093093 recs-searcher-0.0.8/recs_searcher/similarity_search/
--rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/similarity_search/__init__.py
--rw-rw-rw-   0        0        0     8924 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/similarity_search/_base.py
--rw-rw-rw-   0        0        0     1528 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/similarity_search/_validate.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.106095 recs-searcher-0.0.8/recs_searcher/utils/
--rw-rw-rw-   0        0        0       96 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/utils/_concat_embeddings.py
--rw-rw-rw-   0        0        0      377 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/utils/_create_date_name.py
--rw-rw-rw-   0        0        0      586 2024-03-13 07:55:35.000000 recs-searcher-0.0.8/recs_searcher/utils/_distances.py
-drwxrwxrwx   0        0        0        0 2024-03-21 16:39:02.110093 recs-searcher-0.0.8/recs_searcher.egg-info/
--rw-rw-rw-   0        0        0     2019 2024-03-21 16:39:01.000000 recs-searcher-0.0.8/recs_searcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1571 2024-03-21 16:39:01.000000 recs-searcher-0.0.8/recs_searcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 16:39:01.000000 recs-searcher-0.0.8/recs_searcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-03-21 16:39:01.000000 recs-searcher-0.0.8/recs_searcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-21 16:39:01.000000 recs-searcher-0.0.8/recs_searcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 16:39:02.114094 recs-searcher-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1060 2024-03-21 16:38:00.000000 recs-searcher-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.797312 recs-searcher-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2020 2024-04-21 15:21:54.785313 recs-searcher-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2024-03-21 10:34:47.000000 recs-searcher-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.120318 recs-searcher-0.0.9/recs_searcher/
+-rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.155314 recs-searcher-0.0.9/recs_searcher/api/
+-rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.0.9/recs_searcher/api/__init__.py
+-rw-rw-rw-   0        0        0    15662 2024-04-14 15:18:10.000000 recs-searcher-0.0.9/recs_searcher/api/api.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.196313 recs-searcher-0.0.9/recs_searcher/augmentation/
+-rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.0.9/recs_searcher/augmentation/__init__.py
+-rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_actions.py
+-rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_base.py
+-rw-rw-rw-   0        0        0     3283 2024-03-21 12:34:55.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_char_aug.py
+-rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_word_aug.py
+-rw-rw-rw-   0        0        0    16750 2024-04-14 14:08:26.000000 recs-searcher-0.0.9/recs_searcher/base.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.246311 recs-searcher-0.0.9/recs_searcher/dataset/
+-rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1112 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/dataset/_base.py
+-rw-rw-rw-   0        0        0     5723 2024-03-21 15:15:56.000000 recs-searcher-0.0.9/recs_searcher/dataset/_dataframes.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.577312 recs-searcher-0.0.9/recs_searcher/dataset/data/
+-rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/__init__.py
+-rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/address_krasnoyarsk.csv
+-rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/city_russia.csv
+-rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/company_russia.csv
+-rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/exoplanets.csv
+-rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/medical_supplies.csv
+-rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/mobile_phones.csv
+-rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/russian_dictionary.csv
+-rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/video_games.csv
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.598311 recs-searcher-0.0.9/recs_searcher/embeddings/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/embeddings/_base.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.615312 recs-searcher-0.0.9/recs_searcher/explain/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/explain/__init__.py
+-rw-rw-rw-   0        0        0     3278 2024-04-14 12:54:59.000000 recs-searcher-0.0.9/recs_searcher/explain/_base.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.651315 recs-searcher-0.0.9/recs_searcher/preprocessing/
+-rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2024-04-14 15:37:15.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/_base_clear.py
+-rw-rw-rw-   0        0        0     2154 2024-04-14 15:38:26.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/_base_normalize.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.674311 recs-searcher-0.0.9/recs_searcher/similarity_search/
+-rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/__init__.py
+-rw-rw-rw-   0        0        0     8170 2024-04-14 15:40:23.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/_base.py
+-rw-rw-rw-   0        0        0     2490 2024-04-14 15:45:59.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/_validate.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.760313 recs-searcher-0.0.9/recs_searcher/utils/
+-rw-rw-rw-   0        0        0       96 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1637 2024-04-14 15:46:47.000000 recs-searcher-0.0.9/recs_searcher/utils/_concat_embeddings.py
+-rw-rw-rw-   0        0        0      729 2024-04-14 15:48:15.000000 recs-searcher-0.0.9/recs_searcher/utils/_create_date_name.py
+-rw-rw-rw-   0        0        0      712 2024-04-14 15:29:21.000000 recs-searcher-0.0.9/recs_searcher/utils/_distances.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.780315 recs-searcher-0.0.9/recs_searcher.egg-info/
+-rw-rw-rw-   0        0        0     2020 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1571 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:21:54.799312 recs-searcher-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2024-04-21 15:21:17.000000 recs-searcher-0.0.9/setup.py
```

### Comparing `recs-searcher-0.0.8/LICENSE` & `recs-searcher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/PKG-INFO` & `recs-searcher-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: recs-searcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Search engine and registry error corrector
 Home-page: https://github.com/sheriff1max/recs-searcher
 Author: sheriff1max
 Author-email: kobelevmaxim48@gmail.com
 Project-URL: Bug tracker, https://github.com/sheriff1max/recs-searcher/issues
-Keywords: python searcher corrector faiss fasttext embeddings
+Keywords: python searcher corrector faiss chroma-bd embeddings
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: chromadb
 Requires-Dist: datasets
```

### Comparing `recs-searcher-0.0.8/README.md` & `recs-searcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/api/api.py` & `recs-searcher-0.0.9/recs_searcher/similarity_search/_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,233 @@
-""" api.py
-Взаимодействие с системой."""
+"""
+Алгоритмы для получения результатов моделей.
+"""
 
-from typing import List, Iterable, Dict, Type, Optional
+from typing import Iterable, List, Literal, Optional, Tuple
+import numpy as np
 
-from ..base import(
-    BaseTransformation,
-    BaseEmbedding,
-    BaseSearch,
-)
-from ..similarity_search import Validate
+from ..utils import create_date_name
+from ..base import BaseSearch, BaseEmbeddingSearch, BaseEmbedding, BaseTransformation
 
-import numpy as np
-import pandas as pd
-from pathlib import Path
-import pickle
-
-import pathlib
-import platform
-if platform.system() == 'Linux':
-    pathlib.WindowsPath = pathlib.PosixPath
+from thefuzz import process
+import faiss
+import chromadb
+from sklearn.neighbors import NearestNeighbors
 
 
-class Pipeline:
-    """Класс полного цикла """
+class TheFuzzSearch(BaseSearch):
+    """Класс поиска наиболее похожих слов в БД
+    с помощью расстояния Ливенштейна.
+    Основано на: https://github.com/seatgeek/thefuzz
+    """
 
     def __init__(
-        self,
-        dataset: Iterable[str],
-        searcher: Type[BaseSearch],
-        preprocessing: Optional[List[BaseTransformation]] = None,
-        model: Optional[BaseEmbedding] = None,
-        verbose: bool = True,
-        **searcher_args,
+            self,
+            original_array: Iterable[str],
+            preprocessing: List[BaseTransformation],
+            clear_array: Optional[Iterable[str]] = None,
     ):
-        self._original_dataset = np.array(dataset)
-        self._preprocessing = preprocessing
-
-        self.__verbose('Data preparation for training has begun...', verbose)
-        self._clear_dataset = self.__clear_dataset(self._original_dataset, self._preprocessing)
-
-        self._model = model
-        self._embedding_database = None
-        # Если True - обучаем модель для создания эмбеддингов.
-        if isinstance(model, BaseEmbedding):
-            self.__verbose('The training of the model has begun...', verbose)
-            self._embedding_database = self.__fit_transform(self._model, self._clear_dataset)
-
-        # Класс поисковика для будущего дообучения.
-        self.__type_searcher = searcher
-        self.__searcher_args = searcher_args
-
-        self._searcher = self.__create_searcher(
-            searcher=self.__type_searcher,
-            model=self._model,
-            embedding_database=self._embedding_database,
-            original_array=self._original_dataset,
-            preprocessing=self._preprocessing,
-            clear_array=self._clear_dataset,
-            searcher_args=searcher_args,
-        )
-        self.__verbose('Pipeline ready!', verbose)
-
-        # Здесь хранится метрика последнего раза валидации.
-        self.score_metrics = None
-
-    def __verbose(self, message: str, verbose: bool) -> None:
-        """"""
-        if verbose:
-            print(message)
+        super().__init__(
+            original_array=original_array,
+            preprocessing=preprocessing,
+            clear_array=clear_array,
+        )
 
-    def __clear_dataset(
+    def _search(
         self,
-        dataset: Iterable[str],
-        preprocessing: List[BaseTransformation],
-    ) -> np.ndarray:
-        """"""
-        for transformation in preprocessing:
-            dataset = transformation.transform(dataset)
-        return np.array(dataset)
+        clear_text: str,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        results = process.extract(clear_text, self._clear_text, limit=k)
 
-    def __fit_transform(
-        self,
-        model: BaseEmbedding,
-        dataset: Iterable[str],
-    ) -> np.ndarray:
-        """"""
-        embedding_database = model.fit_transform(dataset)
-        return embedding_database
+        list_texts = []
+        list_similarity = []
+        for result in results:
+            list_similarity.append(result[1])
 
-    def __create_searcher(
-        self,
-        searcher: Type[BaseSearch],
-        model: Optional[BaseEmbedding],
-        embedding_database: np.ndarray,
-        original_array: Iterable[str],
-        preprocessing: List[BaseTransformation],
-        clear_array: Iterable[str],
-        searcher_args: dict,
-    ) -> BaseSearch:
-        """"""
-        if isinstance(model, BaseEmbedding):
-            return searcher(
-                model=model,
-                embedding_database=embedding_database,
-                original_array=original_array,
-                preprocessing=preprocessing,
-                clear_array=clear_array,
-                **searcher_args,
-            )
-        else:
-            return searcher(
-                original_array=self._original_dataset,
-                preprocessing=preprocessing,
-                clear_array=clear_array,
-            )
+            index = np.where(self._clear_text == result[0])
+            list_texts.append(self._original_array[index][0])
 
-    def get_model(self) -> Optional[BaseEmbedding]:
-        return self._model
+        return list_texts, list_similarity
 
-    def get_preprocessing(self) -> Optional[List[BaseTransformation]]:
-        return self._preprocessing
 
-    def load(self, path_to_filename: str) -> object:
-        """"""
-        self = load_pipeline(path_to_filename)
-        return self
-
-    def save(self, path_folder_save: str, filename: str) -> object:
-        """"""
-        path_folder_save = Path(path_folder_save)
-        if not path_folder_save.exists():
-            path_folder_save.mkdir()
-
-        if '.pkl' not in filename:
-            filename += '.pkl'
-        path = path_folder_save / filename
-
-        with open(path, 'wb') as f:
-            pickle.dump(self, f)
-        return self
+class NearestNeighborsSearch(BaseEmbeddingSearch):
+    """
+    Поиск на основе ближайших соседей.
+    Основа на: https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html#sklearn.neighbors.NearestNeighbors
+    """
 
-    def validate(
-        self,
-        augmentation_transforms: List[BaseTransformation],
-        accuracy_top: List[int] = [1, 5, 10],
-        ascending: bool = True,
-    ) -> Dict[int, float]:
-        """"""
-        score_metrics = Validate(
-            self._searcher,
-            augmentation_transforms,
-            accuracy_top,
-            ascending=ascending,
-        )
-        self.score_metrics = score_metrics
-        return score_metrics
-
-    def search(self, text: str, k: int, ascending: bool = True) -> pd.DataFrame:
-        """"""
-        return self._searcher.search(text, k, ascending=ascending)
+    def __init__(
+            self,
+            model: BaseEmbedding,
+            embedding_database: np.ndarray,
+            original_array: Iterable[str],
+            preprocessing: List[BaseTransformation],
+            clear_array: Optional[Iterable[str]] = None,
+
+            radius: float = 1.0,
+            algorithm: str = 'auto',
+            leaf_size: int = 30,
+            metric: Literal['cosine', 'l1', 'l2', 'minkowski', 'manhattan', 'cosine'] = 'cosine',
+            p: float = 2,
+            metric_params: dict = None,
+            n_jobs: int = None,
+    ):
+        super().__init__(
+            model=model,
+            embedding_database=embedding_database,
+            original_array=original_array,
+            preprocessing=preprocessing,
+            metric=metric,
+            clear_array=clear_array,
+        )
 
-    def fine_tuning(
-        self,
-        dataset: Iterable[str],
-    ) -> object:
-        """Дообучение пайплайна на новых данных."""
-        dataset = np.array(dataset)
-        dataset = np.append(self._original_dataset, dataset)
-        return Pipeline(
-            dataset=dataset,
-            preprocessing=self._preprocessing,
-            model=self._model,
-            searcher=self.__type_searcher,
-            verbose=True,
-            **self.__searcher_args,
+        self._knn = None
+        self._radius = radius
+        self._algorithm = algorithm
+        self._leaf_size = leaf_size
+        self._p = p
+        self._metric_params = metric_params
+        self._n_jobs = n_jobs
+
+    def _search(
+        self,
+        array: np.ndarray,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        if not self._knn or self._knn.n_neighbors != k:
+            self._knn = NearestNeighbors(
+                n_neighbors=k,
+                radius=self._radius,
+                algorithm=self._algorithm,
+                leaf_size=self._leaf_size,
+                metric=self._metric,
+                p=self._p,
+                metric_params=self._metric_params,
+                n_jobs=self._n_jobs,
+            ).fit(self._embedding_database)
+
+        list_similarity, list_texts = self._knn.kneighbors(array)
+        list_similarity = list_similarity[0]
+        list_texts = self._original_array[list_texts[0]]
+        return list_texts, list_similarity
+
+
+class FaissSearch(BaseEmbeddingSearch):
+    """
+    Основано на: https://github.com/facebookresearch/faiss
+    """
+
+    def __init__(
+            self,
+            model: BaseEmbedding,
+            embedding_database: np.ndarray,
+            original_array: Iterable[str],
+            preprocessing: List[BaseTransformation],
+            count_voronoi_cells: Optional[int] = 1,  # > 1 if type_optimization_searcher != None
+            type_optimization_searcher: Optional[Literal['IVF', 'IVFPQ']] = None,
+            number_centroids: Optional[int] = 8,  # For type_optimization_searcher='IVFPQ'
+            bits: Optional[int] = 8,  # For type_optimization_searcher='IVFPQ'
+            clear_array: Optional[Iterable[str]] = None,
+    ):
+        faiss_database = faiss.IndexFlatL2(embedding_database.shape[1])
+        if count_voronoi_cells > 1:
+            if type_optimization_searcher == 'IVF':
+                faiss_database = faiss.IndexIVFFlat(
+                    faiss_database,
+                    embedding_database.shape[1],
+                    count_voronoi_cells
+                )
+            elif type_optimization_searcher == 'IVFPQ':
+                faiss_database = faiss.IndexIVFPQ(
+                    faiss_database,
+                    embedding_database.shape[1],
+                    count_voronoi_cells,
+                    number_centroids,
+                    bits,
+                )
+            else:
+                raise ValueError('If `count_voronoi_cells` > 1 then `type_optimization` must not be equal to None')
+            faiss_database.train(embedding_database)
+
+        faiss_database.add(embedding_database)
+
+        super().__init__(
+            model=model,
+            embedding_database=faiss_database,
+            original_array=original_array,
+            preprocessing=preprocessing,
+            metric=None,
+            clear_array=clear_array,
         )
-    
-    def change_searcher(
+
+    def _search(
         self,
-        searcher: Type[BaseSearch],
-        **searcher_args,
-    ) -> None:
-        """"""
-        self.__type_searcher = searcher
-        self.__searcher_args = searcher_args
-
-        self._searcher = self.__create_searcher(
-            searcher=self.__type_searcher,
-            model=self._model,
-            embedding_database=self._embedding_database,
-            original_array=self._original_dataset,
-            preprocessing=self._preprocessing,
-            clear_array=self._clear_dataset,
-            searcher_args=searcher_args,
+        array: np.ndarray,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        distances, indices = self._embedding_database.search(array, k)
+        distances, indices = distances[0], indices[0]
+
+        list_texts = []
+        list_similarity = []
+        for i in range(indices.shape[0]):
+            list_texts.append(self._original_array[indices[i]])
+            list_similarity.append(distances[i])
+        return list_texts, list_similarity
+
+
+class ChromaDBSearch(BaseEmbeddingSearch):
+    """
+    Основано на: https://github.com/chroma-core/chroma
+    """
+
+    _MAX_BATCH_CHROMA_DB = 5000
+
+    def __init__(
+            self,
+            model: BaseEmbedding,
+            embedding_database: np.ndarray,
+            original_array: Iterable[str],
+            preprocessing: List[BaseTransformation],
+            metric: Literal['l2', 'ip', 'cosine'] = 'cosine',
+            clear_array: Optional[Iterable[str]] = None,
+    ):
+        chroma_client = chromadb.Client()
+        name_database = create_date_name('database')
+        chroma_database = chroma_client.create_collection(
+            name=name_database,
+            metadata={"hnsw:space": metric}
         )
 
+        if original_array.shape[0] > self._MAX_BATCH_CHROMA_DB:
+            for i in range(0, original_array.shape[0] - self._MAX_BATCH_CHROMA_DB, self._MAX_BATCH_CHROMA_DB):
+                chroma_database.add(
+                    embeddings=embedding_database[i:i+self._MAX_BATCH_CHROMA_DB].tolist(),
+                    ids=original_array[i:i+self._MAX_BATCH_CHROMA_DB].tolist(),
+                )
+        else:
+            chroma_database.add(
+                embeddings=embedding_database.tolist(),
+                ids=original_array.tolist(),
+            )
 
-def load_pipeline(path_to_filename: str) -> Pipeline:
-    """"""
-    if '.pkl' not in path_to_filename:
-        path_to_filename += '.pkl'
-
-    path_to_filename = Path(path_to_filename)
-    with open(path_to_filename, 'rb') as f:
-        pipeline = pickle.load(f)
-    return pipeline
+        super().__init__(
+            model=model,
+            embedding_database=chroma_database,
+            original_array=original_array,
+            preprocessing=preprocessing,
+            metric=metric,
+            clear_array=clear_array,
+        )
+
+    def _search(
+        self,
+        array: np.ndarray,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        result = self._embedding_database.query(
+            query_embeddings=array.tolist(),
+            n_results=k,
+        )
+        list_texts, list_similarity = result['ids'][0], result['distances'][0]
+        return list_texts, list_similarity
```

### Comparing `recs-searcher-0.0.8/recs_searcher/augmentation/_base.py` & `recs-searcher-0.0.9/recs_searcher/augmentation/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/augmentation/_char_aug.py` & `recs-searcher-0.0.9/recs_searcher/augmentation/_char_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/augmentation/_word_aug.py` & `recs-searcher-0.0.9/recs_searcher/augmentation/_word_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/base.py` & `recs-searcher-0.0.9/recs_searcher/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     def load(self, path_folder_load: str, filename: str) -> None:
         """Загрузка vectorizer из файла.
 
         Параметры
         ----------
         path_folder_load : str
             Путь, где лежит файл.
-
         filename : str
             Название файла для загрузки.
 
         Returns
         -------
         None
         """
@@ -90,15 +89,14 @@
     def save(self, path_folder_save: str, filename: str) -> None:
         """Сохранение vectorizer в файл.
 
         Параметры
         ----------
         path_folder_save : str
             Путь сохранения файла.
-
         filename : str
             Название файла для сохранения.
 
         Returns
         -------
         None
         """
@@ -191,41 +189,70 @@
                     text = tmp_text
         else:
             for transformator in preprocessing:
                 text = transformator.transform(text)
         return text
 
     @abstractmethod
+    def _search(
+        self,
+        clear_text: str,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        """Поиск наиболее схожих текстов из БД на clear_text пользователя.
+
+        Параметры
+        ----------
+        clear_text : str
+            Пользовательский текст, которому нужно найти наиболее схожие тексты из БД.
+        k : int
+            Кол-во выдаваемых результатов.
+
+        Returns
+        -------
+        list_texts, list_similarity: Tuple[List[str], List[float]]
+            Вычисленные результаты.
+            В списке `list_texts` хранится текст, который похож на текст пользователя.
+            В списке `list_similarity` хранится схожесть пользовательского текста на текст
+                из бд в виде числа.
+            Все данные соотносятся по индексу в этих двух списках.
+        """
+
     def search(
         self,
         text: str,
         k: int,
         ascending: bool = False,
     ) -> pd.DataFrame:
         """Поиск наиболее схожих k-текстов из БД на text пользователя.
 
         Параметры
         ----------
         text : str
             Пользовательский текст, которому нужно найти наиболее
             схожий текст из БД.
-
         k : int
             Кол-во выдаваемых результатов.
 
         ascending : bool
             Флаг сортировки полученных результатов.
             False - убывающая, True - возрастающая сортировка.
 
         Returns
         -------
         df: pd.DataFrame
             Датафрейм с результатами.
             df.columns = ['text', 'similarity']
         """
+        text = self._preprocessing_text(text, self._preprocessing)
+
+        list_texts, list_similarity = self._search(text, k)
+        df = pd.DataFrame({'text': list_texts, 'similarity': list_similarity})
+        df = df.sort_values(by=['similarity'], ascending=ascending)
+        return df
 
 
 class BaseEmbeddingSearch(BaseSearch):
     """Абстрактный класс для получения результатов
     поиска наиболее схожего текста из БД на основе эмбеддингов.
     """
 
@@ -244,16 +271,73 @@
             clear_array=clear_array,
         )
         self._model = model
         self._embedding_database = embedding_database
         self._metric = metric
 
     @abstractmethod
-    def search(self, text: str, k: int) -> pd.DataFrame:
-        """Та же логика, что и в классе `BaseSearch`."""
+    def _search(
+        self,
+        array: np.ndarray,
+        k: int,
+    ) -> Tuple[List[str], List[float]]:
+        """Поиск наиболее схожих k-векторов из БД на array пользователя.
+
+        Параметры
+        ----------
+        array : np.ndarray
+            Пользовательский текст в виде эмбеддинга, которому нужно найти наиболее
+            схожие вектора из БД.
+        k : int
+            Кол-во выдаваемых результатов.
+
+        Returns
+        -------
+        list_texts, list_similarity: Tuple[List[str], List[float]]
+            Вычисленные результаты.
+            В списке `list_texts` хранится текст, который похож на текст пользователя.
+            В списке `list_similarity` хранится схожесть пользовательского текста на текст
+                из бд в виде числа.
+            Все данные соотносятся по индексу в этих двух списках.
+        """
+    
+    def search(
+        self,
+        text: str,
+        k: int,
+        ascending: bool = False,
+    ) -> pd.DataFrame:
+        """Поиск наиболее схожих k-текстов из БД на text пользователя.
+
+        Параметры
+        ----------
+        text : str
+            Пользовательский текст, которому нужно найти наиболее
+            схожий текст из БД.
+        k : int
+            Кол-во выдаваемых результатов.
+        ascending : bool
+            Флаг сортировки полученных результатов.
+            False - убывающая, True - возрастающая сортировка.
+
+        Returns
+        -------
+        df: pd.DataFrame
+            Датафрейм с результатами.
+            df.columns = ['text', 'similarity']
+        """
+        text = self._preprocessing_text(text, self._preprocessing)
+
+        text = [text]
+        array = self._model.transform(text)
+
+        list_texts, list_similarity = self._search(array, k)
+        df = pd.DataFrame({'text': list_texts, 'similarity': list_similarity})
+        df = df.sort_values(by=['similarity'], ascending=ascending)
+        return df
 
 
 class BaseExplain(ABC):
     """Абстрактный класс для интерпретации схожести двух текстовых данных."""
 
     def __init__(
         self,
@@ -264,29 +348,55 @@
         self._preprocessing = preprocessing
 
     def _preprocessing_text(
         self,
         text: str,
         preprocessing: List[BaseTransformation],
     ) -> str:
-        """"""
+        """
+        Предобработка текста.
+
+        Параметры
+        ----------
+        text : str
+            Необработанный текст.
+        preprocessing : List[BaseTransformation]
+            Список алгоритмов для предобработка текста.
+
+        Returns
+        -------
+        text: str
+            Обработанный текст.
+        """
         for transformator in preprocessing:
             tmp_text = transformator.transform([text])[0]
             if tmp_text:
                 text = tmp_text
         return text
 
     @abstractmethod
     def _explain(
         self,
         clear_compared_text: str,
         clear_original_text: str,
         n_grams: int = 1,
     ) -> Tuple[List[str], List[float]]:
         """
+        Поиск наиболее схожих N-грамм из clear_compared_text в clear_original_text.
+
+        Параметры
+        ----------
+        clear_compared_text : str
+            Пользовательский текст, в котором нужно найти n-граммы,
+            похожие на clear_original_text.
+        clear_original_text : str
+            Текст, с которым сравнивается clear_compared_text.
+        n_grams : int
+            Длина N-грамм.
+
         Returns
         -------
         list_text, list_similarity: Tuple[List[str]. List[float]]
             Кортеж списков.
         """
 
     def explain(
@@ -294,14 +404,32 @@
         compared_text: str,
         original_text: str,
         n_grams: Union[Tuple[int, int], int] = 1,
         k: int = 10,
         ascending: bool = True,
     ) -> pd.DataFrame:
         """
+        Поиск наиболее схожих N-грамм из compared_text в original_text.
+
+        Параметры
+        ----------
+        compared_text : str
+            Пользовательский текст, в котором нужно найти n-граммы,
+            похожие на original_text.
+        original_text : str
+            Текст, с которым сравнивается compared_text.
+        n_grams : Union[Tuple[int, int], int]
+            Длины N-грамм, которые будут оцениваться.
+            Может приниматься либо одно число, либо список чисел.
+        k : int
+            Кол-во выдаваемых результатов.
+        ascending : bool
+            Флаг сортировки полученных результатов.
+            False - убывающая, True - возрастающая сортировка.
+
         Returns
         -------
         df: pd.DataFrame
             Датафрейм с результатами.
             df.columns = ['text', 'similarity']
         """
```

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/_base.py` & `recs-searcher-0.0.9/recs_searcher/dataset/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/_dataframes.py` & `recs-searcher-0.0.9/recs_searcher/dataset/_dataframes.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/address_krasnoyarsk.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/address_krasnoyarsk.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/city_russia.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/city_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/company_russia.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/company_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/exoplanets.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/exoplanets.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/medical_supplies.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/medical_supplies.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/mobile_phones.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/mobile_phones.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/russian_dictionary.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/russian_dictionary.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/dataset/data/video_games.csv` & `recs-searcher-0.0.9/recs_searcher/dataset/data/video_games.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/embeddings/_base.py` & `recs-searcher-0.0.9/recs_searcher/embeddings/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/recs_searcher/explain/_base.py` & `recs-searcher-0.0.9/recs_searcher/explain/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Алгоритмы для объяснение сходства одного текста на другой.
 """
 
 from ..base import BaseExplain, BaseEmbedding, BaseTransformation
 from ..utils import cosine_distance, euclidean_distance
 
 from typing import List, Union, Callable, Literal, Tuple 
-import pandas as pd
 import numpy as np
 
 
 class DistanceExplain(BaseExplain):
     """Класс для интерпретации сходства двух текстовых данных
     путём взятия окна из n-токенов из оригинального текста и подсчёта
     расстояния их эмбеддингов с оригинальным."""
@@ -33,29 +32,41 @@
     def __define_distance(
         self,
         distance: Union[
             Literal['cosine', 'euclidean'],
             Callable[[np.ndarray, np.ndarray], float],
         ],
     ) -> Callable[[np.ndarray, np.ndarray], float]:
-        """"""
+        """
+        Определение функции для подсчёта расстояния между 2 векторами.
+
+        Параметры
+        ----------
+        distance : Union[Literal['cosine', 'euclidean'], Callable[[np.ndarray, np.ndarray], float]]
+            Текст - для получения функции, реализованной в данном проекта.
+            Функция - для встраивания своей функции для подсчёта расстояния.
+
+        Returns
+        -------
+        distance: Callable[[np.ndarray, np.ndarray], float]
+            Функция для подсчёта расстояния между двумя векторами.
+        """
         if distance == 'cosine':
             return cosine_distance
         elif distance == 'euclidean':
             return euclidean_distance
         else:
             return distance
 
     def _explain(
         self,
         clear_compared_text: str,
         clear_original_text: str,
         n_grams: int = 1,
     ) -> Tuple[List[str], List[float]]:
-        """"""
         tokens_list = clear_compared_text.split(' ')
 
         list_text = []
         list_similarity = []
 
         clear_original_embedding = self._model.transform([clear_original_text])
         for i in range(len(tokens_list) - n_grams + 1):
```

### Comparing `recs-searcher-0.0.8/recs_searcher/preprocessing/_base_normalize.py` & `recs-searcher-0.0.9/recs_searcher/preprocessing/_base_normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,51 +4,49 @@
 
 from typing import List
 from ..base import BaseTransformation
 import spacy
 
 
 class LemmatizeSpacy(BaseTransformation):
-    """Лемматизация слов с помощью Spacy-моделей."""
+    """Алгоритм лемматизации слов с помощью Spacy-моделей."""
 
     def __init__(self, spacy_model_name: str):
         super().__init__()
 
         try:
             self._spacy_model = spacy.load(spacy_model_name)
         except OSError:
             print(f'Downloading {spacy_model_name}...')
             spacy.cli.download(spacy_model_name)
             self._spacy_model = spacy.load(spacy_model_name)
 
-    def __transform(self, array: List[str]) -> List[str]:
-        """"""
+    def _transform(self, array: List[str]) -> List[str]:
         transformed_array = []
         for text in array:
             doc = self._spacy_model(text)
             transformed_text = ' '.join([token.lemma_ if token.lemma_ else token for token in doc])
             transformed_array.append(transformed_text)
         return transformed_array
 
 
 class RemoveStopwordsSpacy(BaseTransformation):
-    """Удаление стоп-слов с помощью Spacy-моделей."""
+    """Алгоритм удаления стоп-слов с помощью Spacy-моделей."""
 
     def __init__(self, spacy_model_name: str):
         super().__init__()
 
         try:
             self._spacy_model = spacy.load(spacy_model_name)
         except OSError:
             print(f'Downloading {spacy_model_name}...')
             spacy.cli.download(spacy_model_name)
             self._spacy_model = spacy.load(spacy_model_name)
 
-    def __transform(self, array: List[str]) -> List[str]:
-        """"""
+    def _transform(self, array: List[str]) -> List[str]:
         transformed_array = []
         for text in array:
             clear_tokens = []
             doc = self._spacy_model(text)
             for token in doc:
                 if not token.is_stop:
                     clear_tokens.append(token.text)
```

### Comparing `recs-searcher-0.0.8/recs_searcher/utils/_concat_embeddings.py` & `recs-searcher-0.0.9/recs_searcher/utils/_concat_embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ) -> np.ndarray:
     """Конкатенация эмбеддингов, полученных разными алгоритмами.
 
         Параметры:
         ----------
         embeddings : List[np.ndarray]
             Список массивов-эмбеддингов.
-
         weights : List[float]
             Список весов важности каждого эмбеддинга при конкатенации.
 
         Returns
         -------
         embedding: np.ndarray
             Массив, объединяющий входные эмббединги `embeddings`.
```

### Comparing `recs-searcher-0.0.8/recs_searcher.egg-info/PKG-INFO` & `recs-searcher-0.0.9/recs_searcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: recs-searcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Search engine and registry error corrector
 Home-page: https://github.com/sheriff1max/recs-searcher
 Author: sheriff1max
 Author-email: kobelevmaxim48@gmail.com
 Project-URL: Bug tracker, https://github.com/sheriff1max/recs-searcher/issues
-Keywords: python searcher corrector faiss fasttext embeddings
+Keywords: python searcher corrector faiss chroma-bd embeddings
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: chromadb
 Requires-Dist: datasets
```

### Comparing `recs-searcher-0.0.8/recs_searcher.egg-info/SOURCES.txt` & `recs-searcher-0.0.9/recs_searcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.8/setup.py` & `recs-searcher-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='recs-searcher',
-  version='0.0.8',
+  version='0.0.9',
   author='sheriff1max',
   author_email='kobelevmaxim48@gmail.com',
   description='Search engine and registry error corrector',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/sheriff1max/recs-searcher',
   packages=find_packages(),
@@ -30,13 +30,13 @@
     'thefuzz',
     'torch',
     'torchvision',
   ],
   classifiers=[
     'Programming Language :: Python :: 3',
   ],
-  keywords='python searcher corrector faiss fasttext embeddings',
+  keywords='python searcher corrector faiss chroma-bd embeddings',
   project_urls={
     'Bug tracker': 'https://github.com/sheriff1max/recs-searcher/issues'
   },
   python_requires='>=3.11'
 )
```

