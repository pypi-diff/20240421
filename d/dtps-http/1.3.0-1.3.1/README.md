# Comparing `tmp/dtps_http-1.3.0-py3-none-any.whl.zip` & `tmp/dtps_http-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -34,13 +34,13 @@
 -rw-r--r--  2.0 unx     4682 b- defN 80-Jan-01 00:00 dtps_http_programs/test_memory.py
 -rw-r--r--  2.0 unx     3267 b- defN 80-Jan-01 00:00 dtps_http_programs/test_memory_dashboard.py
 -rw-r--r--  2.0 unx     2988 b- defN 80-Jan-01 00:00 dtps_http_programs/test_memory_dashboard_just_push.py
 -rw-r--r--  2.0 unx     5257 b- defN 80-Jan-01 00:00 dtps_http_programs/test_memory_use.py
 -rw-r--r--  2.0 unx     1270 b- defN 80-Jan-01 00:00 static/favicon.png
 -rw-r--r--  2.0 unx     7885 b- defN 80-Jan-01 00:00 static/send.js
 -rw-r--r--  2.0 unx     1472 b- defN 80-Jan-01 00:00 static/style.css
--rw-r--r--  2.0 unx    75933 b- defN 80-Jan-01 00:00 dtps_http-1.3.0.dist-info/LICENSE.pdf
--rw-r--r--  2.0 unx     1040 b- defN 80-Jan-01 00:00 dtps_http-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dtps_http-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 dtps_http-1.3.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3595 b- defN 16-Jan-01 00:00 dtps_http-1.3.0.dist-info/RECORD
+-rw-r--r--  2.0 unx    75933 b- defN 80-Jan-01 00:00 dtps_http-1.3.1.dist-info/LICENSE.pdf
+-rw-r--r--  2.0 unx     1040 b- defN 80-Jan-01 00:00 dtps_http-1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dtps_http-1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 dtps_http-1.3.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3595 b- defN 16-Jan-01 00:00 dtps_http-1.3.1.dist-info/RECORD
 44 files, 384792 bytes uncompressed, 152862 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -111,23 +111,23 @@
 
 Filename: static/send.js
 Comment: 
 
 Filename: static/style.css
 Comment: 
 
-Filename: dtps_http-1.3.0.dist-info/LICENSE.pdf
+Filename: dtps_http-1.3.1.dist-info/LICENSE.pdf
 Comment: 
 
-Filename: dtps_http-1.3.0.dist-info/METADATA
+Filename: dtps_http-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: dtps_http-1.3.0.dist-info/WHEEL
+Filename: dtps_http-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: dtps_http-1.3.0.dist-info/entry_points.txt
+Filename: dtps_http-1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: dtps_http-1.3.0.dist-info/RECORD
+Filename: dtps_http-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dtps/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 from logging import DEBUG, getLogger
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 from .config import *
```

## dtps_http/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 import coloredlogs  # type: ignore
 
 coloredlogs.install(level="DEBUG")  # type: ignore
 
 from logging import getLogger, INFO, WARNING
```

## dtps_http_programs/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 from logging import DEBUG, getLogger
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 from .server_clock import *
```

## Comparing `dtps_http-1.3.0.dist-info/LICENSE.pdf` & `dtps_http-1.3.1.dist-info/LICENSE.pdf`

 * *Files identical despite different names*

## Comparing `dtps_http-1.3.0.dist-info/METADATA` & `dtps_http-1.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtps-http
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 Author: Andrea Censi
 Author-email: AndreaCensi@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `dtps_http-1.3.0.dist-info/RECORD` & `dtps_http-1.3.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-dtps/__init__.py,sha256=ZPg1vr8zay4cN_ZI3waaC1NRkQhf4Tc6v7MQUmPW0oo,235
+dtps/__init__.py,sha256=En6BEKyFIcSP1KK9_SYnMhSP7mr52SC5z7a8jIdR6XA,235
 dtps/config.py,sha256=pX8NyQFRER6sxKxiCCNW7rTjUR2lQyg7yi-wcTzwlDA,6709
 dtps/ergo_create.py,sha256=awaOjfX8eVBzK_y2us3WcOTxiS3v3j7XqTVf55UKPk4,11921
 dtps/ergo_ui.py,sha256=lnP4ChQcc2hQkOxDDQEj_FG_SQc2aCEiICEPtRL2dSI,7597
 dtps/ergo_use.py,sha256=lZJg0Pd1mj-bbRqlcB06ebEpQ5L0wkHF1QyvvURnI4k,12744
 dtps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dtps/structures.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dtps_http/__init__.py,sha256=f3BIzAsEff9oI3_lYYddxQpY62MLRWAVjK5dyeABdOs,655
+dtps_http/__init__.py,sha256=P3Yl5XJudr1S23w_POIYVYCPHqGjBbS2t7_rVyhiLYA,655
 dtps_http/blob_manager.py,sha256=cHg_4nU1_X7KjBUK6meX0pZkEJ8MCzOw6k1gh1DefzM,4860
 dtps_http/client.py,sha256=gdQF6n3u44i977uwbMf46zWGNKE6usk0ABYY7chC_7M,62746
 dtps_http/constants.py,sha256=1p5-Jywj4SvV4WR-Krx7agOjhHCbbt8cKiD3Ng_n-_8,3576
 dtps_http/ergo_utils.py,sha256=tVW797yywqleDm9f0yoo8pZXHk5yb-8gr3j9yJQjakI,1365
 dtps_http/exceptions.py,sha256=4w-Yrx-MedOytS_QIpNCiIZRQbFTjyjID-MO-JL_skw,420
 dtps_http/link_headers.py,sha256=ADp5tF-pKU1N7W3M4SISASYTTisL086lTHKYpwDPEo0,1672
 dtps_http/object_queue.py,sha256=u7Qjn47RaCzv-PJubiufsRj_wTI0sZkp44C7EbWPRi8,10357
@@ -18,27 +18,27 @@
 dtps_http/server_start.py,sha256=fK1pNHPveSCeEw8AV5M6WfVqKHz4nyq4xW1tP9JZCtI,9695
 dtps_http/structures.py,sha256=wjq_7U4Zn9V1h9yJgpZ82ssU6hHgw84miyafCWun4ps,17307
 dtps_http/types.py,sha256=0izHqzwhIqABEFg6lPuf9-fzu8VvxjsukOOlepl9nhQ,3555
 dtps_http/types_of_source.py,sha256=qpq--U-xBYPWPKpGN1z8wq_uOk0oLBahW9Voz-A2NF0,21400
 dtps_http/urls.py,sha256=NmGcqCpanRrco1JhPQGNvn-rLG2jIQ9W7J2G9YyisGQ,4336
 dtps_http/utils.py,sha256=V31fI0dQSMuG5UcWuQZcuSlol9oC92ZonN_bx6REHDI,6139
 dtps_http/utils_every_once_in_a_while.py,sha256=nvZsWa1dnK0i8bSkOciUw-VrLxMpT25QZ6pOcXQICig,838
-dtps_http_programs/__init__.py,sha256=H5xDK8SaJkchYUGY35pju9E2iLAQKPKBuqUGvZSYg4Q,257
+dtps_http_programs/__init__.py,sha256=hYcROWKDhb2AMbC3diorM-XXNFYyv3SuwNzhNfjLziw,257
 dtps_http_programs/dtps_listen.py,sha256=2T-CxSAqnC7mdT5AD-bsYqWBggPABefadL_TjxGrBR0,3671
 dtps_http_programs/dtps_proxy.py,sha256=luhDbyOQeFuQOeAXhIB8CjsYhjW8260rHVN2vVWKiTM,1721
 dtps_http_programs/dtps_send_continuous.py,sha256=M4QHRoAUrZ04Rshm11n-g4CUsEeDjvW_UpdRqUHccvo,1338
 dtps_http_programs/dtps_stats.py,sha256=oC8uEjPFhUN1soZ6wkyzmffPPRLuZxrjESsbqfVBN9A,3112
 dtps_http_programs/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dtps_http_programs/server_clock.py,sha256=r7aJJjsXN6Gy26Iy6qw_gs0xQ7RbMlgJBcAhZYFZt7M,1789
 dtps_http_programs/test_hashes.py,sha256=jlM1AvYSSndg07LHyIzRRDIWMXeyR5rHlLg18hGvRwU,1886
 dtps_http_programs/test_memory.py,sha256=pI1W8admZA3k7XpR-7q2R1eCuVUi71jW5A4xkFwUZGA,4682
 dtps_http_programs/test_memory_dashboard.py,sha256=MwdW9yT4wfNYpEzDLi9UaZRUvzuD39gfxbaMKth6YQ8,3267
 dtps_http_programs/test_memory_dashboard_just_push.py,sha256=c2HAhcrR2pUqAeBuBFnOmmxxpfAnoHsy4r912JfH1Zc,2988
 dtps_http_programs/test_memory_use.py,sha256=CguYdI4kYFLj_jRmmzVzFEuBSBWA-zLxZMNAA6S9wt8,5257
 static/favicon.png,sha256=SuoDecEFzJG3RabXtOofSBcIPjDhKVLjFB0UX_LW4tI,1270
 static/send.js,sha256=_dvhwM61lpyrlIDd0-3xeJ59RCPgeLzBcMpeDlNqEms,7885
 static/style.css,sha256=hYKy8n6jh47vqXRg-ljM1x3Ket2rtMhH08TpOIHaW_s,1472
-dtps_http-1.3.0.dist-info/LICENSE.pdf,sha256=V1TBclYda54_miAikuVMwqHoWjwkjHw_yoF2zEqpc_k,75933
-dtps_http-1.3.0.dist-info/METADATA,sha256=eHsHz43yIiBRvMc9u0cknLLWR_WTqEttZKaD0OFRjXc,1040
-dtps_http-1.3.0.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-dtps_http-1.3.0.dist-info/entry_points.txt,sha256=0f8h-Ls_gnf01ABr2FNt1iv2hZqrTfchBMIq-hJs6Uc,379
-dtps_http-1.3.0.dist-info/RECORD,,
+dtps_http-1.3.1.dist-info/LICENSE.pdf,sha256=V1TBclYda54_miAikuVMwqHoWjwkjHw_yoF2zEqpc_k,75933
+dtps_http-1.3.1.dist-info/METADATA,sha256=yrsSiu0cOgZlljD46vPg_2uRROp2PGNt2n_Ck6YWO3E,1040
+dtps_http-1.3.1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+dtps_http-1.3.1.dist-info/entry_points.txt,sha256=0f8h-Ls_gnf01ABr2FNt1iv2hZqrTfchBMIq-hJs6Uc,379
+dtps_http-1.3.1.dist-info/RECORD,,
```

