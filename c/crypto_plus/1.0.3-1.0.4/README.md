# Comparing `tmp/crypto_plus-1.0.3.tar.gz` & `tmp/crypto_plus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_plus-1.0.3.tar", max compression
+gzip compressed data, was "crypto_plus-1.0.4.tar", max compression
```

## Comparing `crypto_plus-1.0.3.tar` & `crypto_plus-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.3/LICENSE
--rw-r--r--   0        0        0     1608 2024-04-13 10:41:02.033305 crypto_plus-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.3/README.md
--rw-r--r--   0        0        0      143 2024-04-13 10:41:09.260895 crypto_plus-1.0.3/src/crypto_plus/__init__.py
--rw-r--r--   0        0        0     7586 2024-04-13 10:30:04.946637 crypto_plus-1.0.3/src/crypto_plus/asymmetric.py
--rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.3/src/crypto_plus/base.py
--rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.3/src/crypto_plus/compatible.py
--rw-r--r--   0        0        0     5688 2024-04-13 10:33:43.989796 crypto_plus-1.0.3/src/crypto_plus/encrypt.py
--rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.3/src/crypto_plus/key.py
--rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.3/src/crypto_plus/sign.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-21 11:49:13.365418 crypto_plus-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.4/README.md
+-rw-r--r--   0        0        0      143 2024-04-21 11:49:20.334234 crypto_plus-1.0.4/src/crypto_plus/__init__.py
+-rw-r--r--   0        0        0     7586 2024-04-13 10:30:04.946637 crypto_plus-1.0.4/src/crypto_plus/asymmetric.py
+-rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.4/src/crypto_plus/base.py
+-rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.4/src/crypto_plus/compatible.py
+-rw-r--r--   0        0        0     5688 2024-04-13 10:33:43.989796 crypto_plus-1.0.4/src/crypto_plus/encrypt.py
+-rw-r--r--   0        0        0     6234 2024-04-21 11:48:44.632934 crypto_plus-1.0.4/src/crypto_plus/key.py
+-rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.4/src/crypto_plus/sign.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.4/PKG-INFO
```

### Comparing `crypto_plus-1.0.3/LICENSE` & `crypto_plus-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/pyproject.toml` & `crypto_plus-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crypto_plus"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Easy-to-use Crypto Tool"
 readme = "README.md"
 authors = ["wmymz <wmymz@icloud.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.12",
```

### Comparing `crypto_plus-1.0.3/README.md` & `crypto_plus-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/src/crypto_plus/asymmetric.py` & `crypto_plus-1.0.4/src/crypto_plus/asymmetric.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/src/crypto_plus/compatible.py` & `crypto_plus-1.0.4/src/crypto_plus/compatible.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/src/crypto_plus/encrypt.py` & `crypto_plus-1.0.4/src/crypto_plus/encrypt.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/src/crypto_plus/key.py` & `crypto_plus-1.0.4/src/crypto_plus/key.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from Crypto.PublicKey.ECC import EccKey
 from Crypto.PublicKey.RSA import RsaKey
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import dsa
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509 import Certificate
+from cryptography.x509 import load_der_x509_certificate
 from cryptography.x509 import load_pem_x509_certificate
 
 
 def loads_key(key_bytes: Union[bytes, str], password: Optional[bytes] = None):
     if isinstance(key_bytes, str):
         if key_bytes.startswith("-----"):
             key_bytes = key_bytes.encode()
@@ -56,14 +57,18 @@
         return serialization.load_ssh_public_key(key_bytes)
     except Exception:
         pass
     try:
         return load_pem_x509_certificate(key_bytes)
     except Exception:
         pass
+    try:
+        return load_der_x509_certificate(key_bytes)
+    except Exception:
+        pass
     raise Exception("无法加载密钥，密钥格式或密码错误")
 
 
 def dumps_key(
     key: Union[RsaKey, DsaKey, EccKey], key_format="PEM"
 ) -> Union[bytes, str]:
     return key.export_key(format=key_format)
```

### Comparing `crypto_plus-1.0.3/src/crypto_plus/sign.py` & `crypto_plus-1.0.4/src/crypto_plus/sign.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.3/PKG-INFO` & `crypto_plus-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto_plus
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Easy-to-use Crypto Tool
 License: MIT
 Author: wmymz
 Author-email: wmymz@icloud.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

