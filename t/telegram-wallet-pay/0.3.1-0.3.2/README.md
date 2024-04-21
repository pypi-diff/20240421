# Comparing `tmp/telegram_wallet_pay-0.3.1.tar.gz` & `tmp/telegram_wallet_pay-0.3.2.tar.gz`

## Comparing `telegram_wallet_pay-0.3.1.tar` & `telegram_wallet_pay-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/examples/01_get_order_preview.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_schemas.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.gitignore
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/README.md
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/codecov.yaml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/examples/00_create_order.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_schemas.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.gitignore
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/README.md
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.3.1/examples/00_create_order.py` & `telegram_wallet_pay-0.3.2/examples/00_create_order.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import hmac
 from base64 import b64encode
+from typing import Union
 
 ENCODING = "utf-8"
 
 
 def from_snake_to_pascal(snake_str: str) -> str:
     """Convert snake_case to PascalCase."""
     return "".join(x.capitalize() for x in snake_str.lower().split("_"))
@@ -19,20 +20,21 @@
 
 
 def compute_signature(
     store_api_key: str,
     http_method: str,
     uri_path: str,
     timestamp: str,
-    body: str,
+    body: Union[str, bytes],
 ) -> str:
     """Compute signature."""
-    body_bytes = bytes(body, ENCODING)
-    body_base64 = b64encode(body_bytes).decode(ENCODING)
+    if isinstance(body, str):
+        body = bytes(body, ENCODING)
 
+    body_base64 = b64encode(body).decode(ENCODING)
     payload = f"{http_method}.{uri_path}.{timestamp}.{body_base64}"
 
     signature_bytes = hmac.new(
         key=bytes(store_api_key, ENCODING),
         msg=bytes(payload, ENCODING),
         digestmod=hashlib.sha256,
     ).digest()
```

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import datetime
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
 from .payment_option import PaymentOption
 
 
 class WebhookPayload(DefaultModel):
     id: int
     number: str
     external_id: str = Field(max_length=255)
-    status: Literal["ACTIVE", "EXPIRED", "PAID", "CANCELLED"]
     custom_data: Optional[str] = Field(None, max_length=255)
     order_amount: MoneyAmount
     selected_payment_option: PaymentOption
     order_completed_datetime: datetime = Field(alias="orderCompletedDateTime")
```

### Comparing `telegram_wallet_pay-0.3.1/tests/test_client.py` & `telegram_wallet_pay-0.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/tests/test_schemas.py` & `telegram_wallet_pay-0.3.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/tests/test_signature.py` & `telegram_wallet_pay-0.3.2/tests/test_signature.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,44 @@
+from typing import Union
+
+import pytest
 from telegram_wallet_pay.tools import compute_signature
 
 
-def test_signature() -> None:
+@pytest.mark.parametrize(
+    "body",
+    [
+        (
+            '[{"eventDateTime":"2023-07-28T10:20:17.681338Z",'
+            '"eventId":10030477545046017,"type":"ORDER_PAID","payload":{'
+            '"id":10030467668508673,"number":"XYTNJP2O","customData":"in exercitation '
+            'culpa","externalId":"JDF23NN","orderAmount":{"amount":"0.100000340",'
+            '"currencyCode":"TON"},"selectedPaymentOption":{"amount":{'
+            '"amount":"0.132653","currencyCode":"USDT"},"amountFee":{'
+            '"amount":"0.001327","currencyCode":"USDT"},"amountNet":{'
+            '"amount":"0.131326","currencyCode":"USDT"},'
+            '"exchangeRate":"1.3265247467314987"},'
+            '"orderCompletedDateTime":"2023-07-28T10:20:17.628946Z"}}]'
+        ),
+        (
+            b'[{"eventDateTime":"2023-07-28T10:20:17.681338Z",'
+            b'"eventId":10030477545046017,"type":"ORDER_PAID","payload":{'
+            b'"id":10030467668508673,"number":"XYTNJP2O","customData":"in exercitation '
+            b'culpa","externalId":"JDF23NN","orderAmount":{"amount":"0.100000340",'
+            b'"currencyCode":"TON"},"selectedPaymentOption":{"amount":{'
+            b'"amount":"0.132653","currencyCode":"USDT"},"amountFee":{'
+            b'"amount":"0.001327","currencyCode":"USDT"},"amountNet":{'
+            b'"amount":"0.131326","currencyCode":"USDT"},'
+            b'"exchangeRate":"1.3265247467314987"},'
+            b'"orderCompletedDateTime":"2023-07-28T10:20:17.628946Z"}}]'
+        ),
+    ],
+)
+def test_signature(body: Union[str, bytes]) -> None:
     """Test signature provided by docs."""
-    body = (
-        '[{"eventDateTime":"2023-07-28T10:20:17.681338Z",'
-        '"eventId":10030477545046017,"type":"ORDER_PAID","payload":{'
-        '"id":10030467668508673,"number":"XYTNJP2O","customData":"in exercitation '
-        'culpa","externalId":"JDF23NN","orderAmount":{"amount":"0.100000340",'
-        '"currencyCode":"TON"},"selectedPaymentOption":{"amount":{'
-        '"amount":"0.132653","currencyCode":"USDT"},"amountFee":{'
-        '"amount":"0.001327","currencyCode":"USDT"},"amountNet":{'
-        '"amount":"0.131326","currencyCode":"USDT"},'
-        '"exchangeRate":"1.3265247467314987"},'
-        '"orderCompletedDateTime":"2023-07-28T10:20:17.628946Z"}}]'
-    )
-
     signature = compute_signature(
         store_api_key="your_secret_api_key_sYIpNypce5sls6Ik",
         http_method="POST",
         uri_path="/webhook/",
         timestamp="168824905680291",
         body=body,
     )
```

### Comparing `telegram_wallet_pay-0.3.1/.gitignore` & `telegram_wallet_pay-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/pyproject.toml` & `telegram_wallet_pay-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.1/PKG-INFO` & `telegram_wallet_pay-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.3.1
+Version: 0.3.2
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
@@ -42,19 +42,20 @@
 Requires-Dist: pytest>=8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Telegram Wallet Pay
 
 Python async client for [Telegram Wallet Pay API](https://pay.wallet.tg) made of `aiohttp` and `pydantic`
 
-[![Python](https://img.shields.io/badge/python-^3.8-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/pypi/pyversions/telegram-wallet-pay.svg)](https://pypi.org/project/telegram-wallet-pay/)
+[![pypi](https://img.shields.io/pypi/v/telegram-wallet-pay?label=pypi%20package)](https://pypi.org/project/telegram-wallet-pay/)
+[![Tests](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml/badge.svg)](https://github.com/Olegt0rr/YaTracker/actions/workflows/tests.yml)
+[![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
 [![Code linter: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![Linters](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/linters.yml/badge.svg)](https://github.com/Olegt0rr/YaTracker/actions/workflows/linters.yml)
-[![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
 ---
 
 ## Get started
 
 ### Read Telegram Wallet Pay API docs
 
 https://docs.wallet.tg/pay/#section/Get-started
```

