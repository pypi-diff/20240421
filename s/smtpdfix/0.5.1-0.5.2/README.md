# Comparing `tmp/smtpdfix-0.5.1.tar.gz` & `tmp/smtpdfix-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smtpdfix-0.5.1.tar", last modified: Sat Jul  8 01:18:38 2023, max compression
+gzip compressed data, was "smtpdfix-0.5.2.tar", last modified: Sun Apr 21 14:17:06 2024, max compression
```

## Comparing `smtpdfix-0.5.1.tar` & `smtpdfix-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.648136 smtpdfix-0.5.1/
--rw-r--r--   0 james      (501) staff       (20)     1089 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)    10715 2023-07-08 01:18:38.648217 smtpdfix-0.5.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     9715 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/README.md
--rw-r--r--   0 james      (501) staff       (20)       90 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)     2085 2023-07-08 01:18:38.648595 smtpdfix-0.5.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)       41 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.646337 smtpdfix-0.5.1/smtpdfix/
--rw-r--r--   0 james      (501) staff       (20)      342 2023-07-08 01:17:28.000000 smtpdfix-0.5.1/smtpdfix/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1041 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/authenticator.py
--rw-r--r--   0 james      (501) staff       (20)     3063 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/certs.py
--rw-r--r--   0 james      (501) staff       (20)     5034 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/configuration.py
--rw-r--r--   0 james      (501) staff       (20)     8078 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/smtpdfix/controller.py
--rw-r--r--   0 james      (501) staff       (20)      688 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/event_handler.py
--rw-r--r--   0 james      (501) staff       (20)     2577 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/fixture.py
--rw-r--r--   0 james      (501) staff       (20)     3400 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/smtpdfix/handlers.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/py.typed
--rw-r--r--   0 james      (501) staff       (20)     1660 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/smtpdfix/smtp.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.647215 smtpdfix-0.5.1/smtpdfix.egg-info/
--rw-r--r--   0 james      (501) staff       (20)    10715 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      614 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       36 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      120 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        9 2023-07-08 01:18:38.000000 smtpdfix-0.5.1/smtpdfix.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 01:18:38.648024 smtpdfix-0.5.1/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1191 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/conftest.py
--rw-r--r--   0 james      (501) staff       (20)     3016 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/test_configuration.py
--rw-r--r--   0 james      (501) staff       (20)     4789 2023-06-23 13:43:39.000000 smtpdfix-0.5.1/tests/test_controller.py
--rw-r--r--   0 james      (501) staff       (20)     7914 2023-06-14 22:23:18.000000 smtpdfix-0.5.1/tests/test_fixture.py
--rw-r--r--   0 james      (501) staff       (20)     3057 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/tests/test_smtp.py
--rw-r--r--   0 james      (501) staff       (20)     1068 2023-07-07 21:15:57.000000 smtpdfix-0.5.1/tests/test_smtpdfix.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-21 14:17:06.869844 smtpdfix-0.5.2/
+-rw-r--r--   0 james      (501) staff       (20)     1089 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    11281 2024-04-21 14:17:06.869754 smtpdfix-0.5.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     9879 2023-12-28 16:47:44.000000 smtpdfix-0.5.2/README.md
+-rw-r--r--   0 james      (501) staff       (20)       90 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)     2072 2024-04-21 14:17:06.870194 smtpdfix-0.5.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-21 14:17:06.866888 smtpdfix-0.5.2/smtpdfix/
+-rw-r--r--   0 james      (501) staff       (20)      342 2024-04-21 14:16:56.000000 smtpdfix-0.5.2/smtpdfix/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1041 2023-07-23 23:33:59.000000 smtpdfix-0.5.2/smtpdfix/authenticator.py
+-rw-r--r--   0 james      (501) staff       (20)     4115 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/smtpdfix/certs.py
+-rw-r--r--   0 james      (501) staff       (20)     5731 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/smtpdfix/configuration.py
+-rw-r--r--   0 james      (501) staff       (20)     7624 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/smtpdfix/controller.py
+-rw-r--r--   0 james      (501) staff       (20)      688 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/smtpdfix/event_handler.py
+-rw-r--r--   0 james      (501) staff       (20)     2619 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/smtpdfix/fixture.py
+-rw-r--r--   0 james      (501) staff       (20)     3400 2023-07-07 21:15:57.000000 smtpdfix-0.5.2/smtpdfix/handlers.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/smtpdfix/py.typed
+-rw-r--r--   0 james      (501) staff       (20)     3648 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/smtpdfix/smtp.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-21 14:17:06.869206 smtpdfix-0.5.2/smtpdfix.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    11281 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      614 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       36 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      139 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        9 2024-04-21 14:17:06.000000 smtpdfix-0.5.2/smtpdfix.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-21 14:17:06.868945 smtpdfix-0.5.2/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1191 2023-07-17 15:25:51.000000 smtpdfix-0.5.2/tests/conftest.py
+-rw-r--r--   0 james      (501) staff       (20)     3561 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/tests/test_configuration.py
+-rw-r--r--   0 james      (501) staff       (20)     4588 2024-04-03 14:22:20.000000 smtpdfix-0.5.2/tests/test_controller.py
+-rw-r--r--   0 james      (501) staff       (20)     7914 2023-06-14 22:23:18.000000 smtpdfix-0.5.2/tests/test_fixture.py
+-rw-r--r--   0 james      (501) staff       (20)     3057 2024-02-11 10:10:02.000000 smtpdfix-0.5.2/tests/test_smtp.py
+-rw-r--r--   0 james      (501) staff       (20)     1068 2023-07-07 21:15:57.000000 smtpdfix-0.5.2/tests/test_smtpdfix.py
```

### Comparing `smtpdfix-0.5.1/LICENSE` & `smtpdfix-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/PKG-INFO` & `smtpdfix-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.5.1
+Version: 0.5.2
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
 Project-URL: Issues, https://github.com/bebleo/smtpdfix/issues
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: typing
 License-File: LICENSE
+Requires-Dist: aiosmtpd
+Requires-Dist: cryptography
+Requires-Dist: portpicker
+Requires-Dist: pytest
+Provides-Extra: testing
+Requires-Dist: flake8; extra == "testing"
+Requires-Dist: isort; extra == "testing"
+Requires-Dist: mypy; extra == "testing"
+Requires-Dist: pytest-asyncio; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-timeout; extra == "testing"
+Provides-Extra: dev
+Requires-Dist: smtpdfix[testing]; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # SMTPDFix: Test email, locally
 
 ![build](https://github.com/bebleo/bebleo_smtpd_fixture/workflows/build/badge.svg)
 
 A simple SMTP server based on `aiosmtpd` for use as a fixture with pytest that supports encryption and authentication. All this does is receives messages and appends them to a list as an `email.Message`.
 
@@ -198,19 +209,28 @@
 Many libraries for sending email have built-in methods for testing and using these methods should generally be prefered over SMTPDFix. Some known solutions:
 
 + **fastapi-mail**: has a `record_messsages()` method to intercept the mail. Instructions on how to suppress the sending of mail and implement it can be seen at [https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail](https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail)
 + **flask-mail**: has a method to suppress sending and capture the email for testing purposes. [Instructions](https://pythonhosted.org/Flask-Mail/#unit-tests-and-suppressing-emails)
 
 ## Developing
 
-To develop and test smtpdfix you will need to install [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests, [isort](https://pycqa.github.io/isort/) to sort imports and [flake8](https://flake8.pycqa.org/en/latest/) to lint. To install in a virtual environment for development:
+To develop and test smtpdfix you will need to install:
++ [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests,
++ [pytest-cov](https://github.com/pytest-dev/pytest-cov) to ensure 100% code coverages,
++ [pytest-timeout](https://github.com/pytest-dev/pytest-timeout) so that tests timeout,
++ [isort](https://pycqa.github.io/isort/) to sort imports,
++ [flake8](https://flake8.pycqa.org/en/latest/) to lint,
++ [mypy](https://mypy.readthedocs.io/en/stable/) for type checking,, and finally
++ [tox](https://tox.wiki/) to run a complete set of tests.
+
+To install all of these in a in a virtual environment for development:
 
 ```bash
 $ python -m venv venv
-$ ./venv/scripts/activate
+$ source venv/bin/activate
 $ pip install -e .[dev]
 ```
 
 Code is tested using tox:
 
 ```bash
 $ tox
@@ -218,21 +238,14 @@
 
 Quick tests can be handled by running pytest directly:
 
 ```bash
 $ pytest -p no:smtpd --cov
 ```
 
-Before submitting a pull request with your changes you should ensure that all imports are sorted and that the code passes linting with flake8.
-
-```bash
-$ isort .
-$ flake8 .
-```
-
 We include a [pre-commit](https://pre-commit.com/) configuration file to automate checks and clean up imports before pushing code. In order to install pre-commit git hooks:
 
 ```bash
 $ pip install pre-commit
 $ pre-commit install
 ```
```

### Comparing `smtpdfix-0.5.1/README.md` & `smtpdfix-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -169,19 +169,28 @@
 Many libraries for sending email have built-in methods for testing and using these methods should generally be prefered over SMTPDFix. Some known solutions:
 
 + **fastapi-mail**: has a `record_messsages()` method to intercept the mail. Instructions on how to suppress the sending of mail and implement it can be seen at [https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail](https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail)
 + **flask-mail**: has a method to suppress sending and capture the email for testing purposes. [Instructions](https://pythonhosted.org/Flask-Mail/#unit-tests-and-suppressing-emails)
 
 ## Developing
 
-To develop and test smtpdfix you will need to install [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests, [isort](https://pycqa.github.io/isort/) to sort imports and [flake8](https://flake8.pycqa.org/en/latest/) to lint. To install in a virtual environment for development:
+To develop and test smtpdfix you will need to install:
++ [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests,
++ [pytest-cov](https://github.com/pytest-dev/pytest-cov) to ensure 100% code coverages,
++ [pytest-timeout](https://github.com/pytest-dev/pytest-timeout) so that tests timeout,
++ [isort](https://pycqa.github.io/isort/) to sort imports,
++ [flake8](https://flake8.pycqa.org/en/latest/) to lint,
++ [mypy](https://mypy.readthedocs.io/en/stable/) for type checking,, and finally
++ [tox](https://tox.wiki/) to run a complete set of tests.
+
+To install all of these in a in a virtual environment for development:
 
 ```bash
 $ python -m venv venv
-$ ./venv/scripts/activate
+$ source venv/bin/activate
 $ pip install -e .[dev]
 ```
 
 Code is tested using tox:
 
 ```bash
 $ tox
@@ -189,21 +198,14 @@
 
 Quick tests can be handled by running pytest directly:
 
 ```bash
 $ pytest -p no:smtpd --cov
 ```
 
-Before submitting a pull request with your changes you should ensure that all imports are sorted and that the code passes linting with flake8.
-
-```bash
-$ isort .
-$ flake8 .
-```
-
 We include a [pre-commit](https://pre-commit.com/) configuration file to automate checks and clean up imports before pushing code. In order to install pre-commit git hooks:
 
 ```bash
 $ pip install pre-commit
 $ pre-commit install
 ```
```

### Comparing `smtpdfix-0.5.1/setup.cfg` & `smtpdfix-0.5.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 	LICENSE
 classifiers = 
 	Framework :: Pytest
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 project_urls = 
@@ -32,30 +31,31 @@
 packages = find:
 include_package_data = True
 install_requires = 
 	aiosmtpd
 	cryptography
 	portpicker
 	pytest
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 pytest11 = 
 	smtpd = smtpdfix.fixture
 
 [options.extras_require]
-dev = 
+testing = 
 	flake8
 	isort
+	mypy
 	pytest-asyncio
 	pytest-cov
 	pytest-timeout
+dev = 
+	smtpdfix[testing]
 	tox
-typing = 
-	mypy
 
 [options.package_data]
 smtpdfix = py.typed
 
 [options.packages.find]
 exclude = 
 	docs*
@@ -66,19 +66,19 @@
 testpaths = tests
 
 [coverage:run]
 branch = True
 source = smtpdfix
 
 [flake8]
-exclude = env,venv,.tox
+exclude = env,venv,.venv,.tox
 
 [mypy]
 files = smtpdfix
-python_version = 3.7
+python_version = 3.8
 disallow_any_generics = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
 no_implicit_optional = True
 no_implicit_reexport = True
```

### Comparing `smtpdfix-0.5.1/smtpdfix/authenticator.py` & `smtpdfix-0.5.2/smtpdfix/authenticator.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/smtpdfix/certs.py` & `smtpdfix-0.5.2/smtpdfix/certs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 import logging
 import socket
-from datetime import datetime, timedelta
+from collections import namedtuple
+from datetime import datetime, timedelta, timezone
 from ipaddress import ip_address
 from pathlib import Path
 from typing import Union
 
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509 import (BasicConstraints, CertificateBuilder, DNSName,
                                IPAddress, Name, NameAttribute,
                                SubjectAlternativeName, random_serial_number)
 from cryptography.x509.oid import NameOID
 
 log = logging.getLogger(__name__)
 
+Cert = namedtuple("Cert", ["cert", "key"], defaults=[None, None])
+
 
 def _generate_certs(path: Union[Path, str],
-                    days: int = 3652,
+                    days: int = 365,
                     key_size: int = 2048,
-                    separate_key: bool = False) -> None:
+                    separate_key: bool = False) -> Cert:
+    """DO NOT USE THIS FOR ANYTHING PRODUCTION RELATED, EVER!
+
+    Params:
+    - path: the `Path` or `str` of the directory to write the file to.
+    - days: an `int` of the number of days the certificate will be valid.
+    - key_size: an `int` representing the byte size of the key.
+    - separate_key: a `bool` representing whether the private key should be
+      written to a separate file.
+
+    Returns:
+    - By default returns a `tuple` with a `Path` to the certificate file
+      "cert.pem" and `None` for the key file.
+    - If separate_key was `True` a `tuple` with the paths to the certificate
+      file "cert.pem" and key file "key.pem" (each as a `Path`) will be
+      returned.
+
+    Changed as of v0.5.2
+    - Now returns a tuple of the location of the cert file and, if separate,
+      the key file. Previously always returned `None`
+    """
     # DO NOT USE THIS FOR ANYTHING PRODUCTION RELATED, EVER!
     # Generate private key
     # 2048 is the minimum that works as of 3.9
     key = rsa.generate_private_key(public_exponent=65537, key_size=key_size)
     key_file = "key.pem" if separate_key else "cert.pem"
     key_path = Path(path).joinpath(key_file)
     with open(key_path, "ab") as f:
@@ -59,18 +82,20 @@
     # ca=true, path_length=0 means it can only sign itself.
     constraints = BasicConstraints(ca=True, path_length=0)
 
     cert = (CertificateBuilder()
             .issuer_name(subject)
             .subject_name(subject)
             .serial_number(random_serial_number())
-            .not_valid_before(datetime.utcnow())
-            .not_valid_after(datetime.utcnow() + timedelta(days=days))
+            .not_valid_before(datetime.now(timezone.utc))
+            .not_valid_after(datetime.now(timezone.utc) + timedelta(days=days))
             .add_extension(SubjectAlternativeName(alt_names), critical=False)
             .public_key(key.public_key())
             .add_extension(constraints, critical=False)
             .sign(private_key=key, algorithm=hashes.SHA256()))
 
     cert_path = Path(path).joinpath("cert.pem")
     with open(cert_path, "ab") as f:
         f.write(cert.public_bytes(serialization.Encoding.PEM))
     log.debug("Certificate generated")
+
+    return Cert(cert_path, [key_path if separate_key else None])
```

### Comparing `smtpdfix-0.5.1/smtpdfix/configuration.py` & `smtpdfix-0.5.2/smtpdfix/configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import logging
 import os
 from pathlib import Path
-from typing import Any, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
 
 import portpicker
 
 from .event_handler import EventHandler
 
-PathType = Union[str, os.PathLike]
+log = logging.getLogger(__name__)
 
-_current_dir = Path(__file__).parent
+if TYPE_CHECKING:  # pragma: no cover
+    PathType = Union[str, os.PathLike[Any]]
+else:
+    PathType = Union[str, os.PathLike]
 
 
 def _strtobool(val: str) -> bool:
     """Convert a string representation of truth to true (1) or false (0).
 
     True values are "y", "yes", "t", "true", "on", and "1"; false values are
     "n", "no", "f", "false", "off", and "0".  Raises ValueError if "val" is
@@ -26,39 +30,59 @@
     elif val in ("n", "no", "f", "false", "off", "0"):
         return False
     else:
         raise ValueError(f"invalid truth value {val}")
 
 
 class Config():
-    def __init__(self) -> None:
+    """Holds all of the configuration values for the Controller.
 
+    Changed in v0.5.2:
+    - Removed the SSL_Cert_Path property
+    """
+    def __init__(self) -> None:
+        # Sets an event handler on the object
         self.OnChanged = EventHandler()
 
-        self._host = os.getenv("SMTPD_HOST")
+        self._host: Optional[str] = os.getenv("SMTPD_HOST", "localhost")
         self._port = int(
             os.getenv("SMTPD_PORT", portpicker.pick_unused_port())
         )
         self._ready_timeout = float(os.getenv("SMTPD_READY_TIMEOUT", 10.0))
         self._login_username = os.getenv("SMTPD_LOGIN_NAME", "user")
         self._login_password = os.getenv("SMTPD_LOGIN_PASSWORD", "password")
         self._enforce_auth = _strtobool(os.getenv("SMTPD_ENFORCE_AUTH",
                                                   "False"))
         self._auth_require_tls = _strtobool(os.getenv("SMTPD_AUTH_REQUIRE_TLS",
                                                       "True"))
-        self._ssl_cert_path: PathType = os.getenv(
-            "SMTPD_SSL_CERTS_PATH",
-            _current_dir.joinpath("certs"))
-        self._ssl_cert_files = (
-            os.getenv("SMTPD_SSL_CERTIFICATE_FILE", "./cert.pem"),
-            os.getenv("SMTPD_SSL_KEY_FILE"))
+        self._ssl_cert_files = (os.getenv("SMTPD_SSL_CERTIFICATE_FILE"),
+                                os.getenv("SMTPD_SSL_KEY_FILE"))
         self._use_starttls = _strtobool(os.getenv("SMTPD_USE_STARTTLS",
                                                   "False"))
         self._use_ssl = (_strtobool(os.getenv("SMTPD_USE_SSL", "False"))
                          or _strtobool(os.getenv("SMTPD_USE_TLS", "False")))
+        # Check to ensure that the _ssl_cert_files are either none or resolve
+        assert self._check_cert_files()
+
+    def _check_cert_files(self) -> bool:
+        """Check that the certificate and, optional, key files exist or are
+        None.
+
+        Returns:
+        - `True` if there are no errors.
+
+        Raises:
+        - FileNotFoundError if the certificate of key file is not None and does
+          resolve to a file.
+        """
+        for file_ in self._ssl_cert_files:
+            if file_ is not None and Path(file_).is_file() is False:
+                log.debug("File not found: verify cert and key config")
+                raise FileNotFoundError
+        return True
 
     def convert_to_bool(self, value: Any) -> bool:
         """Consistently convert to bool."""
         if isinstance(value, str):
             return bool(_strtobool(value))
         return bool(value)
 
@@ -122,33 +146,25 @@
 
     @auth_require_tls.setter
     def auth_require_tls(self, value: bool) -> None:
         self._auth_require_tls = self.convert_to_bool(value)
         self.OnChanged()
 
     @property
-    def ssl_certs_path(self) -> PathType:
-        return self._ssl_cert_path
-
-    @ssl_certs_path.setter
-    def ssl_certs_path(self, value: PathType) -> None:
-        self._ssl_cert_path = value
-        self.OnChanged()
-
-    @property
-    def ssl_cert_files(self) -> Tuple[str, Optional[str]]:
+    def ssl_cert_files(self) -> Tuple[Optional[str], Optional[str]]:
         return self._ssl_cert_files
 
     @ssl_cert_files.setter
     def ssl_cert_files(self,
                        value: Union[str, Tuple[str, Optional[str]]]) -> None:
         if isinstance(value, tuple):
             self._ssl_cert_files = (value[0], value[1])
         else:
             self._ssl_cert_files = (value, None)
+        assert self._check_cert_files()
         self.OnChanged()
 
     @property
     def use_starttls(self) -> bool:
         return self._use_starttls
 
     @use_starttls.setter
```

### Comparing `smtpdfix-0.5.1/smtpdfix/controller.py` & `smtpdfix-0.5.2/smtpdfix/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from socket import create_connection
 from ssl import CERT_OPTIONAL, Purpose, SSLContext, create_default_context
 from typing import Any, Coroutine, List, Optional
 
 from aiosmtpd.controller import Controller, get_localhost
 
 from .authenticator import Authenticator
-from .configuration import Config, PathType
+from .configuration import Config
 from .handlers import AuthMessage
 from .smtp import _SMTP
 
 AsyncServer = asyncio.base_events.Server
 ServerCoroutine = Coroutine[Any, Any, asyncio.base_events.Server]
 
 log = logging.getLogger(__name__)
@@ -81,35 +81,28 @@
                      tls_context=context,
                      authenticator=self._authenticator)
 
     def _get_ssl_context(self) -> SSLContext:
         if self._ssl_context is not None:
             return self._ssl_context
 
-        certs_path = Path(self.config.ssl_certs_path).resolve()
         cert_file, key_file = self.config.ssl_cert_files
 
-        def _resolve_file(basepath: Path, file_: PathType) -> str:
-            # Resolve the file paths in order:
-            #   1. if the file exists return the path as string
-            #   2. try to combine basepath and the filename and if that exists
-            #      return as a string.
+        def _resolve_file(file_: Optional[str]) -> str:
             # NB: the paths are returned as strings becuase PYPY3 doesn't
             # support paths in sslcontext.load_cert_chain()
-            if Path(file_).is_file():
+            if file_ and Path(file_).is_file():
                 return str(Path(file_))
-            elif basepath.joinpath(file_).resolve().is_file():
-                return str(basepath.joinpath(file_).resolve())
 
             raise FileNotFoundError(errno.ENOENT,
                                     strerror(errno.ENOENT),
                                     file_)
 
-        cert_path = _resolve_file(certs_path, cert_file)
-        key_path = _resolve_file(certs_path, key_file) if key_file else None
+        cert_path = _resolve_file(cert_file)
+        key_path = _resolve_file(key_file) if key_file else None
 
         context = create_default_context(Purpose.CLIENT_AUTH)
         context.check_hostname = False
         context.load_verify_locations(cert_path)
         context.load_cert_chain(cert_path, keyfile=key_path)
         return context
```

### Comparing `smtpdfix-0.5.1/smtpdfix/event_handler.py` & `smtpdfix-0.5.2/smtpdfix/event_handler.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/smtpdfix/fixture.py` & `smtpdfix-0.5.2/smtpdfix/fixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,14 @@
     Example:
         def test_mail(smtpd):
             from smtplib import SMTP
             with SMTP(smtpd.hostname, smtpd.port) as client:
                 code, resp = client.noop()
                 assert code == 250
     """
-    if os.getenv("SMTPD_SSL_CERTS_PATH") is None:
+    if os.getenv("SMTPD_SSL_CERTIFICATE_FILE") is None:
         path = tmp_path_factory.mktemp("certs")
-        _generate_certs(path)
-        os.environ["SMTPD_SSL_CERTS_PATH"] = str(path.resolve())
+        cert, _ = _generate_certs(path, separate_key=False)
+        os.environ["SMTPD_SSL_CERTIFICATE_FILE"] = str(cert.resolve())
 
     with SMTPDFix() as fixture:
         yield fixture
```

### Comparing `smtpdfix-0.5.1/smtpdfix/handlers.py` & `smtpdfix-0.5.2/smtpdfix/handlers.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/smtpdfix.egg-info/PKG-INFO` & `smtpdfix-0.5.2/smtpdfix.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: smtpdfix
-Version: 0.5.1
+Version: 0.5.2
 Summary: A SMTP server for use as a pytest fixture that implements encryption and authentication for testing.
 Home-page: https://github.com/bebleo/smtpdfix
 Author: James Warne
 Author-email: bebleo@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/bebleo/smtpdfix
 Project-URL: Documentation, https://github.com/bebleo/smtpdfix#readme
 Project-URL: Issues, https://github.com/bebleo/smtpdfix/issues
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: typing
 License-File: LICENSE
+Requires-Dist: aiosmtpd
+Requires-Dist: cryptography
+Requires-Dist: portpicker
+Requires-Dist: pytest
+Provides-Extra: testing
+Requires-Dist: flake8; extra == "testing"
+Requires-Dist: isort; extra == "testing"
+Requires-Dist: mypy; extra == "testing"
+Requires-Dist: pytest-asyncio; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-timeout; extra == "testing"
+Provides-Extra: dev
+Requires-Dist: smtpdfix[testing]; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # SMTPDFix: Test email, locally
 
 ![build](https://github.com/bebleo/bebleo_smtpd_fixture/workflows/build/badge.svg)
 
 A simple SMTP server based on `aiosmtpd` for use as a fixture with pytest that supports encryption and authentication. All this does is receives messages and appends them to a list as an `email.Message`.
 
@@ -198,19 +209,28 @@
 Many libraries for sending email have built-in methods for testing and using these methods should generally be prefered over SMTPDFix. Some known solutions:
 
 + **fastapi-mail**: has a `record_messsages()` method to intercept the mail. Instructions on how to suppress the sending of mail and implement it can be seen at [https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail](https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail)
 + **flask-mail**: has a method to suppress sending and capture the email for testing purposes. [Instructions](https://pythonhosted.org/Flask-Mail/#unit-tests-and-suppressing-emails)
 
 ## Developing
 
-To develop and test smtpdfix you will need to install [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests, [isort](https://pycqa.github.io/isort/) to sort imports and [flake8](https://flake8.pycqa.org/en/latest/) to lint. To install in a virtual environment for development:
+To develop and test smtpdfix you will need to install:
++ [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests,
++ [pytest-cov](https://github.com/pytest-dev/pytest-cov) to ensure 100% code coverages,
++ [pytest-timeout](https://github.com/pytest-dev/pytest-timeout) so that tests timeout,
++ [isort](https://pycqa.github.io/isort/) to sort imports,
++ [flake8](https://flake8.pycqa.org/en/latest/) to lint,
++ [mypy](https://mypy.readthedocs.io/en/stable/) for type checking,, and finally
++ [tox](https://tox.wiki/) to run a complete set of tests.
+
+To install all of these in a in a virtual environment for development:
 
 ```bash
 $ python -m venv venv
-$ ./venv/scripts/activate
+$ source venv/bin/activate
 $ pip install -e .[dev]
 ```
 
 Code is tested using tox:
 
 ```bash
 $ tox
@@ -218,21 +238,14 @@
 
 Quick tests can be handled by running pytest directly:
 
 ```bash
 $ pytest -p no:smtpd --cov
 ```
 
-Before submitting a pull request with your changes you should ensure that all imports are sorted and that the code passes linting with flake8.
-
-```bash
-$ isort .
-$ flake8 .
-```
-
 We include a [pre-commit](https://pre-commit.com/) configuration file to automate checks and clean up imports before pushing code. In order to install pre-commit git hooks:
 
 ```bash
 $ pip install pre-commit
 $ pre-commit install
 ```
```

### Comparing `smtpdfix-0.5.1/smtpdfix.egg-info/SOURCES.txt` & `smtpdfix-0.5.2/smtpdfix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/tests/conftest.py` & `smtpdfix-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/tests/test_configuration.py` & `smtpdfix-0.5.2/tests/test_configuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import functools
+from pathlib import Path  # noqa: F401
 from typing import Any, Generator, List
+from unittest.mock import MagicMock, patch
 
 import pytest
 
 from smtpdfix.configuration import Config, _strtobool
 from smtpdfix.event_handler import EventHandler
 
 values = [
@@ -17,15 +19,14 @@
     ("enforce_auth", "True", True, bool),
     ("enforce_auth", True, True, bool),
     ("enforce_auth", 1, True, bool),
     ("auth_require_tls", 0, False, bool),
     ("auth_require_tls", "0", False, bool),
     ("auth_require_tls", False, False, bool),
     ("auth_require_tls", "False", False, bool),
-    ("ssl_certs_path", "./certs", "./certs", str),
     ("ssl_cert_files",
         ("./certs/cert.pem", "./certs/key.pem"),
         ("./certs/cert.pem", "./certs/key.pem"),
         tuple),
     ("ssl_cert_files",
         "./certs/key.pem",
         ("./certs/key.pem", None),
@@ -65,23 +66,40 @@
 
 def test_init() -> None:
     config = Config()
     assert isinstance(config, Config)
 
 
 @pytest.mark.parametrize("attr, value, expected, type", values)
-def test_set_values(attr: str, value: Any, expected: Any, type: Any) -> None:
+@patch("smtpdfix.configuration.Path.is_file")
+def test_set_values(mock_is_file: Any,
+                    attr: str,
+                    value: Any,
+                    expected: Any,
+                    type: Any) -> None:
+    mock_is_file.return_value = True
     config = Config()
     setattr(config, attr, value)
     assert isinstance(getattr(config, attr), type)
     assert getattr(config, attr) == expected
 
 
+def test_file_not_found():
+    config = Config()
+    with pytest.raises(FileNotFoundError):
+        config.ssl_cert_files = "rubbish"
+
+
 @pytest.mark.parametrize("prop", props)
-def test_event_handler_fires(prop: str, handler: FakeHandler) -> None:
+@patch("smtpdfix.configuration.Path.__new__")
+def test_event_handler_fires(mock_Path: MagicMock,
+                             prop: str,
+                             handler: FakeHandler) -> None:
+    mock_Path.return_value = MagicMock()
+    mock_Path.is_file = True
     config = Config()
     result: List[Any] = []
     config.OnChanged += functools.partial(handler.handle, result)
     setattr(config, prop, 1)
     assert result.pop() is True
```

### Comparing `smtpdfix-0.5.1/tests/test_controller.py` & `smtpdfix-0.5.2/tests/test_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,30 +53,25 @@
         client.starttls()
         client.send_message(msg)
 
     assert len(server.messages) == 1
 
 
 def test_missing_certs(request: FixtureRequest, msg: EmailMessage) -> None:
-    with pytest.raises(FileNotFoundError) as error:
-        _config = Config()
-        _config.use_starttls = True
-        _config.ssl_certs_path = "."
-        _authenticator = _Authenticator(config=_config)
-        server = AuthController(hostname=_config.host,
-                                port=_config.port,
-                                config=_config,
-                                authenticator=_authenticator)
-        request.addfinalizer(server.stop)
+    _config = Config()
+    _config.use_starttls = True
+    _config.ssl_cert_files = None
+    _authenticator = _Authenticator(config=_config)
+    server = AuthController(hostname=_config.host,
+                            port=_config.port,
+                            config=_config,
+                            authenticator=_authenticator)
+    with pytest.raises(FileNotFoundError):
         server.start()
-
-        with SMTP(server.hostname, server.port) as client:
-            client.send_message(msg)
-
-    assert error.type == FileNotFoundError
+        server.stop()
 
 
 def test_custom_cert_and_key(request: FixtureRequest,
                              tmp_path_factory: TempPathFactory,
                              msg: EmailMessage) -> None:
     path = tmp_path_factory.mktemp("certs")
     _generate_certs(path, separate_key=True)
```

### Comparing `smtpdfix-0.5.1/tests/test_fixture.py` & `smtpdfix-0.5.2/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/tests/test_smtp.py` & `smtpdfix-0.5.2/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `smtpdfix-0.5.1/tests/test_smtpdfix.py` & `smtpdfix-0.5.2/tests/test_smtpdfix.py`

 * *Files identical despite different names*

