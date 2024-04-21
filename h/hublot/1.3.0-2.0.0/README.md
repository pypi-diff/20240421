# Comparing `tmp/hublot-1.3.0.tar.gz` & `tmp/hublot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hublot-1.3.0.tar", last modified: Sun Jan 29 18:41:26 2023, max compression
+gzip compressed data, was "hublot-2.0.0.tar", last modified: Sun Apr 21 14:35:41 2024, max compression
```

## Comparing `hublot-1.3.0.tar` & `hublot-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-29 18:41:26.042701 hublot-1.3.0/
--rw-rw-r--   0 herve     (1000) herve     (1000)       23 2021-11-15 20:26:52.000000 hublot-1.3.0/MANIFEST.in
--rw-rw-r--   0 herve     (1000) herve     (1000)      342 2023-01-29 18:41:26.042701 hublot-1.3.0/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)       73 2022-05-27 21:23:52.000000 hublot-1.3.0/README.md
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-29 18:41:26.034701 hublot-1.3.0/hublot/
--rw-rw-r--   0 herve     (1000) herve     (1000)      355 2023-01-29 18:15:19.000000 hublot-1.3.0/hublot/__init__.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-29 18:41:26.038701 hublot-1.3.0/hublot/cache/
--rw-rw-r--   0 herve     (1000) herve     (1000)      140 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/cache/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     4968 2021-11-15 20:38:54.000000 hublot-1.3.0/hublot/cache/binaryblob.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3175 2022-05-27 21:23:52.000000 hublot-1.3.0/hublot/cache/cache.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3419 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/cache/key.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3079 2021-11-16 07:21:29.000000 hublot-1.3.0/hublot/cache/storage.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    10731 2022-05-27 21:23:52.000000 hublot-1.3.0/hublot/client.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1238 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/courtesy.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2317 2022-05-27 21:23:52.000000 hublot-1.3.0/hublot/decorator.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1070 2023-01-29 18:34:16.000000 hublot-1.3.0/hublot/exceptions.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2112 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/logs.py
--rw-rw-r--   0 herve     (1000) herve     (1000)        0 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/py.typed
--rw-rw-r--   0 herve     (1000) herve     (1000)     2337 2021-11-15 20:26:52.000000 hublot-1.3.0/hublot/utils.py
--rw-rw-r--   0 herve     (1000) herve     (1000)       49 2023-01-29 18:35:27.000000 hublot-1.3.0/hublot/version.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-29 18:41:26.038701 hublot-1.3.0/hublot.egg-info/
--rw-rw-r--   0 herve     (1000) herve     (1000)      342 2023-01-29 18:41:25.000000 hublot-1.3.0/hublot.egg-info/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)      818 2023-01-29 18:41:25.000000 hublot-1.3.0/hublot.egg-info/SOURCES.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-01-29 18:41:25.000000 hublot-1.3.0/hublot.egg-info/dependency_links.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2021-11-16 07:12:35.000000 hublot-1.3.0/hublot.egg-info/not-zip-safe
--rw-rw-r--   0 herve     (1000) herve     (1000)       65 2023-01-29 18:41:25.000000 hublot-1.3.0/hublot.egg-info/requires.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        7 2023-01-29 18:41:25.000000 hublot-1.3.0/hublot.egg-info/top_level.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)       38 2023-01-29 18:41:26.042701 hublot-1.3.0/setup.cfg
--rw-rw-r--   0 herve     (1000) herve     (1000)     1143 2022-05-27 21:26:13.000000 hublot-1.3.0/setup.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-01-29 18:41:26.042701 hublot-1.3.0/test/
--rw-rw-r--   0 herve     (1000) herve     (1000)      133 2021-01-17 18:09:21.000000 hublot-1.3.0/test/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7381 2021-11-15 20:26:52.000000 hublot-1.3.0/test/conftest.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     5814 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_cache.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    11002 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_cache_keys.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     5859 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_cache_max_age.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7512 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_client.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3246 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_cookies.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3361 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_courtesy_sleep.py
--rw-rw-r--   0 herve     (1000) herve     (1000)      608 2023-01-29 18:29:04.000000 hublot-1.3.0/test/test_error_handling.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1790 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_logging.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7341 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_retry_decorator.py
--rw-rw-r--   0 herve     (1000) herve     (1000)      680 2022-05-27 21:23:52.000000 hublot-1.3.0/test/test_threading.py
--rw-rw-r--   0 herve     (1000) herve     (1000)      392 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_types.py
--rw-rw-r--   0 herve     (1000) herve     (1000)      975 2021-11-15 20:26:52.000000 hublot-1.3.0/test/test_user_agent.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2195 2021-11-15 20:26:52.000000 hublot-1.3.0/test/utils.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 14:35:41.437843 hublot-2.0.0/
+-rw-rw-r--   0 herve     (1000) herve     (1000)       23 2023-03-06 11:52:04.000000 hublot-2.0.0/MANIFEST.in
+-rw-r--r--   0 herve     (1000) herve     (1000)      537 2024-04-21 14:35:41.437843 hublot-2.0.0/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1058 2024-04-21 14:22:59.000000 hublot-2.0.0/README.md
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 14:35:41.433843 hublot-2.0.0/hublot/
+-rw-rw-r--   0 herve     (1000) herve     (1000)      767 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/__init__.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 14:35:41.433843 hublot-2.0.0/hublot/cache/
+-rw-rw-r--   0 herve     (1000) herve     (1000)      305 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/cache/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3856 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/cache/binaryblob.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2918 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/cache/cache.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3502 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/cache/key.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3132 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/cache/storage.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5827 2024-04-21 14:22:59.000000 hublot-2.0.0/hublot/client.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3102 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/compile.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1531 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/config.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     9853 2024-04-21 14:22:59.000000 hublot-2.0.0/hublot/datastructures.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2523 2024-04-21 14:22:59.000000 hublot-2.0.0/hublot/decorator.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2446 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/logs.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)        0 2023-03-06 11:52:04.000000 hublot-2.0.0/hublot/py.typed
+-rw-rw-r--   0 herve     (1000) herve     (1000)       49 2024-04-21 14:22:35.000000 hublot-2.0.0/hublot/version.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 14:35:41.437843 hublot-2.0.0/hublot.egg-info/
+-rw-r--r--   0 herve     (1000) herve     (1000)      537 2024-04-21 14:35:41.000000 hublot-2.0.0/hublot.egg-info/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)      831 2024-04-21 14:35:41.000000 hublot-2.0.0/hublot.egg-info/SOURCES.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2024-04-21 14:35:41.000000 hublot-2.0.0/hublot.egg-info/dependency_links.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-03-12 08:39:51.000000 hublot-2.0.0/hublot.egg-info/not-zip-safe
+-rw-rw-r--   0 herve     (1000) herve     (1000)      106 2024-04-21 14:35:41.000000 hublot-2.0.0/hublot.egg-info/requires.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        7 2024-04-21 14:35:41.000000 hublot-2.0.0/hublot.egg-info/top_level.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)       38 2024-04-21 14:35:41.437843 hublot-2.0.0/setup.cfg
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1298 2024-04-21 14:22:35.000000 hublot-2.0.0/setup.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-04-21 14:35:41.437843 hublot-2.0.0/test/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5844 2024-04-21 14:22:59.000000 hublot-2.0.0/test/test_cache.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    11664 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_cache_keys.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5987 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_cache_max_age.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     8008 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_client.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3240 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_cookies.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2973 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_courtesy_sleep.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3103 2024-04-21 14:22:59.000000 hublot-2.0.0/test/test_engine_pool_rotation.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3295 2024-04-21 14:22:59.000000 hublot-2.0.0/test/test_engines.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)      260 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_error_handling.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3175 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_headers.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2022 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_logging.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     7281 2024-04-21 14:22:59.000000 hublot-2.0.0/test/test_retry_decorator.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)      685 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_threading.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1077 2024-04-21 14:22:35.000000 hublot-2.0.0/test/test_user_agent.py
```

### Comparing `hublot-1.3.0/hublot/cache/binaryblob.py` & `hublot-2.0.0/hublot/cache/binaryblob.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,142 +10,117 @@
 
 # standards
 from codecs import getwriter
 from io import BytesIO
 import re
 from typing import Callable, Optional, Tuple
 
-# 3rd parties
-from requests import PreparedRequest, Response
-from requests.structures import CaseInsensitiveDict
+# hublot
+from ..datastructures import CompiledRequest, Headers, Response
 
 
-EOL = '\r\n'
-EOL_BYTES = EOL.encode('UTF-8')
+EOL = "\r\n"
+EOL_BYTES = EOL.encode("UTF-8")
 EOL_LEN = len(EOL)
 
 
-Writer = getwriter('UTF-8')  # pylint: disable=invalid-name
+Writer = getwriter("UTF-8")  # pylint: disable=invalid-name
 
 
 def compose_binary_blob(res: Response) -> bytes:
     output = BytesIO()
     write = Writer(output).write
     _compose_request_blob(res.request, output, write)
     _compose_response_blob(res, output, write)
     return output.getvalue()
 
 
 def _compose_request_blob(
-    preq: PreparedRequest,
+    creq: CompiledRequest,
     output: BytesIO,
     write: Callable[[str], None],
 ) -> None:
-
-    write(f'{preq.method} {preq.url}{EOL}')
-    for key, value in sorted(preq.headers.items()):
-        write(f'{key}: {value}{EOL}')
+    write(f"{creq.method} {creq.url}{EOL}")
+    for key, value in sorted(creq.headers.items()):
+        write(f"{key}: {value}{EOL}")
     write(EOL)
-    if 'Content-Length' in preq.headers:
-        body = b'' if preq.body is None else preq.body
-        content_length = int(preq.headers['Content-Length'])
+    if "Content-Length" in creq.headers:
+        body = b"" if creq.data is None else creq.data
+        content_length = int(creq.headers["Content-Length"])
         if content_length != len(body):
             # Don't write it out because we won't be able to read it back
-            raise Exception(f'body has {len(body)} bytes but Content-Length is {content_length}')
-        if isinstance(body, str):
-            # `PreparedRequest.prepare_body` leaves `body` as a `str` if `data` was a dict
-            body_bytes = body.encode('UTF-8')
-        else:
-            body_bytes = body
-        output.write(body_bytes)
+            raise Exception(f"body has {len(body)} bytes but Content-Length is {content_length}")
+        output.write(body)
         write(EOL)
+    else:
+        assert creq.data is None, "compile_request should've set the Content-Length"
     write(EOL)
 
 
 def _compose_response_blob(
     res: Response,
     output: BytesIO,
     write: Callable[[str], None],
 ) -> None:
-
-    write(f'HTTP {res.status_code} {res.reason}{EOL}')
-    if hasattr(res.raw, '_fp'):
-        # Using `res.raw._fp.headers` rather than `res.headers` means we store repeated headers (e.g. Set-Cookie) as separate lines
-        header_items = res.raw._fp.headers.items()  # pylint: disable=protected-access
-    else:
-        # Sometimes however, in tests especially, `raw` might've been replaced by some other file object, and has no `_fp`, so fall
-        # back to this:
-        header_items = res.headers.items()
-    for key, value in sorted(header_items):
-        write(f'{key}: {value}{EOL}')
+    write(f"HTTP {res.status_code} {res.reason}{EOL}")
+    for key, value in sorted(res.headers.items()):
+        write(f"{key}: {value}{EOL}")
     write(EOL)
     if res.content is not None:
         output.write(res.content)
 
 
 def parse_binary_blob(data: bytes) -> Response:
-    # pylint: disable=protected-access
     pos = 0
-    _method_unused, url, pos = _parse_line(data, pos, r'^(\w+) (.+)$')
-    _headers_unused, _body_unused, pos = _parse_message(data, pos)
-    status_code, reason, pos = _parse_line(data, pos, r'^HTTP (\d+) (.*)$')
-    res = Response()
-    res.status_code = int(status_code)
-    res.reason = reason
-    res.url = url
-    res.headers, res._content, pos = _parse_message(data, pos, read_to_end=True)
-    res._content_consumed = True  # type: ignore[attr-defined]
-    return res
+    method, url, pos = _parse_line(data, pos, r"^(\w+) (.+)$")
+    req_headers, req_body, pos = _parse_message(data, pos)
+    creq = CompiledRequest(
+        url=url,
+        method=method,
+        headers=req_headers,
+        data=req_body,
+        num_retries=0,
+    )
+    status_code, reason, pos = _parse_line(data, pos, r"^HTTP (\d+) (.*)$")
+    res_headers, res_body, pos = _parse_message(data, pos, read_to_end=True)
+    assert res_body is not None  # since we passed `read_to_end=True`
+    return Response(
+        request=creq,
+        from_cache=True,
+        history=[],  # set elsewhere
+        status_code=int(status_code),
+        reason=reason,
+        headers=res_headers,
+        content=res_body,
+    )
 
 
 def _parse_message(
     data: bytes,
     pos: int,
     read_to_end: bool = False,
-) -> Tuple[CaseInsensitiveDict, Optional[bytes], int]:
-
-    headers = MultipleCaseInsensitiveDict()
-    while data[pos : pos+EOL_LEN] != EOL_BYTES:
-        key, value, pos = _parse_line(data, pos, r'^([^:]+): (.*)$')
+) -> Tuple[Headers, Optional[bytes], int]:
+    headers = Headers()
+    while data[pos : pos + EOL_LEN] != EOL_BYTES:
+        key, value, pos = _parse_line(data, pos, r"^([^:]+): (.*)$")
         headers[key] = value
     pos += EOL_LEN
     body: Optional[bytes] = None
     if read_to_end:
-        body = data[pos : ]
+        body = data[pos:]
         pos = len(data)
-    elif headers.get('Content-Length'):
-        length = int(headers['Content-Length'])
-        body = data[pos : pos+length]
+    elif headers.get("Content-Length"):
+        length = int(headers["Content-Length"])
+        body = data[pos : pos + length]
         pos += length + (2 * EOL_LEN)
     else:
         pos += EOL_LEN
     return headers, body, pos
 
 
 def _parse_line(data: bytes, pos: int, regex: str):
     eol_pos = data.find(EOL_BYTES, pos)
-    line = data[pos : eol_pos].decode('UTF-8')
+    line = data[pos:eol_pos].decode("UTF-8")
     match = re.search(regex, line)
-    if not match:
+    if not match:  # pragma: no cover
         raise ValueError(repr(line))
     return (*match.groups(), eol_pos + EOL_LEN)
-
-
-
-class MultipleCaseInsensitiveDict(CaseInsensitiveDict):  # pylint: disable=too-many-ancestors
-
-    def __setitem__(self, key, item):
-        values = self.get_all(key, [])
-        values.append(item)
-        super().__setitem__(key, values)
-
-    def __getitem__(self, key):
-        values = super().__getitem__(key)
-        return ', '.join(values)
-
-    def get_all(self, key, failobj=None):
-        # Deliberately copying the interface of `email.message.EmailMessage.get_all` for consistency's sake, though we're not
-        # actually using this object in place of that.
-        try:
-            return super().__getitem__(key)
-        except KeyError:
-            return failobj
```

### Comparing `hublot-1.3.0/hublot/cache/key.py` & `hublot-2.0.0/hublot/cache/key.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 # standards
 from dataclasses import dataclass, replace
 from hashlib import md5
 import re
 from typing import Optional, Tuple, Union
 
-# 3rd parties
-from requests import PreparedRequest
+# hublot
+from ..config import Config
+from ..datastructures import CompiledRequest
 
 
-UserSpecifiedCacheKey = Union['CacheKey', Tuple[str, ...], str]
+UserSpecifiedCacheKey = Union["CacheKey", Tuple[str, ...], str]
 
 
 @dataclass(frozen=True, order=True)
 class CacheKey:
 
     parts: Tuple[str, ...]
     sequence_num: int = 0
@@ -22,70 +23,65 @@
     @property
     def path_parts(self) -> Tuple[str, ...]:
         parts = [
             # chars that *must* be escaped:
             #  * all chars that aren't valid in Windows file names
             #  * slashes, backslashes and null chars
             #  * dots, so that ".4" at the end unambiguously identifies a sequence num (and also avoids directory traversal vulns)
-            re.sub(r'[^\w\-]', lambda m: f'%{ord(m.group()):02X}', part)
+            re.sub(r"[^\w\-]", lambda m: f"%{ord(m.group()):02X}", part)
             for part in self.parts
         ]
         if self.sequence_num > 0:
-            parts[-1] += f'.{self.sequence_num}'
+            parts[-1] += f".{self.sequence_num}"
         return tuple(parts)
 
     @property
     def unique_str(self) -> str:
         # NB the string we return isn't for use in paths, so we can use '/' as the separator regardless of platform. Slashes have
         # been removed from the parts, so this is unambiguous.
-        return '/'.join(self.path_parts)
+        return "/".join(self.path_parts)
 
     def next_in_sequence(self):
         return replace(self, sequence_num=self.sequence_num + 1)
 
     @classmethod
     def from_path_parts(cls, parts):
-        seq_match = re.search(r'\.(\d+)$', parts[-1])
+        seq_match = re.search(r"\.(\d+)$", parts[-1])
         if seq_match:
             sequence_num = int(seq_match.group(1))
-            parts[-1] = parts[-1][:seq_match.start()]
+            parts[-1] = parts[-1][: seq_match.start()]
         else:
             sequence_num = 0
         return cls(
-            parts=tuple(
-                re.sub(r'%([0-9a-fA-F]{2})', lambda m: chr(int(m.group(1), 16)), p)
-                for p in parts
-            ),
+            parts=tuple(re.sub(r"%([0-9a-fA-F]{2})", lambda m: chr(int(m.group(1), 16)), p) for p in parts),
             sequence_num=sequence_num,
         )
 
     @classmethod
-    def compute(cls, preq: PreparedRequest) -> 'CacheKey':
+    def compute(cls, creq: CompiledRequest, config: Config) -> "CacheKey":
         # NB we don't normalise the order of the `params` dict or `data` dict. If running in Python 3.6+, where dicts preserve
         # their insertion order, multiple calls from the same code, where the params are defined in the same order, will hit the
         # same cache key. In previous versions, maybe not, so in 3.5 and before params and body should be serialised before being
         # sent to Hublot.
-        headers = sorted(
-            (key.title(), value)
-            for key, value in preq.headers.items()
-        )
+        headers_ignored_by_cache = config.headers_ignored_by_cache or set()
+        headers = sorted((key.title(), value) for key, value in creq.headers.items() if key not in headers_ignored_by_cache)
         key = (
-            preq.method,
-            preq.url,
+            creq.method,
+            creq.url,
             headers,
-            preq.body,
+            creq.data,
         )
         # Shortening to 16 chars means it's easier to copy-paste, takes less space in the terminal, etc. Seems like a flimsy reason
         # for increasing the chances of a collision, but at 2^64 bits these chances are still comfortably negligible.
-        hashed = md5(repr(key).encode('UTF-8')).hexdigest()[:16]
+        hashed = md5(repr(key).encode("UTF-8")).hexdigest()[:16]
         return cls((hashed[:3], hashed[3:]))
 
     @classmethod
     def parse(cls, user_specified_key: Optional[UserSpecifiedCacheKey]):
         if isinstance(user_specified_key, CacheKey):
             return user_specified_key
         elif isinstance(user_specified_key, tuple):
             return cls(user_specified_key)
         elif isinstance(user_specified_key, str):
-            return cls(tuple(user_specified_key.strip('/').split('/')))
+            return cls(tuple(user_specified_key.strip("/").split("/")))
         else:
             raise TypeError(repr(user_specified_key))
```

### Comparing `hublot-1.3.0/hublot/cache/storage.py` & `hublot-2.0.0/hublot/cache/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 #!/usr/bin/env python3
 
 # standards
+from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 import gzip
 import logging
 from pathlib import Path
 import re
 from typing import Iterable, Optional
 
-# 3rd parties
-from requests import Response
-
 # hublot
+from ..datastructures import Response
 from .binaryblob import compose_binary_blob, parse_binary_blob
 from .key import CacheKey
 
 
-class Storage:  # pragma: no cover
+class Storage(ABC):  # pragma: no-cover
 
-    def read(self, key: CacheKey, max_age: Optional[timedelta] = None) -> Optional[Response]:
-        raise NotImplementedError
+    @abstractmethod
+    def read(self, key: CacheKey, max_age: Optional[timedelta] = None) -> Optional[Response]: ...
 
-    def write(self, key: CacheKey, response: Response) -> None:
-        raise NotImplementedError
+    @abstractmethod
+    def write(self, key: CacheKey, response: Response) -> None: ...
 
-    def iter_all_keys(self) -> Iterable[CacheKey]:
-        raise NotImplementedError
+    @abstractmethod
+    def iter_all_keys(self) -> Iterable[CacheKey]: ...
 
-    def prune(self, max_age: timedelta) -> None:
-        raise NotImplementedError
+    @abstractmethod
+    def prune(self, max_age: timedelta) -> None: ...
 
 
 class DiskStorage(Storage):
 
-    def __init__(self, root_path: Path):
+    def __init__(self, root_path: Path) -> None:
         self.root_path = root_path
 
     def read(self, key: CacheKey, max_age: Optional[timedelta] = None) -> Optional[Response]:
         file_path = self._file_path(key)
         if not file_path.exists():
             return None
         if max_age is not None:
             file_age = current_datetime() - datetime.fromtimestamp(file_path.stat().st_mtime)
             if file_age > max_age:
                 return None
         try:
-            with gzip.open(file_path, 'rb') as file_in:
+            with gzip.open(file_path, "rb") as file_in:
                 return parse_binary_blob(file_in.read())
-        except gzip.BadGzipFile as error:
+        except gzip.BadGzipFile as error:  # pragma: no cover
             logging.error("Couldn't read %s: %s", file_path, error)
             return None
 
     def write(self, key: CacheKey, response: Response) -> None:
         file_path = self._file_path(key)
         file_path.parent.mkdir(parents=True, exist_ok=True)
-        with gzip.open(file_path, 'wb') as file_out:
+        with gzip.open(file_path, "wb") as file_out:
             file_out.write(compose_binary_blob(response))
 
     def iter_all_keys(self) -> Iterable[CacheKey]:
         for file_path in self._iter_all_files():
             parts = list(file_path.relative_to(self.root_path).parts)
-            parts[-1] = re.sub(r'\.gz$', '', file_path.name)
+            parts[-1] = re.sub(r"\.gz$", "", file_path.name)
             yield CacheKey.from_path_parts(parts)
 
     def prune(self, max_age: timedelta) -> None:
         now = current_datetime()
         dirs_to_check = set()
         for file_path in self._iter_all_files():
             file_age = now - datetime.fromtimestamp(file_path.stat().st_mtime)
             if file_age > max_age:
                 file_path.unlink()
                 dirs_to_check.add(file_path.parent)
         for dir_path in dirs_to_check:
-            while not next(dir_path.iterdir(), None):
+            while dir_path != self.root_path and not next(dir_path.iterdir(), None):
                 dir_path.rmdir()
                 dir_path = dir_path.parent
 
     def _iter_all_files(self) -> Iterable[Path]:
-        return self.root_path.glob('**/*.gz')
+        return self.root_path.glob("**/*.gz")
 
     def _file_path(self, key: CacheKey) -> Path:
         file_path = self.root_path / Path(*key.path_parts)
-        if not file_path.suffix == '.gz':
-            file_path = file_path.parent / f'{file_path.name}.gz'
+        if not file_path.suffix == ".gz":
+            file_path = file_path.parent / f"{file_path.name}.gz"
         return file_path
 
 
 def current_datetime() -> datetime:
     # This is put in a separate function so that tests can patch that function
     return datetime.now()
```

### Comparing `hublot-1.3.0/hublot/decorator.py` & `hublot-2.0.0/hublot/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 from collections.abc import Generator, Iterator, Sized
 from contextlib import contextmanager
 from dataclasses import dataclass
 from functools import wraps
 import threading
 from time import sleep
 from typing import Callable, Optional, Sequence
+from uuid import UUID, uuid4
 
 # hublot
-from .exceptions import ScraperError
+from .datastructures import HublotException
 from .logs import LOGGER
 
 
 @dataclass
 class ThreadLocalStackFrame:
-    is_retry: bool = False
+    request_uuid: Optional[UUID] = None
+    num_retries: int = 0
 
 
 class ThreadLocalStack(threading.local):
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         # each thread will magically get a different stack
         self.stack = [ThreadLocalStackFrame()]
 
 
 SCRAPER_LOCAL = ThreadLocalStack()
 
 
 def retry_on_scraper_error(
     no_parens_function: Optional[Callable] = None,
     *,
-    error_types: Sequence[type] = (),
+    error_types: Sequence[type] = (HublotException, ValueError),
     num_attempts: int = 5,
 ):
     if no_parens_function:
         # decorator is without parentheses
         return retry_on_scraper_error()(no_parens_function)
 
     @contextmanager
@@ -45,31 +47,34 @@
         frame = ThreadLocalStackFrame()
         SCRAPER_LOCAL.stack.append(frame)
         try:
             yield frame
         finally:
             SCRAPER_LOCAL.stack.pop()
 
-    error_types = (ScraperError, *error_types)
+    error_types = tuple(error_types)
 
     def make_wrapper(function: Callable):
         @wraps(function)
         def wrapper(*args, **kwargs):
             with scraper_stack_frame() as frame:
+                frame.request_uuid = uuid4()
                 for attempt in range(num_attempts):
+                    frame.num_retries = attempt
                     try:
-                        if attempt > 0:
-                            frame.is_retry = True
                         payload = function(*args, **kwargs)
                         if isinstance(payload, (Iterator, Generator)) and not isinstance(payload, Sized):
+                            # milk the generator so that all content is parsed
                             payload = list(payload)
                         return payload
                     except Exception as error:  # pylint: disable=broad-except
                         if isinstance(error, error_types) and attempt < num_attempts - 1:
-                            delay = 5 ** attempt
-                            LOGGER.error('%s: %s - sleeping %ds', type(error).__name__, error, delay)
+                            delay = 5**attempt
+                            LOGGER.error("%s: %s - sleeping %ds", type(error).__name__, error, delay)
                             sleep(delay)
                         else:
                             raise
-            raise Exception("can't reach here")
+            raise AssertionError("can't reach here")  # pragma: no cover
+
         return wrapper
+
     return make_wrapper
```

### Comparing `hublot-1.3.0/hublot/logs.py` & `hublot-2.0.0/hublot/logs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 #!/usr/bin/env python3
 
 # standards
 from dataclasses import dataclass
 import logging
-from typing import Optional, Union
+from typing import Iterator, List, Optional, Union
 
-# 3rd parties
-from requests import PreparedRequest
+# hublot
+from .datastructures import CompiledRequest
 
-
-LOGGER = logging.getLogger('hublot')
+LOGGER = logging.getLogger("hublot")
 
 
 @dataclass(frozen=False)
 class LogEntry:
-    preq: PreparedRequest
+    creq: CompiledRequest
     is_redirect: bool = False
     cache_key_str: Optional[str] = None
     cached: Optional[bool] = None
     courtesy_seconds: Optional[float] = None
+    engine_short_code: Optional[str] = None
 
-    def _compose_line(self):
+    def _compose_line(self) -> Iterator[str]:
         if self.cache_key_str:
-            yield f'[{self.cache_key_str}] '
+            yield f"[{self.cache_key_str}] "
         if self.cached:
-            yield '[cached] '
-        elif self.courtesy_seconds and self.courtesy_seconds > 0.5:
-            rounded = f'{round(self.courtesy_seconds)}s'
-            yield f'[{rounded:^6s}] '
+            yield "[cached] "
         else:
-            yield '         '
+            engine_and_sleep = self._compose_engine_and_sleep()
+            if engine_and_sleep:
+                yield f"{engine_and_sleep:8s} "
+            else:
+                yield "         "
         if self.is_redirect:
-            yield '-> '
-        pr = self.preq
-        yield pr.url
-        if pr.method != 'GET':
-            yield f' [{pr.method}'
-            try:
-                length = int(pr.headers.get('Content-Length', 0))
-            except ValueError:
-                length = 0
-            if length > 0:
-                yield f' {length} bytes'
-            yield ']'
+            yield "-> "
+        yield self.creq.url
+        if self.creq.data is not None:
+            yield f" [{self.creq.method} {len(self.creq.data)} bytes]"
+
+    def _compose_engine_and_sleep(self) -> Optional[str]:
+        if self.cached:
+            return "[cached]"
+        parts: List[str] = []
+        if self.engine_short_code:
+            parts.append(self.engine_short_code)
+        if self.courtesy_seconds and self.courtesy_seconds > 0.5:
+            parts.append(f"{round(self.courtesy_seconds)}s")
+        if not parts:
+            return None
+        return "[%s]" % "+".join(parts)
 
-    def __str__(self):
-        return ''.join(self._compose_line())
+    def __str__(self) -> str:
+        return "".join(self._compose_line())
 
 
-def basic_logging_config(level: Union[int, str] = 'INFO', propagate: bool = False):
+def basic_logging_config(level: Union[int, str] = "INFO", propagate: bool = False) -> None:
     """
     Sets up logging for the common use case. Calls `logging.basicConfig`, lowers verbosity for the `urllib3` logger. If `propagate`
     is False (the default), a new handler will be attached to `hublot.LOGGER` that logs in a simple format to stderr, and does not
     propagate log events to the root logger.
     """
     if not isinstance(level, int):
         level = getattr(logging, level)
     logging.basicConfig(level=level)
-    logging.getLogger('urllib3').setLevel(max(logging.WARNING, level))
+    logging.getLogger("urllib3").setLevel(max(logging.WARNING, level))
     if not propagate and not LOGGER.handlers:
         handler = logging.StreamHandler()
-        formatter = logging.Formatter('%(message)s', None, '%')
+        formatter = logging.Formatter("%(message)s", None, "%")
         handler.setFormatter(formatter)
         LOGGER.addHandler(handler)
         LOGGER.propagate = False
```

### Comparing `hublot-1.3.0/hublot.egg-info/SOURCES.txt` & `hublot-2.0.0/hublot.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 MANIFEST.in
 README.md
 setup.py
 hublot/__init__.py
 hublot/client.py
-hublot/courtesy.py
+hublot/compile.py
+hublot/config.py
+hublot/datastructures.py
 hublot/decorator.py
-hublot/exceptions.py
 hublot/logs.py
 hublot/py.typed
-hublot/utils.py
 hublot/version.py
 hublot.egg-info/PKG-INFO
 hublot.egg-info/SOURCES.txt
 hublot.egg-info/dependency_links.txt
 hublot.egg-info/not-zip-safe
 hublot.egg-info/requires.txt
 hublot.egg-info/top_level.txt
 hublot/cache/__init__.py
 hublot/cache/binaryblob.py
 hublot/cache/cache.py
 hublot/cache/key.py
 hublot/cache/storage.py
-test/__init__.py
-test/conftest.py
 test/test_cache.py
 test/test_cache_keys.py
 test/test_cache_max_age.py
 test/test_client.py
 test/test_cookies.py
 test/test_courtesy_sleep.py
+test/test_engine_pool_rotation.py
+test/test_engines.py
 test/test_error_handling.py
+test/test_headers.py
 test/test_logging.py
 test/test_retry_decorator.py
 test/test_threading.py
-test/test_types.py
-test/test_user_agent.py
-test/utils.py
+test/test_user_agent.py
```

### Comparing `hublot-1.3.0/setup.py` & `hublot-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,36 +5,42 @@
 import re
 
 # 3rd parties
 import setuptools
 
 
 def get_version() -> str:
-    version_file = Path(__file__).parent / 'hublot' / 'version.py'
+    version_file = Path(__file__).parent / "hublot" / "version.py"
     version_match = re.search(
-        r"HUBLOT_VERSION = \'(.+)\'",
-        version_file.read_text('UTF-8'),
+        r"HUBLOT_VERSION = \"(.+)\"",
+        version_file.read_text("UTF-8"),
     )
     if not version_match:
-        raise Exception("Couldn't parse version.py")
+        raise ValueError("Couldn't parse version.py")
     return version_match.group(1)
 
 
 setuptools.setup(
-    name='hublot',
+    name="hublot",
     version=get_version(),
-    description='A thin wrapper around Requests that adds caching and throttling',
-    url='https://github.com/saintamh/hublot',
-    author='Hervé Saint-Amand',
-    packages=['hublot', 'hublot.cache'],
-    package_data={'hublot': ['py.typed']},
+    description="A thin wrapper around Requests that adds caching and throttling",
+    url="https://github.com/saintamh/hublot",
+    author="Hervé Saint-Amand",
+    packages=["hublot", "hublot.cache"],
+    package_data={"hublot": ["py.typed"]},
     install_requires=[
+        "chardet>= 3.0.2,<5",  # version req copied from requests
         'dataclasses>=0.8,<1; python_version<"3.7"',
-        'requests>=2.25,<3',
+        "requests>=2.25,<3",
     ],
+    extras_require={
+        "pycurl": [
+            "pycurl>=7,<8",
+        ],
+    },
     classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3',
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
     ],
-    zip_safe=False, # https://mypy.readthedocs.io/en/latest/installed_packages.html#creating-pep-561-compatible-packages
+    zip_safe=False,  # https://mypy.readthedocs.io/en/latest/installed_packages.html#creating-pep-561-compatible-packages
 )
```

### Comparing `hublot-1.3.0/test/test_cache.py` & `hublot-2.0.0/test/test_cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,155 +1,145 @@
 #!/usr/bin/env python3
 
 # standards
-from datetime import timedelta
+from dataclasses import replace
 from pathlib import Path
+from typing import Iterable, Tuple
 
 # 3rd parties
 import pytest
-from requests import Response
 
 # hublot
-from hublot import Client
+from hublot import HttpClient, Response
 from hublot.cache.storage import DiskStorage
 from hublot.logs import LogEntry
-from .utils import assert_responses_equal, dummy_prepared_request, dummy_response
+from .utils import dummy_compiled_request, dummy_response
 
 
-def iter_pairs(client):
-    for url in ('http://one/', 'http://two/'):
-        for method, body in [('GET', None), ('POST', b'dummy body')]:
-            for headers in ({}, {'X-Test': '1'}, {'X-Test': '2'}):
+def iter_pairs(client: HttpClient) -> Iterable[Tuple[dict, Response]]:
+    for url in ("http://one/", "http://two/"):
+        for method, body in [("GET", None), ("POST", b"dummy body")]:
+            for headers in ({}, {"X-Test": "1"}, {"X-Test": "2"}):
                 # NB there's more comprehensive tests for cache key equivalent in `test_cache_keys.py`, but here's a sample
-                request_kwargs = {'url': url, 'method': method, 'headers': headers, 'data': body}
-                preq = dummy_prepared_request(client, **request_kwargs)
-                res = dummy_response(preq)
+                request_kwargs = {"url": url, "method": method, "headers": headers, "data": body}
+                creq = dummy_compiled_request(client, **request_kwargs)
+                res = dummy_response(creq, from_cache=True)
                 yield request_kwargs, res
 
 
-def test_cache(reinstantiable_client):
+def test_cache(reinstantiable_client) -> None:
     client = reinstantiable_client()
-    pairs = [
-        (dummy_prepared_request(client, **req), res)
-        for req, res in iter_pairs(client)
-    ]
-    log_entries = [
-        LogEntry(preq)
-        for preq, _res_unused in pairs
-    ]
+    pairs = [(dummy_compiled_request(client, **req), res) for req, res in iter_pairs(client)]
+    log_entries = [LogEntry(creq) for creq, _res_unused in pairs]
     cache = client.cache
-    for (preq, _res_unused), log in zip(pairs, log_entries):
-        assert cache.get(preq, log) is None  # else test is invalid
+    for (creq, _res_unused), log in zip(pairs, log_entries):
+        assert cache.get(creq, log) is None  # else test is invalid
         assert log.cached is False
-    for (preq, res), log in zip(pairs, log_entries):
-        cache.put(preq, log, res)
+    for (creq, res), log in zip(pairs, log_entries):
+        cache.put(creq, log, res)
     cache = reinstantiable_client().cache
-    for (preq, res), log in zip(pairs, log_entries):
-        assert_responses_equal(cache.get(preq, log), res)
+    for (creq, res), log in zip(pairs, log_entries):
+        assert cache.get(creq, log) == res
         assert log.cached is True
 
 
-def test_client_caching(mocker, reinstantiable_client):
+def test_client_caching(mocker, reinstantiable_client) -> None:
     client = reinstantiable_client()
     for req, res in iter_pairs(client):
-        request = mocker.patch.object(client.session, 'request', return_value=res)
-        assert_responses_equal(client.fetch(**req), res)
+        res = replace(res, from_cache=False)
+        request = mocker.patch.object(client.engine, "request", return_value=res)
+        assert client.fetch(**req) == res
         request.assert_called_once()
     client = reinstantiable_client()
     for req, res in iter_pairs(client):
-        request = mocker.patch.object(client.session, 'request', return_value=res)
-        assert_responses_equal(client.fetch(**req), res)
+        res = replace(res, from_cache=True)
+        request = mocker.patch.object(client.engine, "request", return_value=res)
+        assert client.fetch(**req) == res
         request.assert_not_called()
 
 
-def test_http_errors_are_cached(client, server):
-    one = client.get(f'{server}/fail-with-random-value', raise_for_status=False)
+def test_http_errors_are_cached(client, server) -> None:
+    one = client.get(f"{server}/fail-with-random-value", raise_for_status=False)
     assert one.status_code == 500
-    two = client.get(f'{server}/fail-with-random-value', raise_for_status=False)
+    two = client.get(f"{server}/fail-with-random-value", raise_for_status=False)
     assert two.status_code == 500
-    three = client.get(f'{server}/fail-with-random-value', raise_for_status=False, force_cache_stale=True)
+    three = client.get(f"{server}/fail-with-random-value", raise_for_status=False, force_cache_stale=True)
     assert three.status_code == 500
     assert one.text == two.text
     assert two.text != three.text
 
 
-def test_repeated_http_headers_are_cached(reinstantiable_client, server):
+def test_repeated_http_headers_are_cached(reinstantiable_client, server) -> None:
     client = reinstantiable_client()
-    res = client.get(f'{server}/cookies/set-two-cookies')
-    assert res.headers.get('Set-Cookie') == 'a=1, b=2'
-    assert res.raw._fp.headers.get_all('Set-Cookie') == ['a=1', 'b=2']   # pylint: disable=protected-access
+    res = client.get(f"{server}/cookies/set-two-cookies")
+    assert res.headers.get("Set-Cookie") == "a=1; b=2"
+    assert sorted(f"{c.name}={c.value!r}" for c in client.cookies) == ["a='1'", "b='2'"]
     unique = res.text
 
     client = reinstantiable_client()
-    res = client.get(f'{server}/cookies/set-two-cookies')
-    assert res.text == unique  # check that it was cached
-    assert res.headers.get('Set-Cookie') == 'a=1, b=2'
-    #if callable(getattr(res.headers, 'get_all', None)):
-    assert res.headers.get_all('Set-Cookie') == ['a=1', 'b=2']
+    res = client.get(f"{server}/cookies/set-two-cookies")
+    assert res.text == unique  # it was cached
+    assert res.headers.get("Set-Cookie") == "a=1; b=2"
+    assert res.headers.get_all("Set-Cookie") == ["a=1", "b=2"]
 
-    assert [f'{c.name}={c.value!r}' for c in client.session.cookies] == ["a='1'", "b='2'"]
+    assert sorted(f"{c.name}={c.value!r}" for c in client.cookies) == ["a='1'", "b='2'"]
+    assert [f"{c.name}={c.value!r}" for c in client.cookies] == ["a='1'", "b='2'"]
 
 
-def test_cache_wont_save_body_with_wrong_length(client):
-    preq = dummy_prepared_request(
+def test_cache_wont_save_body_with_wrong_length(client) -> None:
+    creq = dummy_compiled_request(
         client,
-        data=b'More than one byte',
+        data=b"More than one byte",
+        headers={"Content-Length": "1"},
     )
-    preq.headers['Content-Length'] = '1'
-    response = Response()
-    response.request = preq
+    response = dummy_response(creq)
     with pytest.raises(Exception) as ex:
-        client.cache.put(preq, LogEntry(preq), response)
-    assert 'body has 18 bytes but Content-Length is 1' in str(ex)
+        client.cache.put(creq, LogEntry(creq), response)
+    assert "body has 18 bytes but Content-Length is 1" in str(ex)
 
 
-def test_cache_wont_save_get_request_with_content_length(client):
-    preq = dummy_prepared_request(
+def test_cache_wont_save_get_request_with_content_length(client) -> None:
+    creq = dummy_compiled_request(
         client,
-        method='GET',
+        method="GET",
     )
-    preq.headers['Content-Length'] = '999'
-    response = Response()
-    response.request = preq
+    creq.headers["Content-Length"] = "999"
+    response = dummy_response(creq)
     with pytest.raises(Exception) as ex:
-        client.cache.put(preq, LogEntry(preq), response)
-    assert 'body has 0 bytes but Content-Length is 999' in str(ex)
+        client.cache.put(creq, LogEntry(creq), response)
+    assert "body has 0 bytes but Content-Length is 999" in str(ex)
 
 
-def test_cache_can_handle_empty_post_request(client, server):
+def test_cache_can_handle_empty_post_request(client, server) -> None:
     for _from_cache_unused in (False, True):
-        res = client.fetch(f'{server}/echo', data={})
+        res = client.fetch(f"{server}/echo", data={})
         obtained = res.json()
-        obtained.pop('headers')
-        assert obtained == {'method': 'POST', 'args': {}, 'files': {}, 'form': {}, 'json': None}
+        obtained.pop("headers")
+        assert obtained == {"method": "POST", "args": {}, "data": ""}
 
 
-def test_cant_pass_cache_kwargs_and_preinstantiated_cache(cache):
-    with pytest.raises(Exception) as ex:
-        Client(cache=cache, max_cache_age=timedelta(10))
-    assert "can't specify a max_age" in str(ex)
-
-
-def test_cache_can_be_specified_as_path():
-    client = Client(cache=Path('/cache'))
+def test_cache_can_be_specified_as_path() -> None:
+    client = HttpClient(cache=Path("/cache"))
+    assert client.cache is not None
     assert isinstance(client.cache.storage, DiskStorage)
-    assert client.cache.storage.root_path == Path('/cache')
+    assert client.cache.storage.root_path == Path("/cache")
 
 
-def test_cache_cannot_be_specified_as_str():
+def test_cache_cannot_be_specified_as_str() -> None:
     # The idea of not accepting strings is mostly to just keep the client code readable, and maybe preserve forward flexibility.
     # But if this ever a problem, we could consider auto-converting str objects to Path objects.
-    with pytest.raises(ValueError):
-        Client(cache='/cache')
+    with pytest.raises(TypeError):
+        HttpClient(cache="/cache")
 
 
-def test_from_cache_attribute(client, server):
+def test_from_cache_attribute(client, server) -> None:
     for from_cache in (False, True):
-        res = client.fetch(f'{server}/hello')
+        res = client.fetch(f"{server}/hello")
         assert res.from_cache == from_cache
 
 
-def test_cache_can_handle_empty_http_reason(client, server):
+@pytest.mark.skip("Flask 2 no longer lets us send a response without a reason")
+def test_cache_can_handle_empty_http_reason(client, server) -> None:  # pragma: no cover
     for _from_cache_unused in (False, True):
-        res = client.fetch(f'{server}/no-reason')
-        assert res.reason == ''
-        assert res.text == 'hello'
+        res = client.fetch(f"{server}/no-reason", raise_for_status=False)
+        assert res.reason == ""
+        assert res.text == "hello"
```

### Comparing `hublot-1.3.0/test/test_cache_keys.py` & `hublot-2.0.0/test/test_cache_keys.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,313 +1,305 @@
 #!/usr/bin/env python3
 
 # standards
 from collections import OrderedDict
+from dataclasses import replace
 from itertools import count, product
 
 # 3rd parties
 import pytest
-from requests import Request
 
 # hublot
+from hublot import Request
 from hublot.cache import CacheKey
+from hublot.config import Config
 from hublot.logs import LogEntry
-from .utils import assert_responses_equal, dummy_prepared_request, dummy_response, iter_equal_pairs, iter_nonequal_pairs
+from .utils import dummy_compiled_request, dummy_response, iter_equal_pairs, iter_nonequal_pairs
 
 
 def test_simple_cache_use(client):
-    preq = dummy_prepared_request(client)
-    log = LogEntry(preq)
+    creq = dummy_compiled_request(client)
+    log = LogEntry(creq)
     cache = client.cache
-    assert cache.get(preq, log) is None
+    assert cache.get(creq, log) is None
     assert log.cache_key_str is not None
-    cache.put(preq, log, dummy_response(preq))
-    assert_responses_equal(cache.get(preq, log), dummy_response(preq))
+    cache.put(creq, log, dummy_response(creq))
+    assert cache.get(creq, log) == dummy_response(creq, from_cache=True)
 
 
 EQUIVALENCIES = [
-    # For every attribute of a PreparedRequest, lists groups values such that values within the same group should be cached under
+    # For every attribute of a CompiledRequest, lists groups values such that values within the same group should be cached under
     # the same key, but not across groups
-
     # Obviously requests using different methods should be cached separately
-    [{'method': 'GET'}],
-    [{'method': 'POST'}],
-
+    [{"method": "GET"}],
+    [{"method": "POST"}],
     # URLs are case sensitive
-    [{'url': 'http://cache-test/url'}],
-    [{'url': 'http://cache-test/URL'}],
-    [{'url': 'http://cache-test/URL/'}],
-
+    [{"url": "http://cache-test/url"}],
+    [{"url": "http://cache-test/URL"}],
+    [{"url": "http://cache-test/URL/"}],
     # The ordering of the parameters in the URL string matters. They're not parsed at all, so a final '&' is also a cache breaker
-    [{'url': 'http://cache-test/TEST?a=1&b=2'}],
-    [{'url': 'http://cache-test/TEST?b=2&a=1'}],
-    [{'url': 'http://cache-test/TEST?a=1&b=2&'}],
-
+    [{"url": "http://cache-test/TEST?a=1&b=2"}],
+    [{"url": "http://cache-test/TEST?b=2&a=1"}],
+    [{"url": "http://cache-test/TEST?a=1&b=2&"}],
     # `params` are also part of the URL key
-    [{'url': 'http://cache-test/params', 'params': {}}],
-    [{'url': 'http://cache-test/params', 'params': {'x': 'a'}}],
-
+    [{"url": "http://cache-test/params", "params": {}}],
+    [{"url": "http://cache-test/params", "params": {"x": "a"}}],
     # `params` get appended to the URL, so these are equivalent. Using OrderedDict for pythons before 3.7.
     [
-        {'url': 'http://cache-test/params-test', 'params': OrderedDict([('a', '1'), ('b', '2')])},
-        {'url': 'http://cache-test/params-test?', 'params': OrderedDict([('a', '1'), ('b', '2')])},
-        {'url': 'http://cache-test/params-test?a=1', 'params': OrderedDict([('b', '2')])},
-        {'url': 'http://cache-test/params-test?a=1&b=2', 'params': OrderedDict()},
+        {"url": "http://cache-test/params-test", "params": OrderedDict([("a", "1"), ("b", "2")])},
+        {"url": "http://cache-test/params-test?", "params": OrderedDict([("a", "1"), ("b", "2")])},
+        {"url": "http://cache-test/params-test?a=1", "params": OrderedDict([("b", "2")])},
+        {"url": "http://cache-test/params-test?a=1&b=2", "params": OrderedDict()},
     ],
-
     # The presence, absence, or value of a header are all enough to bust the cache
-    [{'url': 'http://cache-test/header-test', 'headers': {}}],
-    [{'url': 'http://cache-test/header-test', 'headers': {'X-Test': '1'}}],
-    [{'url': 'http://cache-test/header-test', 'headers': {'X-Test': '2'}}],
-
+    [{"url": "http://cache-test/header-test", "headers": {}}],
+    [{"url": "http://cache-test/header-test", "headers": {"X-Test": "1"}}],
+    [{"url": "http://cache-test/header-test", "headers": {"X-Test": "2"}}],
     # The `requests` library will normalise the case of headers before sending them off to the server, and so headers are
     # case-insensitive, and so all of these get the same cache key
     [
-        {'url': 'http://cache-test/header-test-2', 'headers': {'X-Test': '1'}},
-        {'url': 'http://cache-test/header-test-2', 'headers': {'x-test': '1'}},
-        {'url': 'http://cache-test/header-test-2', 'headers': {'X-TEST': '1'}},
+        {"url": "http://cache-test/header-test-2", "headers": {"X-Test": "1"}},
+        {"url": "http://cache-test/header-test-2", "headers": {"x-test": "1"}},
+        {"url": "http://cache-test/header-test-2", "headers": {"X-TEST": "1"}},
     ],
-
     # The order of the headers in the dict doesn't matter of course
     [
-        {'url': 'http://cache-test/header-order-test', 'headers': {'X-Test-A': 'a', 'X-Test-B': 'b'}},
-        {'url': 'http://cache-test/header-order-test', 'headers': {'X-Test-B': 'b', 'X-Test-A': 'a'}},
+        {"url": "http://cache-test/header-order-test", "headers": {"X-Test-A": "a", "X-Test-B": "b"}},
+        {"url": "http://cache-test/header-order-test", "headers": {"X-Test-B": "b", "X-Test-A": "a"}},
     ],
-
     # Setting a cookie via `cookies` is the same as setting it manually in a header
     [
-        {'url': 'http://cache-test/cookie-test', 'cookies': {'a': '1'}, 'headers': {}},
-        {'url': 'http://cache-test/cookie-test', 'cookies': {}, 'headers': {'Cookie': 'a=1'}},
+        {"url": "http://cache-test/cookie-test", "cookies": {"a": "1"}, "headers": {}},
+        {"url": "http://cache-test/cookie-test", "cookies": {}, "headers": {"Cookie": "a=1"}},
     ],
-
     # Setting `data` as a dict is equivalent to setting it manually as bytes
     [
-        {'url': 'http://cache-test/data-test', 'data': {'a': '1'}},
+        {"url": "http://cache-test/data-test", "data": {"a": "1"}},
         {
-            'url': 'http://cache-test/data-test',
-            'data': b'a=1',
-            'headers': {'Content-Type': 'application/x-www-form-urlencoded', 'Content-Length': '3'},
+            "url": "http://cache-test/data-test",
+            "data": b"a=1",
+            "headers": {"Content-Type": "application/x-www-form-urlencoded", "Content-Length": "3"},
         },
     ],
-
     # Setting `json` is equivalent to manually building the request
     [
-        {'url': 'http://cache-test/json-test', 'json': {'a': '1'}},
+        {"url": "http://cache-test/json-test", "json": {"a": "1"}},
         {
-            'url': 'http://cache-test/json-test',
-            'data': b'{"a": "1"}',
-            'headers': {'Content-Type': 'application/json'},
+            "url": "http://cache-test/json-test",
+            "data": b'{"a": "1"}',
+            "headers": {"Content-Type": "application/json"},
         },
     ],
-
     # requests can be specified as `Request` objects
     [
-        {'url': 'http://cache-test/request-objects', 'method': 'GET'},
-        {'url': 'http://cache-test/request-objects', 'method': 'GET', 'params': {}},
-        {'url': Request(url='http://cache-test/request-objects', method='GET')},
-        {'url': Request(url='http://cache-test/request-objects', method='GET', params={})},
+        {"url": "http://cache-test/request-objects", "method": "GET"},
+        {"url": "http://cache-test/request-objects", "method": "GET", "params": {}},
+        {"url": Request(url="http://cache-test/request-objects", method="GET")},
+        {"url": Request(url="http://cache-test/request-objects", method="GET", params={})},
     ],
     [
-        {'url': 'http://cache-test/request-objects', 'method': 'POST', 'data': {}},
-        {'url': Request(url='http://cache-test/request-objects', method='POST', data={})},
+        {"url": "http://cache-test/request-objects", "method": "POST", "data": {}},
+        {"url": Request(url="http://cache-test/request-objects", method="POST", data={})},
     ],
     [
         {
-            'url': 'http://cache-test/request-objects',
-            'method': 'POST',
-            'data': {'a': '1'},
+            "url": "http://cache-test/request-objects",
+            "method": "POST",
+            "data": {"a": "1"},
         },
         {
-            'url': 'http://cache-test/request-objects',
-            'method': 'POST',
-            'data': 'a=1',
-            'headers': {'Content-Type': 'application/x-www-form-urlencoded'},
+            "url": "http://cache-test/request-objects",
+            "method": "POST",
+            "data": "a=1",
+            "headers": {"Content-Type": "application/x-www-form-urlencoded"},
         },
         {
-            'url': Request(
-                url='http://cache-test/request-objects',
-                method='POST',
-                data={'a': '1'},
+            "url": Request(
+                url="http://cache-test/request-objects",
+                method="POST",
+                data={"a": "1"},
             ),
         },
         {
-            'url': Request(
-                url='http://cache-test/request-objects',
-                method='POST',
-                data='a=1',
-                headers={'Content-Type': 'application/x-www-form-urlencoded'},
+            "url": Request(
+                url="http://cache-test/request-objects",
+                method="POST",
+                data="a=1",
+                headers={"Content-Type": "application/x-www-form-urlencoded"},
             ),
         },
     ],
-
 ]
 
 
 @pytest.mark.parametrize(
-    'config_1, config_2',
+    "config_1, config_2",
     iter_nonequal_pairs(EQUIVALENCIES),
 )
 def test_unique_keys(client, config_1, config_2):
-    key = CacheKey.compute(dummy_prepared_request(client, **config_1))
-    other_key = CacheKey.compute(dummy_prepared_request(client, **config_2))
+    key = CacheKey.compute(dummy_compiled_request(client, **config_1), Config())
+    other_key = CacheKey.compute(dummy_compiled_request(client, **config_2), Config())
     assert key != other_key
 
 
 @pytest.mark.parametrize(
-    'config_1, config_2',
+    "config_1, config_2",
     iter_nonequal_pairs(EQUIVALENCIES),
 )
 def test_unique_requests(client, config_1, config_2):
     cache = client.cache
-    preq_1 = dummy_prepared_request(client, **config_1)
-    preq_2 = dummy_prepared_request(client, **config_2)
-    cache.put(preq_1, LogEntry(preq_1), dummy_response(preq_1))
-    assert cache.get(preq_2, LogEntry(preq_2)) is None
+    creq_1 = dummy_compiled_request(client, **config_1)
+    creq_2 = dummy_compiled_request(client, **config_2)
+    cache.put(creq_1, LogEntry(creq_1), dummy_response(creq_1))
+    assert cache.get(creq_2, LogEntry(creq_2)) is None
 
 
 @pytest.mark.parametrize(
-    'config_1, config_2',
+    "config_1, config_2",
     iter_equal_pairs(EQUIVALENCIES),
 )
 def test_equivalent_keys(client, config_1, config_2):
-    key_1 = CacheKey.compute(dummy_prepared_request(client, **config_1))
-    key_2 = CacheKey.compute(dummy_prepared_request(client, **config_2))
-    print(dummy_prepared_request(client, **config_1).__dict__)
-    print(dummy_prepared_request(client, **config_2).__dict__)
+    key_1 = CacheKey.compute(dummy_compiled_request(client, **config_1), Config())
+    key_2 = CacheKey.compute(dummy_compiled_request(client, **config_2), Config())
+    print(dummy_compiled_request(client, **config_1))
+    print(dummy_compiled_request(client, **config_2))
     assert key_1 == key_2, (config_1, config_2)
 
 
 @pytest.mark.parametrize(
-    'config_1, config_2',
+    "config_1, config_2",
     iter_equal_pairs(EQUIVALENCIES),
 )
 def test_equivalent_requests(client, config_1, config_2):
     cache = client.cache
-    preq_1 = dummy_prepared_request(client, **config_1)
-    preq_2 = dummy_prepared_request(client, **config_2)
-    response = dummy_response(preq_1)
-    assert cache.get(preq_2, LogEntry(preq_2)) is None  # else test is invalid
-    cache.put(preq_1, LogEntry(preq_1), response)
-    assert_responses_equal(
-        cache.get(preq_2, LogEntry(preq_2)),
-        response,
-    )
+    creq_1 = dummy_compiled_request(client, **config_1)
+    creq_2 = dummy_compiled_request(client, **config_2)
+    response = dummy_response(creq_1)
+    assert cache.get(creq_2, LogEntry(creq_2)) is None  # else test is invalid
+    cache.put(creq_1, LogEntry(creq_1), response)
+    assert cache.get(creq_2, LogEntry(creq_2)) == replace(response, from_cache=True)
 
 
 def test_cache_updates_log_entry_attributes(client):
     cache = client.cache
-    preq = dummy_prepared_request(client)
-    log = LogEntry(preq)
+    creq = dummy_compiled_request(client)
+    log = LogEntry(creq)
     assert log.cache_key_str is None
     assert log.cached is None
-    cache.get(preq, log)
+    cache.get(creq, log)
     assert log.cache_key_str is not None
     assert log.cached is False
-    cache.put(preq, log, dummy_response(preq))
-    cache.get(preq, log)
+    cache.put(creq, log, dummy_response(creq))
+    cache.get(creq, log)
     assert log.cached is True
 
 
 TEST_KEYS = [
-    ('simple-string', '/simple-string', 'simple-string'),
-    ('space string', '/space%20string', 'space%20string'),
-    ('slash/string', '/slash/string', 'slash/string'),
-    ('/slash/string', '/slash/string', 'slash/string'),
-    ('slash/string/', '/slash/string', 'slash/string'),
-    (('item', '123'), '/item/123', 'item/123'),
-    (('slash', '/'), '/slash/%2F', 'slash/%2F'),
+    ("simple-string", "/simple-string", "simple-string"),
+    ("space string", "/space%20string", "space%20string"),
+    ("slash/string", "/slash/string", "slash/string"),
+    ("/slash/string", "/slash/string", "slash/string"),
+    ("slash/string/", "/slash/string", "slash/string"),
+    (("item", "123"), "/item/123", "item/123"),
+    (("slash", "/"), "/slash/%2F", "slash/%2F"),
 ]
 
 
-@pytest.mark.parametrize(
-    'user_specified, expected_path, expected_unique_str',
-    TEST_KEYS
-)
+@pytest.mark.parametrize("user_specified, expected_path, expected_unique_str", TEST_KEYS)
 def test_cache_key_parsing(user_specified, expected_path, expected_unique_str):
     parsed = CacheKey.parse(user_specified)
-    assert ''.join(f'/{p}' for p in parsed.path_parts) == expected_path
+    assert "".join(f"/{p}" for p in parsed.path_parts) == expected_path
     assert parsed.unique_str == expected_unique_str
 
 
-@pytest.mark.parametrize(
-    'user_specified',
-    [spec[0] for spec in TEST_KEYS]
-)
+@pytest.mark.parametrize("user_specified", [spec[0] for spec in TEST_KEYS])
 def test_cache_key_parsing_from_path_parts(user_specified):
     parsed = CacheKey.parse(user_specified)
     assert CacheKey.from_path_parts(parsed.path_parts) == parsed
 
 
 def test_user_specified_cache_key(client, server):
     counter = count()
-    all_keys = ['one', 'two', 'three']
+    all_keys = ["one", "two", "three"]
     all_values = [
-        client.get(
-            f'{server}/unique-number',
-            cache_key=key,
-            params={'unique': str(next(counter))}
-        ).text
-        for key in all_keys
+        client.get(f"{server}/unique-number", cache_key=key, params={"unique": str(next(counter))}).text for key in all_keys
     ]
     assert len(set(all_values)) == len(all_values)  # they're all different
     for key, expected in zip(all_keys, all_values):
         obtained = client.get(
-            f'{server}/unique-number',
+            f"{server}/unique-number",
             cache_key=key,
             # the param is actually different, but the cache key isn't, so we should get the same value back
-            params={'unique': str(next(counter))}
+            params={"unique": str(next(counter))},
         ).text
         assert obtained == expected
 
 
 def test_user_specified_cache_key_on_redirect(client, server):
     res = client.get(
-        f'{server}/redirect/chain/1',
-        cache_key='fixed',
+        f"{server}/redirect/chain/1",
+        cache_key="fixed",
     )
-    assert res.text == 'Landed'
+    assert res.text == "Landed"
     all_keys_in_cache = sorted(k.unique_str for k in client.cache.storage.iter_all_keys())
-    assert all_keys_in_cache == ['fixed', 'fixed.1', 'fixed.2']
+    assert all_keys_in_cache == ["fixed", "fixed.1", "fixed.2"]
 
 
 @pytest.mark.parametrize(
-    'key_1, key_2, should_match',
+    "key_1, key_2, should_match",
     [
         (key_1, key_2, group_1 is group_2)
         for group_1, group_2 in product(
             # Keys from the same line here should match each other, and keys from different lines shouldn't
             [
-                (CacheKey(parts=('a', 'b')), ('a', 'b'), 'a/b'),
-                (CacheKey(parts=('A', 'B')), ('A', 'B'), 'A/B'),
-                (CacheKey(parts=('b', 'c')), ('b', 'c'), 'b/c'),
+                (CacheKey(parts=("a", "b")), ("a", "b"), "a/b"),
+                (CacheKey(parts=("A", "B")), ("A", "B"), "A/B"),
+                (CacheKey(parts=("b", "c")), ("b", "c"), "b/c"),
             ],
             repeat=2,
         )
         for key_1 in group_1
         for key_2 in group_2
-    ]
+    ],
 )
 def test_different_ways_to_express_cache_keys(client, server, key_1, key_2, should_match):
     counter = count()
     response_1, response_2 = (
-        client.get(
-            f'{server}/unique-number',
-            cache_key=key,
-            params={'unique': str(next(counter))}
-        ).text
-        for key in (key_1, key_2)
+        client.get(f"{server}/unique-number", cache_key=key, params={"unique": str(next(counter))}).text for key in (key_1, key_2)
     )
     if should_match:
         assert response_1 == response_2
     else:
         assert response_1 != response_2
 
 
 def test_cache_key_of_unknown_class(client):
     class MyRandoClass:
         pass
 
     with pytest.raises(TypeError):
         client.fetch(
-            'http://whatever/',
+            "http://whatever/",
             cache_key=MyRandoClass(),
         )
+
+
+def test_headers_ignored_by_cache(client):
+    key1 = CacheKey.compute(
+        dummy_compiled_request(client, headers={"Accept": "pudding", "Reject": "asparagus"}),
+        Config(),
+    )
+    key2 = CacheKey.compute(
+        dummy_compiled_request(client, headers={"Accept": "pudding", "Reject": "broccoli"}),
+        Config(),
+    )
+    assert key1 != key2
+
+    key1 = CacheKey.compute(
+        dummy_compiled_request(client, headers={"Accept": "pudding", "Reject": "asparagus"}),
+        Config(headers_ignored_by_cache=["Reject"]),
+    )
+    key2 = CacheKey.compute(
+        dummy_compiled_request(client, headers={"Accept": "pudding", "Reject": "broccoli"}),
+        Config(headers_ignored_by_cache=["Reject"]),
+    )
+    assert key1 == key2
```

### Comparing `hublot-1.3.0/test/test_cache_max_age.py` & `hublot-2.0.0/test/test_cache_max_age.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,119 +6,123 @@
 import gzip
 from itertools import count, product
 from os import utime
 
 # 3rd parties
 import pytest
 
+# hublot
+from hublot.config import Config
+
 
 def _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server):
     now = datetime.now()
     client = reinstantiable_client()
-    unique = client.get(f'{server}/unique-number').text
-    mocker.patch('hublot.cache.storage.current_datetime', return_value=now + timedelta(days=1))
+    unique = client.get(f"{server}/unique-number").text
+    mocker.patch("hublot.cache.storage.current_datetime", return_value=now + timedelta(days=1))
     return unique
 
 
 def test_cache_max_age_defaults(mocker, reinstantiable_client, server):
     # no max_age specified, cache is still valid a day later
     unique = _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server)
     client = reinstantiable_client()
-    assert unique == client.get(f'{server}/unique-number').text
+    assert unique == client.get(f"{server}/unique-number").text
 
 
 def test_cache_long_max_age(mocker, reinstantiable_client, server):
     # max_age is 2 days, cache is still valid a day later
     unique = _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server)
     client = reinstantiable_client()
-    assert unique == client.get(f'{server}/unique-number', max_cache_age=timedelta(days=2)).text
+    assert unique == client.get(f"{server}/unique-number", max_cache_age=timedelta(days=2)).text
 
 
 def test_cache_short_max_age(mocker, reinstantiable_client, server):
     # max_age is 12 hours, cache is no longer valid a day later, we get a new `unique` number
     unique = _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server)
     client = reinstantiable_client()
-    assert unique != client.get(f'{server}/unique-number', max_cache_age=timedelta(hours=12)).text
+    assert unique != client.get(f"{server}/unique-number", max_cache_age=timedelta(hours=12)).text
 
 
 def test_cache_pruning(mocker, reinstantiable_client, server):
     # client is created with max_age of 12 hours, and a request (of any URL) is run. The cache gets pruned.
     unique = _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server)
-    client = reinstantiable_client(max_age=timedelta(hours=12))
-    client.get(f'{server}/hello')
+    client = reinstantiable_client(config=Config(max_cache_age=timedelta(hours=12)))
+    client.get(f"{server}/hello")
     # now it's no longer cached, we fetch a new `unique` number
     client = reinstantiable_client()
-    assert unique != client.get(f'{server}/unique-number').text
+    assert unique != client.get(f"{server}/unique-number").text
 
 
 def test_override_with_method_kwarg(mocker, reinstantiable_client, server):
     # instantiate cache with a max_age that would accept the cached file, but then call the get() method with a shorter age -- the
     # method kwarg overrides the constructor kwarg, cache is invalidated, a new value is fetched
     unique = _fetch_unique_number_then_move_clock_to_next_day(mocker, reinstantiable_client, server)
-    client = reinstantiable_client(max_age=timedelta(days=10))
-    assert unique != client.get(f'{server}/unique-number', max_cache_age=timedelta(hours=12)).text
+    client = reinstantiable_client(config=Config(max_cache_age=timedelta(days=10)))
+    assert unique != client.get(f"{server}/unique-number", max_cache_age=timedelta(hours=12)).text
 
 
 def test_cant_override_with_longer_age(mocker, reinstantiable_client, server):
     # instantiate cache with a max_age that doesn't accept the cached file. Try overriding it with a longer max_cache_age -- that
     # doesn't work. The constructor-given max_cache_age is an upper bound on what the method kwarg accepts (to stay consistent with
     # the fact that the constructor-given max_cache_age triggers full prunes)
     now = datetime.now()
-    client = reinstantiable_client(max_age=timedelta(hours=12))
-    unique = client.get(f'{server}/unique-number').text
-    mocker.patch('hublot.cache.storage.current_datetime', return_value=now + timedelta(days=1))
+    client = reinstantiable_client(config=Config(max_cache_age=timedelta(hours=12)))
+    unique = client.get(f"{server}/unique-number").text
+    mocker.patch("hublot.cache.storage.current_datetime", return_value=now + timedelta(days=1))
     # re-use the same client to ensure there's no pruning happening, that would render the test invalid
-    assert unique != client.get(f'{server}/unique-number', max_cache_age=timedelta(days=2)).text
+    assert unique != client.get(f"{server}/unique-number", max_cache_age=timedelta(days=2)).text
 
 
 def test_cant_override_with_null_age(mocker, reinstantiable_client, server):
     # instantiate cache with a max_age that doesn't accept the cached file. Try overriding it with max_cache_age=None -- that also
     # doesn't work, we fall back to the constructor-given kwarg
     now = datetime.now()
-    client = reinstantiable_client(max_age=timedelta(hours=12))
-    unique = client.get(f'{server}/unique-number').text
-    mocker.patch('hublot.cache.storage.current_datetime', return_value=now + timedelta(days=1))
+    client = reinstantiable_client(config=Config(max_cache_age=timedelta(hours=12)))
+    unique = client.get(f"{server}/unique-number").text
+    mocker.patch("hublot.cache.storage.current_datetime", return_value=now + timedelta(days=1))
     # again, re-use the same client to ensure there's no pruning
-    assert unique != client.get(f'{server}/unique-number', max_cache_age=None).text
+    assert unique != client.get(f"{server}/unique-number", max_cache_age=None).text
 
 
 @pytest.mark.parametrize(
-    'redirect_step_is_cached',
+    "redirect_step_is_cached",
     product([False, True], repeat=3),
 )
 def test_max_age_applies_when_following_redirects(mocker, reinstantiable_client, server, redirect_step_is_cached):
     now = datetime.now()
-    mocker.patch('hublot.cache.storage.current_datetime', lambda: now)
+    mocker.patch("hublot.cache.storage.current_datetime", lambda: now)
 
     @contextmanager
     def mocked_gzip_open(path, *rest, **kwargs):
         with _real_gzip_open(path, *rest, **kwargs) as f:
             yield f
         utime(path, (now.timestamp(), now.timestamp()))
+
     _real_gzip_open = gzip.open
-    mocker.patch('hublot.cache.storage.gzip.open', mocked_gzip_open)
+    mocker.patch("hublot.cache.storage.gzip.open", mocked_gzip_open)
 
     client = reinstantiable_client(
         cookies_enabled=False,  # disable cookies as they would invalidate the cache
     )
 
     # first, cache every step of the redirect chain
-    client.fetch(f'{server}/redirect/chain/1')
+    client.fetch(f"{server}/redirect/chain/1")
 
     # then on the next day, freshen the cache for the redirect steps that should be read from cache
     now += timedelta(hours=24)
     for step_num, is_cached in zip(count(1), redirect_step_is_cached):
         if is_cached:
             client.fetch(
-                f'{server}/redirect/chain/{step_num}',
+                f"{server}/redirect/chain/{step_num}",
                 allow_redirects=False,
                 force_cache_stale=True,
             )
 
     # now if you re-fetch the whole chain, only the ones that were freshly fetched should be read from cache
     now += timedelta(hours=12)
     res = client.fetch(
-        f'{server}/redirect/chain/1',
+        f"{server}/redirect/chain/1",
         max_cache_age=timedelta(hours=24),
     )
 
     assert [r.from_cache for r in [*res.history, res]] == list(redirect_step_is_cached)
```

### Comparing `hublot-1.3.0/test/test_cookies.py` & `hublot-2.0.0/test/test_cookies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 #!/usr/bin/env python3
 
 # hublot
-from hublot import Client
+from hublot import HttpClient
 
 
 def test_cookies_are_saved(client, server):
-    assert client.get(f'{server}/cookies/get').json() == {}
-    client.get(f'{server}/cookies/set?coo=kie')
-    assert client.get(f'{server}/cookies/get').json() == {'coo': 'kie'}
+    assert client.get(f"{server}/cookies/get").json() == {}
+    client.get(f"{server}/cookies/set?coo=kie")
+    assert client.get(f"{server}/cookies/get").json() == {"coo": "kie"}
 
 
 def test_cookies_are_available_via_client(cache, server):
     for _ in (1, 2):
-        client = Client(cache=cache)  # keep cache, clear cookies
-        client.get(f'{server}/cookies/set?coo=kie')
-        assert dict(client.cookies) == {'coo': 'kie'}
-
-
-def test_cookies_are_available_via_session(cache, server):
-    for _ in (1, 2):
-        client = Client(cache=cache)  # keep cache, clear cookies
-        client.get(f'{server}/cookies/set?coo=kie')
-        assert dict(client.session.cookies) == {'coo': 'kie'}
+        client = HttpClient(cache=cache)  # keep cache, clear cookies
+        client.get(f"{server}/cookies/set?coo=kie")
+        assert dict(client.cookies) == {"coo": "kie"}
 
 
 def test_cookies_are_available_via_response(cache, server):
     for _ in (1, 2):
-        client = Client(cache=cache)  # keep cache, clear cookies
-        response = client.get(f'{server}/cookies/set?coo=kie')
-        assert dict(response.cookies) == {'coo': 'kie'}
+        client = HttpClient(cache=cache)  # keep cache, clear cookies
+        response = client.get(f"{server}/cookies/set?coo=kie")
+        assert dict(response.cookies) == {"coo": "kie"}
 
 
 def test_cookies_are_set_when_running_from_cache(reinstantiable_client, server):
     for _ in (1, 2):
         client = reinstantiable_client()
-        assert client.get(f'{server}/cookies/get').json() == {}
-        client.get(f'{server}/cookies/set?coo=kie')
-        assert client.get(f'{server}/cookies/get').json() == {'coo': 'kie'}
+        assert client.get(f"{server}/cookies/get").json() == {}
+        client.get(f"{server}/cookies/set?coo=kie")
+        assert client.get(f"{server}/cookies/get").json() == {"coo": "kie"}
 
 
 def test_cached_redirects(cache, server):
     for _ in (1, 2):
-        client = Client(cache=cache)
-        client.get(f'{server}/redirect/chain/1')
-        cookies = {c.name: c.value for c in client.session.cookies}
-        assert cookies == {'redirect1': 'yes', 'redirect2': 'yes', 'redirect3': 'yes'}
+        client = HttpClient(cache=cache)
+        client.get(f"{server}/redirect/chain/1")
+        cookies = {c.name: c.value for c in client.cookies}
+        assert cookies == {"redirect1": "yes", "redirect2": "yes", "redirect3": "yes"}
 
 
 def test_cookies_can_be_disabled(cache, server):
     for _ in (1, 2):
-        client = Client(cache=cache, cookies_enabled=False)
-        assert client.get(f'{server}/cookies/get').json() == {}
-        client.get(f'{server}/cookies/set?coo=kie')
-        assert client.get(f'{server}/cookies/get').json() == {}
+        client = HttpClient(cache=cache, cookies_enabled=False)
+        assert client.get(f"{server}/cookies/get").json() == {}
+        client.get(f"{server}/cookies/set?coo=kie")
+        assert client.get(f"{server}/cookies/get").json() == {}
 
 
 def test_multiple_cookies_headers(reinstantiable_client, server):
     for reading_from_cache in (False, True):
         client = reinstantiable_client()
-        response = client.get(f'{server}/cookies/set-two-cookies')
+        response = client.get(f"{server}/cookies/set-two-cookies")
         if not reading_from_cache:
             # Check that the mock server returns cookies in 2 separate headers, else this test isn't testing what it meant to test.
             # Can't run this test on the second iteration, because we don't have `response.raw` when coming from cache.
-            response_cookies = sorted(
-                (key, value)
-                for key, value in response.raw.headers.items()
-                if key == 'Set-Cookie'
-            )
-            assert response_cookies == [('Set-Cookie', 'a=1'), ('Set-Cookie', 'b=2')]
-        assert sorted(response.cookies.items()) == [('a', '1'), ('b', '2')]
-        assert sorted(client.session.cookies.items()) == [('a', '1'), ('b', '2')]
+            response_cookies = sorted((key, value) for key, value in response.headers.items() if key == "Set-Cookie")
+            assert response_cookies == [("Set-Cookie", "a=1"), ("Set-Cookie", "b=2")]
+        assert sorted(response.cookies.items()) == [("a", "1"), ("b", "2")]
+        assert sorted(client.cookies.items()) == [("a", "1"), ("b", "2")]
 
 
 def test_response_that_redirects_to_same_url_with_cookie(client, server):
-    assert client.get(f'{server}/self-redirect').text == 'ok'
+    assert client.get(f"{server}/self-redirect").text == "ok"
 
 
 def test_set_cookie_manually(client, server):
-    client.cookies.set('x', '1')
-    assert client.get(f'{server}/cookies/get').json() == {'x': '1'}
+    client.cookies.set("x", "1")
+    assert client.get(f"{server}/cookies/get").json() == {"x": "1"}
+
+
+def test_cookies_can_be_cleared(client, server):
+    assert client.get(f"{server}/cookies/get").json() == {}
+    client.get(f"{server}/cookies/set?coo=kie")
+    assert client.get(f"{server}/cookies/get").json() == {"coo": "kie"}
+    client.cookies.clear()
+    assert client.get(f"{server}/cookies/get").json() == {}
```

### Comparing `hublot-1.3.0/test/test_courtesy_sleep.py` & `hublot-2.0.0/test/test_courtesy_sleep.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,86 +6,77 @@
 from datetime import timedelta
 from itertools import combinations
 
 # 3rd parties
 import pytest
 
 # hublot
-from hublot import Client
-from .utils import dummy_prepared_request, dummy_response
+from hublot import HttpClient
+from .utils import dummy_compiled_request, dummy_response
 
 
 @pytest.mark.parametrize(
-    'courtesy_sleep',
+    "courtesy_sleep",
     [None, timedelta(seconds=0), timedelta(seconds=5), timedelta(seconds=37)],
 )
 def test_courtesy_sleep(mocked_courtesy_sleep, server, courtesy_sleep):
-    kwargs = {} if courtesy_sleep is None else {'courtesy_sleep': courtesy_sleep}
-    client = Client(**kwargs)
-    client.fetch(f'{server}/hello')
+    kwargs = {} if courtesy_sleep is None else {"courtesy_sleep": courtesy_sleep}
+    client = HttpClient(**kwargs)
+    client.fetch(f"{server}/hello")
     mocked_courtesy_sleep.assert_not_called()  # 1st request, no sleep
-    client.fetch(f'{server}/hello')
+    client.fetch(f"{server}/hello")
     expected_sleep = 5 if courtesy_sleep is None else courtesy_sleep.total_seconds()
     if expected_sleep == 0:
         mocked_courtesy_sleep.assert_not_called()
     else:
         mocked_courtesy_sleep.assert_called_once()
-        delay, = mocked_courtesy_sleep.call_args[0]
+        (delay,) = mocked_courtesy_sleep.call_args[0]
         assert delay == pytest.approx(expected_sleep, 0.1)
 
 
 def test_method_kwarg_overrides_default(mocked_courtesy_sleep, server):
-    client = Client()
-    client.fetch(f'{server}/hello')
+    client = HttpClient()
+    client.fetch(f"{server}/hello")
     mocked_courtesy_sleep.assert_not_called()  # 1st request, no sleep
-    client.fetch(f'{server}/hello', courtesy_sleep=timedelta(minutes=1))
+    client.fetch(f"{server}/hello", courtesy_sleep=timedelta(minutes=1))
     mocked_courtesy_sleep.assert_called_once()
     assert mocked_courtesy_sleep.call_args[0][0] == pytest.approx(60, 0.1)
 
 
 def test_method_kwarg_zero_disables_courtesy_sleep(mocked_courtesy_sleep, server):
-    client = Client()
-    client.fetch(f'{server}/hello')
+    client = HttpClient()
+    client.fetch(f"{server}/hello")
     mocked_courtesy_sleep.assert_not_called()  # 1st request, no sleep
-    client.fetch(f'{server}/hello', courtesy_sleep=timedelta(0))
+    client.fetch(f"{server}/hello", courtesy_sleep=timedelta(0))
     mocked_courtesy_sleep.assert_not_called()
 
 
-def test_method_kwarg_zero_none_does_nothing(mocked_courtesy_sleep, server):
-    client = Client()
-    client.fetch(f'{server}/hello')
-    mocked_courtesy_sleep.assert_not_called()  # 1st request, no sleep
-    client.fetch(f'{server}/hello', courtesy_sleep=None)
-    mocked_courtesy_sleep.assert_called_once()
-    assert mocked_courtesy_sleep.call_args[0][0] == pytest.approx(5, 0.1)  # slept default 5 seconds
-
-
 def test_nonequal_hostnames(mocker, mocked_courtesy_sleep):
-    client = Client()
-    mocker.patch.object(client.session, 'request', return_value=dummy_response(dummy_prepared_request(client)))
-    client.fetch('http://one/')
+    client = HttpClient()
+    mocker.patch.object(client.engine, "request", return_value=dummy_response(dummy_compiled_request(client)))
+    client.fetch("http://one/")
     mocked_courtesy_sleep.assert_not_called()
-    client.fetch('http://two/')
+    client.fetch("http://two/")
     mocked_courtesy_sleep.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    'url_1, url_2',
+    "url_1, url_2",
     combinations(
         [
             # All of these are the same host, and so we should sleep between fetches of any pair of URLs in here
-            'http://test/',
-            'http://TEST/',
-            'https://test/',
-            'https://TEST/',
-            'http://test:8080',
+            "http://test/",
+            "http://TEST/",
+            "https://test/",
+            "https://TEST/",
+            "http://test:8080",
         ],
         2,
-    )
+    ),
 )
 def test_equal_hostnames(mocker, mocked_courtesy_sleep, url_1, url_2):
-    client = Client()
-    mocker.patch.object(client.session, 'request', return_value=dummy_response(dummy_prepared_request(client)))
+    client = HttpClient()
+    mocker.patch.object(client.engine, "request", return_value=dummy_response(dummy_compiled_request(client)))
     client.fetch(url_1)
     mocked_courtesy_sleep.assert_not_called()  # 1st request, no sleep
     client.fetch(url_2)
     mocked_courtesy_sleep.assert_called_once()
```

### Comparing `hublot-1.3.0/test/test_logging.py` & `hublot-2.0.0/test/test_logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,49 +4,54 @@
 import re
 
 # hublot
 from hublot import retry_on_scraper_error
 
 
 def test_basic_logging(client, server, captured_logs):
-    client.get(f'{server}/hello')
-    assert re.search(fr'^\[\w\w\w/\w{{13}}\]          {server}/hello\n$', captured_logs())
-    client.get(f'{server}/hello')
-    assert re.search(fr'^\[\w\w\w/\w{{13}}\] \[cached\] {server}/hello\n$', captured_logs())
+    engine = client.engine.short_code()
+    client.get(f"{server}/hello")
+    assert re.search(rf"^\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/hello\n$", captured_logs())
+    client.get(f"{server}/hello")
+    assert re.search(rf"^\[\w\w\w/\w{{13}}\] \[cached\] {server}/hello\n$", captured_logs())
 
 
 def test_logging_courtesy_sleep(client, server, captured_logs):
-    client.get(f'{server}/echo?x=1')
-    assert re.search(fr'^\[\w\w\w/\w{{13}}\]          {server}/echo\?x=1\n$', captured_logs())
-    client.get(f'{server}/echo?x=2')
-    assert re.search(fr'^\[\w\w\w/\w{{13}}\] \[  5s  \] {server}/echo\?x=2\n$', captured_logs())
+    engine = client.engine.short_code()
+    client.get(f"{server}/echo?x=1")
+    assert re.search(rf"^\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/echo\?x=1\n$", captured_logs())
+    client.get(f"{server}/echo?x=2")
+    assert re.search(rf"^\[\w\w\w/\w{{13}}\] \[{engine}\+5s\]  {server}/echo\?x=2\n$", captured_logs())
 
 
 def test_logging_redirects(client, server, captured_logs):
-    client.get(f'{server}/redirect/chain/1')
+    engine = client.engine.short_code()
+    client.get(f"{server}/redirect/chain/1")
     assert re.search(
-        r'^'
-        fr'\[\w\w\w/\w{{13}}\]          {server}/redirect/chain/1\n'
-        fr'\[\w\w\w/\w{{13}}\]          -> {server}/redirect/chain/2\n'
-        fr'\[\w\w\w/\w{{13}}\]          -> {server}/redirect/chain/3\n'
-        r'$',
+        r"^"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/redirect/chain/1\n"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     -> {server}/redirect/chain/2\n"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     -> {server}/redirect/chain/3\n"
+        r"$",
         captured_logs(),
     )
 
 
 def test_logging_on_retry(client, server, unique_key, captured_logs):
+    engine = client.engine.short_code()
+
     @retry_on_scraper_error
     def scrape():
-        client.get(f'{server}/fail-twice-then-succeed/{unique_key}')
-        return 'ok'
+        client.get(f"{server}/fail-twice-then-succeed/{unique_key}")
+        return "ok"
 
     scrape()
     assert re.search(
-        r'^'
-        fr'\[\w\w\w/\w{{13}}\]          {server}/fail-twice-then-succeed/{unique_key}\n'
-        'HTTPError: 500 .+ sleeping 1s\n'
-        fr'\[\w\w\w/\w{{13}}\]          {server}/fail-twice-then-succeed/{unique_key}\n'
-        'HTTPError: 500 .+ sleeping 5s\n'
-        fr'\[\w\w\w/\w{{13}}\]          {server}/fail-twice-then-succeed/{unique_key}\n'
-        r'$',
+        r"^"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/fail-twice-then-succeed/{unique_key}\n"
+        "HttpError: 500 .+ sleeping 1s\n"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/fail-twice-then-succeed/{unique_key}\n"
+        "HttpError: 500 .+ sleeping 5s\n"
+        rf"\[\w\w\w/\w{{13}}\] \[{engine}\]     {server}/fail-twice-then-succeed/{unique_key}\n"
+        r"$",
         captured_logs(),
     )
```

### Comparing `hublot-1.3.0/test/test_retry_decorator.py` & `hublot-2.0.0/test/test_retry_decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,223 +1,243 @@
 #!/usr/bin/env python3
 
 # standards
 from itertools import count
-import json
 from random import choices
 from string import ascii_letters
 
 # 3rd parties
 import pytest
-import requests
 
 # hublot
-from hublot import ScraperError, retry_on_scraper_error
+from hublot import HublotException, retry_on_scraper_error
 
 
 def test_retry_decorator_no_exception(client, server):
     @retry_on_scraper_error
     def fetch():
-        return client.get(f'{server}/hello').text
-    assert fetch() == 'hello'
+        return client.get(f"{server}/hello").text
+
+    assert fetch() == "hello"
 
 
 def test_retry_decorator_on_http_error(client, server, unique_key):
     @retry_on_scraper_error
     def fetch():
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    assert fetch() == 'success after 2 failures'
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
+    assert fetch() == "success after 2 failures"
 
 
 def test_retry_decorator_on_value_error():
     counter = count()
+
     @retry_on_scraper_error
     def fetch():
         i = next(counter)
         if i < 3:
-            raise ValueError('x')
-        return f'Success on attempt {i}'
-    assert fetch() == 'Success on attempt 3'
+            raise ValueError("x")
+        return f"Success on attempt {i}"
+
+    assert fetch() == "Success on attempt 3"
 
 
 def test_retry_decorator_num_attempts_just_enough(client, server, unique_key):
     @retry_on_scraper_error(num_attempts=3)
     def fetch():
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    assert fetch() == 'success after 2 failures'
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
+    assert fetch() == "success after 2 failures"
 
 
 def test_retry_decorator_num_attempts_just_not_enough(client, server, unique_key):
     @retry_on_scraper_error(num_attempts=2)
     def fetch():
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    with pytest.raises(ScraperError):
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
+    with pytest.raises(HublotException):
         fetch()
 
 
 def test_retry_decorator_doesnt_catch_other_exceptions():
     @retry_on_scraper_error
     def fetch():
-        raise KeyError('x')
+        raise KeyError("x")
+
     with pytest.raises(KeyError):
         fetch()
 
 
 def test_retry_decorator_error_types():
     counter = count()
+
     @retry_on_scraper_error(error_types=[KeyError])
     def fetch():
         i = next(counter)
         if i < 3:
-            raise KeyError('x')
-        return f'Success on attempt {i}'
-    assert fetch() == 'Success on attempt 3'
+            raise KeyError("x")
+        return f"Success on attempt {i}"
+
+    assert fetch() == "Success on attempt 3"
 
 
 def test_if_scraper_returns_generator_it_gets_consumed():
     @retry_on_scraper_error
     def fetch():
         yield 1
         yield 2
         yield 3
+
     assert fetch() == [1, 2, 3]
 
 
 def test_if_scraper_returns_iterator_it_gets_consumed():
     @retry_on_scraper_error
     def fetch():
         return (i for i in range(1, 4))
+
     assert fetch() == [1, 2, 3]
 
 
 def test_if_scraper_returns_map_it_gets_consumed():
     @retry_on_scraper_error
     def fetch():
         return map(lambda x: x, range(1, 4))
+
     assert fetch() == [1, 2, 3]
 
 
 def test_if_scraper_returns_filter_it_gets_consumed():
     @retry_on_scraper_error
     def fetch():
         return filter(lambda x: x, range(1, 4))
+
     assert fetch() == [1, 2, 3]
 
 
 def test_if_scraper_returns_dict_keys_it_doesnt_get_consumed():
     @retry_on_scraper_error
     def fetch():
         return {1: 1, 2: 2, 3: 3}.keys()
+
     assert isinstance(fetch(), type({}.keys()))  # you're confused, pylint: disable=isinstance-second-argument-not-valid-type
 
 
-def test_if_scraper_returns_requests_response_it_doesnt_get_turned_into_a_list():
-    # requests.Response is an example of an object that is iterable, but doesn't have a __len__
+def test_if_scraper_returns_custom_iterable_without_len_it_doesnt_get_turned_into_a_list():
+    class MyIterable:
+        def __iter__(self):  # pragma: no cover
+            assert False, "this shouldn't get called"
+            yield from (1, 2, 3)
+
     @retry_on_scraper_error
     def fetch():
-        return requests.Response()
-    assert isinstance(fetch(), requests.Response)
+        return MyIterable()
+
+    assert isinstance(fetch(), MyIterable)
 
 
 def test_scraper_sleeps_increasingly_long_delays(mocked_sleep_on_retry):
     """
     The first sleep must be >= 0 seconds, and then they must all be > than the previous
     """
     counter = count()
+
     @retry_on_scraper_error
     def fetch():
         i = next(counter)
         if i < 4:
-            raise ValueError('x')
-        return f'Success on attempt {i}'
-    assert fetch() == 'Success on attempt 4'
+            raise ValueError("x")
+        return f"Success on attempt {i}"
+
+    assert fetch() == "Success on attempt 4"
     assert mocked_sleep_on_retry.call_count == 4
     previous_sleep = -1
     for attempt in range(4):
         called_args = mocked_sleep_on_retry.call_args_list[attempt][0]
         assert len(called_args) == 1, called_args
-        sleep, = called_args
+        (sleep,) = called_args
         assert sleep > previous_sleep
         previous_sleep = sleep
 
 
 def test_no_courtesy_sleep_on_retries(mocked_courtesy_sleep, client, server, unique_key):
-    client.get(f'{server}/hello')
+    client.get(f"{server}/hello")
+
     @retry_on_scraper_error
     def fetch():
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
     fetch()
     sleeps = [call[0][0] for call in mocked_courtesy_sleep.call_args_list]
     # we should've slept on the 1st call b/c we'd just called the server, then no sleep on subsequent calls
     assert sleeps == [pytest.approx(5, 0.1)]
 
 
 def test_decorated_function_fetches_twice(client, server):
-    key_1 = ''.join(choices(ascii_letters, k=32))
-    key_2 = ''.join(choices(ascii_letters, k=32))
+    key_1 = "".join(choices(ascii_letters, k=32))
+    key_2 = "".join(choices(ascii_letters, k=32))
 
     @retry_on_scraper_error
     def fetch():
         return [
-            client.get(f'{server}/fail-twice-then-succeed/{key_1}').text,
-            client.get(f'{server}/fail-twice-then-succeed/{key_2}').text,
+            client.get(f"{server}/fail-twice-then-succeed/{key_1}").text,
+            client.get(f"{server}/fail-twice-then-succeed/{key_2}").text,
         ]
 
     # The call will succeed on the 5th attempt -- the 1st call fails twice (and the 2nd isn't even reached), then the 2nd call
     # fails twice, then they both work. Because force_cache_stale=True on every retry and applies to both calls, the 1st call was
     # not cached, even after it had succeeded -- when the decorator performs a retry, *all* requests within it are uncached. For
     # that reason the 1st endpoint ends up being called 4 times, and the 2nd one 3 times.
-    assert fetch() == ['success after 2 failures and 2 successes', 'success after 2 failures']
+    assert fetch() == ["success after 2 failures and 2 successes", "success after 2 failures"]
 
 
 def test_decorator_on_client_from_outer_scope(reinstantiable_client, server, unique_key):
     client = reinstantiable_client()
+
     @retry_on_scraper_error
     def fetch():
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    assert fetch() == 'success after 2 failures'
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
+    assert fetch() == "success after 2 failures"
 
 
 def test_decorator_on_client_passed_as_argument(reinstantiable_client, server, unique_key):
     @retry_on_scraper_error
     def fetch(c):
-        return c.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    assert fetch(reinstantiable_client()) == 'success after 2 failures'
+        return c.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
+
+    assert fetch(reinstantiable_client()) == "success after 2 failures"
 
 
 def test_decorator_on_client_created_within_function(reinstantiable_client, server, unique_key):
     @retry_on_scraper_error
     def fetch():
         client = reinstantiable_client()
-        return client.get(f'{server}/fail-twice-then-succeed/{unique_key}').text
-    assert fetch() == 'success after 2 failures'
-
+        return client.get(f"{server}/fail-twice-then-succeed/{unique_key}").text
 
-def test_parsing_html_as_json_is_a_scraper_error():
-    with pytest.raises(ScraperError):
-        json.loads('<html>')
+    assert fetch() == "success after 2 failures"
 
 
 def test_nested_scraper_functions(client, server, unique_key):
 
     # What should happen here:
     #
     #  1. the GET call in `inner()` fails, is retried, and so the call to `inner()` returns "success after 2 failures"
     #
     #  2. the GET call in `outer()` fails, and is retried; this does not force the inner call to be retried though -- that one
     #     keeps being served from cache
 
     @retry_on_scraper_error
     def inner():
-        return 'inner: ' + client.get(f'{server}/fail-twice-then-succeed/{unique_key}-inner').text
+        return "inner: " + client.get(f"{server}/fail-twice-then-succeed/{unique_key}-inner").text
 
     @retry_on_scraper_error
     def outer():
         return [
             inner(),
-            'outer: ' + client.get(f'{server}/fail-twice-then-succeed/{unique_key}-outer').text,
+            "outer: " + client.get(f"{server}/fail-twice-then-succeed/{unique_key}-outer").text,
         ]
 
     assert outer() == [
-        'inner: success after 2 failures',
-        'outer: success after 2 failures',
+        "inner: success after 2 failures",
+        "outer: success after 2 failures",
     ]
```

