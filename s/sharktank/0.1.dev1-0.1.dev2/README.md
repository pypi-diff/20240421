# Comparing `tmp/sharktank-0.1.dev1-py3-none-any.whl.zip` & `tmp/sharktank-0.1.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 63173 bytes, number of entries: 43
+Zip file size: 63172 bytes, number of entries: 43
 -rw-rw-r--  2.0 unx      228 b- defN 24-Apr-20 22:22 sharktank/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-20 22:22 sharktank/py.typed
 -rw-rw-r--  2.0 unx     4538 b- defN 24-Apr-20 22:22 sharktank/examples/export_paged_llm_v1.py
 -rw-rw-r--  2.0 unx     8418 b- defN 24-Apr-20 22:22 sharktank/examples/paged_llm_v1.py
 -rw-rw-r--  2.0 unx     1422 b- defN 24-Apr-20 22:22 sharktank/examples/validate_llama_ref_model.py
 -rw-rw-r--  2.0 unx     5296 b- defN 24-Apr-20 22:22 sharktank/examples/validate_paged_llama_model.py
 -rw-rw-r--  2.0 unx      560 b- defN 24-Apr-20 22:22 sharktank/layers/__init__.py
@@ -34,12 +34,12 @@
 -rw-rw-r--  2.0 unx     3983 b- defN 24-Apr-20 22:22 sharktank/types/gguf_interop/base.py
 -rw-rw-r--  2.0 unx    10013 b- defN 24-Apr-20 22:22 sharktank/types/gguf_interop/layouts.py
 -rw-rw-r--  2.0 unx     3289 b- defN 24-Apr-20 22:22 sharktank/utils/cli.py
 -rw-rw-r--  2.0 unx     2144 b- defN 24-Apr-20 22:22 sharktank/utils/debugging.py
 -rw-rw-r--  2.0 unx     5542 b- defN 24-Apr-20 22:22 sharktank/utils/hf_datasets.py
 -rw-rw-r--  2.0 unx      282 b- defN 24-Apr-20 22:22 sharktank/utils/logging.py
 -rw-rw-r--  2.0 unx     3128 b- defN 24-Apr-20 22:22 sharktank/utils/tokenizer.py
--rw-rw-r--  2.0 unx     1681 b- defN 24-Apr-20 23:19 sharktank-0.1.dev1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 23:19 sharktank-0.1.dev1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 24-Apr-20 23:19 sharktank-0.1.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3758 b- defN 24-Apr-20 23:19 sharktank-0.1.dev1.dist-info/RECORD
-43 files, 183782 bytes uncompressed, 57139 bytes compressed:  68.9%
+-rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-20 23:55 sharktank-0.1.dev2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 23:55 sharktank-0.1.dev2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 24-Apr-20 23:55 sharktank-0.1.dev2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3758 b- defN 24-Apr-20 23:55 sharktank-0.1.dev2.dist-info/RECORD
+43 files, 183778 bytes uncompressed, 57138 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -111,20 +111,20 @@
 
 Filename: sharktank/utils/logging.py
 Comment: 
 
 Filename: sharktank/utils/tokenizer.py
 Comment: 
 
-Filename: sharktank-0.1.dev1.dist-info/METADATA
+Filename: sharktank-0.1.dev2.dist-info/METADATA
 Comment: 
 
-Filename: sharktank-0.1.dev1.dist-info/WHEEL
+Filename: sharktank-0.1.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: sharktank-0.1.dev1.dist-info/top_level.txt
+Filename: sharktank-0.1.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: sharktank-0.1.dev1.dist-info/RECORD
+Filename: sharktank-0.1.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sharktank-0.1.dev1.dist-info/METADATA` & `sharktank-0.1.dev2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sharktank
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: SHARK layers and inference models for genai
-Home-page: https://github.com/nod-ai/SHARK-Turbine
+Home-page: https://github.com/nod-ai/sharktank
 Author: SHARK Authors
 Author-email: stella@nod.ai
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

## Comparing `sharktank-0.1.dev1.dist-info/RECORD` & `sharktank-0.1.dev2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -33,11 +33,11 @@
 sharktank/types/gguf_interop/base.py,sha256=XTyK2rFMlCj-aXCn7SvGe5gxKo4CgFfEjFFyUX41DhQ,3983
 sharktank/types/gguf_interop/layouts.py,sha256=rnmKQmo9qQE9Dkf2En38mMVI_9Anq0jkW4A1spFgu3o,10013
 sharktank/utils/cli.py,sha256=lEwhcmS9g3dFdOZ2-6MsMLhBgcx-HW3iQjD9B2U2VK8,3289
 sharktank/utils/debugging.py,sha256=jsHTC49KI93ysoJyIVr4K_H56SUAUdopqzttMb_JRjo,2144
 sharktank/utils/hf_datasets.py,sha256=-BXAESbGm1D0mWiry7NRM5f5HHI911mr1McXH2865ec,5542
 sharktank/utils/logging.py,sha256=KdpFZpx5yVBELDLGshvpWL2dTM0Wdy7rhf7TUm_GSNw,282
 sharktank/utils/tokenizer.py,sha256=CkB2udi-8oRifxC6T3TGRItZWSOBFXP6sipoT8hhxms,3128
-sharktank-0.1.dev1.dist-info/METADATA,sha256=6AgyRgcu4yA9ANGLStqBkksn9AQp5TB1oF_QOXhC-gM,1681
-sharktank-0.1.dev1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-sharktank-0.1.dev1.dist-info/top_level.txt,sha256=oSoFZzz1TWh9sLGFIiy1n6ARmNjGTARk5_Tagz9vzKA,10
-sharktank-0.1.dev1.dist-info/RECORD,,
+sharktank-0.1.dev2.dist-info/METADATA,sha256=12WDHsEcVQ-HFuzAHGlF0C-wCeNMDj6dpbiQJd7MPQs,1677
+sharktank-0.1.dev2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sharktank-0.1.dev2.dist-info/top_level.txt,sha256=oSoFZzz1TWh9sLGFIiy1n6ARmNjGTARk5_Tagz9vzKA,10
+sharktank-0.1.dev2.dist-info/RECORD,,
```

