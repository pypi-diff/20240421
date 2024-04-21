# Comparing `tmp/openapi_service_client-0.0.8.tar.gz` & `tmp/openapi_service_client-0.0.9.tar.gz`

## Comparing `openapi_service_client-0.0.8.tar` & `openapi_service_client-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/client.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/client_configuration.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/anthropic.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/cohere.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/converter.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/llm_provider.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/openai.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/payload_extractor.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_complex_request_body_mixed.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_anthropic.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_cohere.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_openai.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_cohere_conversion.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_openai_conversion.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/complex_types_openapi_service.json
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/LICENSE
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/README.md
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/anthropic.py
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/cohere.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/converter.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/llm_provider.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/openai.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/providers/payload_extractor.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_complex_request_body_mixed.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_live.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_live_anthropic.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_live_cohere.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_client_live_openai.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_cohere_conversion.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/client/test_openai_conversion.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/complex_types_openapi_service.json
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 openapi_service_client-0.0.9/PKG-INFO
```

### Comparing `openapi_service_client-0.0.8/.github/workflows/tests.yml` & `openapi_service_client-0.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/client.py` & `openapi_service_client-0.0.9/src/openapi_service_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/client_configuration.py` & `openapi_service_client-0.0.9/src/openapi_service_client/client_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     AuthenticationStrategy,
     HTTPAuthentication,
     HttpClientConfig,
     OAuthAuthentication,
     PassThroughAuthentication,
 )
 from openapi_service_client.http_client import AbstractHttpClient, RequestsHttpClient
-from openapi_service_client.providers import LLMProvider, OpenAILLMProvider
-from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor
+from openapi_service_client.providers import FunctionPayloadExtractor, LLMProvider, OpenAILLMProvider
 from openapi_service_client.spec import OpenAPISpecification
 
 
 class ClientConfiguration(Protocol):
 
     def get_http_client(self) -> AbstractHttpClient:
         pass
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.9/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.9/src/openapi_service_client/http_client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Protocol
 
 import requests
 
 from openapi_service_client.config.configuration import HttpClientConfig
 
 VALID_HTTP_METHODS = [
     "get",
@@ -13,16 +12,15 @@
     "options",
     "head",
     "patch",
     "trace",
 ]
 
 
-class AbstractHttpClient(ABC):
-    @abstractmethod
+class AbstractHttpClient(Protocol):
     def send_request(self, request: Dict[str, Any]) -> Any:
         pass
 
 
 class RequestsHttpClient(AbstractHttpClient):
     def __init__(self, config: Optional[HttpClientConfig] = None):
         self.config = config or HttpClientConfig()
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/providers/__init__.py` & `openapi_service_client-0.0.9/src/openapi_service_client/providers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from openapi_service_client.providers.anthropic import AnthropicLLMProvider
 from openapi_service_client.providers.cohere import CohereLLMProvider
 from openapi_service_client.providers.converter import OpenAPISpecificationConverter
 from openapi_service_client.providers.llm_provider import LLMProvider
 from openapi_service_client.providers.openai import OpenAILLMProvider
+from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor
 
 __all__ = [
     "LLMProvider",
     "AnthropicLLMProvider",
     "CohereLLMProvider",
     "OpenAILLMProvider",
     "OpenAPISpecificationConverter",
+    "FunctionPayloadExtractor",
 ]
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/providers/anthropic.py` & `openapi_service_client-0.0.9/src/openapi_service_client/providers/anthropic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 import logging
 
 from openapi_service_client.providers.llm_provider import LLMProvider, OpenAPISpecificationConverter
 from openapi_service_client.providers.openai import OpenAISchemaConverter
-from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor, GenericPayloadExtractor
+from openapi_service_client.providers.payload_extractor import (
+    DefaultRecursivePayloadExtractor,
+    FunctionPayloadExtractor,
+)
 from openapi_service_client.spec import OpenAPISpecification
 
 MIN_REQUIRED_OPENAPI_SPEC_VERSION = 3
 
 logger = logging.getLogger(__name__)
 
 
-class AnthropicSchemaConverter(OpenAISchemaConverter):
-    def __init__(self, schema: OpenAPISpecification):
-        super().__init__(schema=schema, parameters_name="input_schema")
-
-
-class AnthropicPayloadExtractor(GenericPayloadExtractor):
-    """
-    Extracts the function name and arguments from the Anthropic generated function call payload.
-    See https://docs.anthropic.com/claude/docs/tool-use for more information.
-    """
-
-    def __init__(self):
-        super().__init__(arguments_field_name="input")
-
-
 class AnthropicLLMProvider(LLMProvider):
 
     def get_payload_extractor(self) -> FunctionPayloadExtractor:
-        return AnthropicPayloadExtractor()
+        # See https://docs.anthropic.com/claude/docs/tool-use for more information.
+        return DefaultRecursivePayloadExtractor(arguments_field_name="input")
 
     def get_schema_converter(self, openapi_spec: OpenAPISpecification) -> OpenAPISpecificationConverter:
-        return AnthropicSchemaConverter(schema=openapi_spec)
+        # anthropic is using the same conversion format as OpenAI except for the parameters name
+        return OpenAISchemaConverter(schema=openapi_spec, parameters_name="input_schema")
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/providers/cohere.py` & `openapi_service_client-0.0.9/src/openapi_service_client/providers/cohere.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 from typing import Any, Dict, List
 
 import jsonref
 
 from openapi_service_client.providers.converter import OpenAPISpecificationConverter
 from openapi_service_client.providers.llm_provider import LLMProvider
-from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor, GenericPayloadExtractor
+from openapi_service_client.providers.payload_extractor import (
+    DefaultRecursivePayloadExtractor,
+    FunctionPayloadExtractor,
+)
 from openapi_service_client.spec import OpenAPISpecification
 
 logger = logging.getLogger(__name__)
 
 
 class CohereSchemaConverter(OpenAPISpecificationConverter):
 
@@ -101,24 +104,15 @@
             return "object"
         elif schema_type == "array":
             return "list"
         else:
             raise ValueError(f"Unsupported schema type {schema_type}")
 
 
-class CoherePayloadExtractor(GenericPayloadExtractor):
-    """
-    Extracts the function name and arguments from the Cohere generated function call payload.
-    See https://docs.cohere.com/docs/tool-use for more information.
-    """
-
-    def __init__(self):
-        super().__init__(arguments_field_name="parameters")
-
-
 class CohereLLMProvider(LLMProvider):
 
     def get_payload_extractor(self) -> FunctionPayloadExtractor:
-        return CoherePayloadExtractor()
+        # See https://docs.cohere.com/docs/tool-use for more information.
+        return DefaultRecursivePayloadExtractor(arguments_field_name="parameters")
 
     def get_schema_converter(self, openapi_spec: OpenAPISpecification) -> OpenAPISpecificationConverter:
         return CohereSchemaConverter(schema=openapi_spec)
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/providers/openai.py` & `openapi_service_client-0.0.9/src/openapi_service_client/providers/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-import json
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 
 import jsonref
 
 from openapi_service_client.providers.converter import OpenAPISpecificationConverter
 from openapi_service_client.providers.llm_provider import LLMProvider
-from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor
+from openapi_service_client.providers.payload_extractor import (
+    DefaultRecursivePayloadExtractor,
+    FunctionPayloadExtractor,
+)
 from openapi_service_client.spec import OpenAPISpecification
 
 MIN_REQUIRED_OPENAPI_SPEC_VERSION = 3
 
 logger = logging.getLogger(__name__)
 
 
-class OpenAIPayloadExtractor(FunctionPayloadExtractor):
-    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
-        fields_and_values = self.search(payload)
-        if fields_and_values:
-            args = fields_and_values.get("arguments")
-            if not isinstance(args, (str, dict)):
-                raise ValueError(f"Invalid arguments type {type(args)} for OpenAI function call, expected str or dict")
-            return {
-                "name": fields_and_values.get("name"),
-                "arguments": json.loads(args) if isinstance(args, str) else args,
-            }
-        return {}
-
-    def required_fields(self) -> List[str]:
-        return ["name", "arguments"]
-
-
 class OpenAILLMProvider(LLMProvider):
 
     def get_payload_extractor(self) -> FunctionPayloadExtractor:
-        return OpenAIPayloadExtractor()
+        return DefaultRecursivePayloadExtractor(arguments_field_name="arguments")
 
     def get_schema_converter(self, openapi_spec: OpenAPISpecification) -> OpenAPISpecificationConverter:
-        return OpenAISchemaConverter(schema=openapi_spec)
+        # each function in the OpenAI schema needs to be wrapped the below described json object
+        return OpenAISchemaConverter(schema=openapi_spec, transform_fn=lambda fn: {"type": "function", "function": fn})
 
 
 class OpenAISchemaConverter(OpenAPISpecificationConverter):
 
-    def __init__(self, schema: OpenAPISpecification, parameters_name: str = "parameters"):
+    def __init__(
+        self,
+        schema: OpenAPISpecification,
+        parameters_name: str = "parameters",
+        transform_fn: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
+    ):
         self.schema = schema
         self.parameters_name = parameters_name
+        self.transform_fn = transform_fn
 
     def convert(self) -> List[Dict[str, Any]]:
         resolved_schema = jsonref.replace_refs(self.schema.spec_dict)
-        return self._openapi_to_functions(resolved_schema)
+        fn_definitions = self._openapi_to_functions(resolved_schema)
+        return [self.transform_fn(fn) for fn in fn_definitions] if self.transform_fn else fn_definitions
 
     def _openapi_to_functions(self, service_openapi_spec: Dict[str, Any]) -> List[Dict[str, Any]]:
         """
         Extracts functions from the OpenAPI specification of the service and converts them into a format
         suitable for OpenAI function calling.
 
         :param service_openapi_spec: The OpenAPI specification from which functions are to be extracted.
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/providers/payload_extractor.py` & `openapi_service_client-0.0.9/src/openapi_service_client/providers/payload_extractor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import dataclasses
-from abc import ABC, abstractmethod
-from typing import Any, Dict, List
+import json
+from typing import Any, Callable, Dict, List, Optional, Protocol, Union
 
 
-class FunctionPayloadExtractor(ABC):
+class FunctionPayloadExtractor(Protocol):
 
-    @abstractmethod
     def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
         """
         Extracts the function name and arguments from the LLM generated function call payload.
 
         Regardless of the LLM provider the return value should be a dictionary containing the function name
         and arguments under the keys "name" and "arguments" respectively. If payload is not found, an empty
         dictionary should be returned.
@@ -17,65 +16,77 @@
         :param payload: The LLM generated function call payload.
         :returns: A dictionary containing the function name and arguments.
                 - `name`: The name of the function to be called.
                 - `arguments`: The arguments to be passed to the function.
         """
         pass
 
-    @abstractmethod
+
+class DefaultRecursivePayloadExtractor(FunctionPayloadExtractor):
+    """
+    Implements a recursive search for extracting function payloads from complex and nested data structures.
+    DefaultRecursivePayloadExtractor is designed to handle payloads that are dictionaries or lists by recursively
+    searching for and extracting necessary fields as specified in the required_fields method.
+
+    When encountering a non-dictionary or non-list payload, the extractor will attempt to convert the payload to a
+    dictionary using the get_dict_converter method. If the payload is successfully converted, the extractor will
+    continue the recursive search in the converted dictionary. This allows the extractor to handle payloads that are
+    instances of dataclasses or other objects that can be converted to dictionaries (e.g. Pydantic models).
+    """
+
+    def __init__(self, arguments_field_name: str):
+        self.arguments_field_name = arguments_field_name
+
+    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
+        fields_and_values = self.search(payload)
+        if fields_and_values:
+            arguments = fields_and_values.get(self.arguments_field_name)
+            if not isinstance(arguments, (str, dict)):
+                raise ValueError(
+                    f"Invalid {self.arguments_field_name} type {type(arguments)} for function call, expected str/dict"
+                )
+            return {
+                "name": fields_and_values.get("name"),
+                "arguments": json.loads(arguments) if isinstance(arguments, str) else arguments,
+            }
+        return {}
+
     def required_fields(self) -> List[str]:
-        """
-        Returns a list of required fields that must be present in the function call payload.
-        :returns: A list of required fields to find in the function call payload.
-        """
-        pass
+        return ["name", self.arguments_field_name]
 
     def search(self, payload: Any) -> Dict[str, Any]:
-        if self.is_pydantic(payload):
-            payload = payload.dict()
+        if self.is_primitive(payload):
+            return {}
 
+        if dict_converter := self.get_dict_converter(payload):
+            payload = dict_converter()
         elif dataclasses.is_dataclass(payload):
             payload = dataclasses.asdict(payload)
 
         if isinstance(payload, dict):
             if all(field in payload for field in self.required_fields()):
+                # this is the payload we are looking for
                 return payload
             for _, value in payload.items():
-                if isinstance(value, (dict, list)):
-                    result = self.search(value)
-                    if result:
-                        return result
-                elif self.is_pydantic(value):
-                    result = self.search(value.dict())
-                    if result:
-                        return result
+                result = self.search(value)
+                if result:
+                    return result
 
         elif isinstance(payload, list):
             for item in payload:
                 result = self.search(item)
                 if result:
                     return result
 
         return {}
 
-    def is_pydantic(self, payload: Any) -> bool:
-        # pydantic v1 and v2 models have a dict method that can be used to convert the model to a dictionary
-        return hasattr(payload, "dict") and callable(payload.dict)
-
-
-class GenericPayloadExtractor(FunctionPayloadExtractor):
-    def __init__(self, arguments_field_name: str):
-        self.arguments_field_name = arguments_field_name
-
-    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
-        fields_and_values = self.search(payload)
-        if fields_and_values:
-            arguments = fields_and_values.get(self.arguments_field_name)
-            if not isinstance(arguments, dict):
-                raise ValueError(
-                    f"Invalid {self.arguments_field_name} type {type(arguments)} for function call, expected dict"
-                )
-            return {"name": fields_and_values.get("name"), "arguments": arguments}
-        return {}
+    def get_dict_converter(
+        self, obj: Any, method_names: Optional[List[str]] = None
+    ) -> Union[Callable[[], Dict[str, Any]], None]:
+        method_names = method_names or ["model_dump", "dict"]  # search for pydantic v2 then v1
+        for attr in method_names:
+            if hasattr(obj, attr) and callable(getattr(obj, attr)):
+                return getattr(obj, attr)
+        return None
 
-    def required_fields(self) -> List[str]:
-        return ["name", self.arguments_field_name]
+    def is_primitive(self, obj) -> bool:
+        return isinstance(obj, (int, float, str, bool, type(None)))
```

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.9/src/openapi_service_client/request_builder/builder.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.9/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.9/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/conftest.py` & `openapi_service_client-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client.py` & `openapi_service_client-0.0.9/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_auth.py` & `openapi_service_client-0.0.9/tests/client/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.9/tests/client/test_client_complex_request_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def create_order(order: Order):
         total_amount = sum(item.quantity * 10 for item in order.items)
         response = OrderResponse(
             orderId="ORDER-001",
             status="CREATED",
             totalAmount=total_amount,
         )
-        return JSONResponse(content=response.dict(), status_code=201)
+        return JSONResponse(content=response.model_dump(), status_code=201)
 
     return app
 
 
 class TestComplexRequestBody:
 
     @pytest.mark.parametrize("spec_file_path", ["openapi_order_service.yml", "openapi_order_service.json"])
```

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_complex_request_body_mixed.py` & `openapi_service_client-0.0.9/tests/client/test_client_complex_request_body_mixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @app.post("/new_payment")
     def process_payment(payment: PaymentRequest):
         # sanity
         assert payment.transaction_amount == 100.0
         response = PaymentResponse(
             transaction_id="TRANS-12345", status="SUCCESS", message="Payment processed successfully."
         )
-        return JSONResponse(content=response.dict(), status_code=200)
+        return JSONResponse(content=response.model_dump(), status_code=200)
 
     return app
 
 
 # Write the unit test
 class TestPaymentProcess:
```

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_edge_cases.py` & `openapi_service_client-0.0.9/tests/client/test_client_edge_cases.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.9/tests/client/test_client_error_handling.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_live.py` & `openapi_service_client-0.0.9/tests/client/test_client_live.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_client_live_anthropic.py` & `openapi_service_client-0.0.9/tests/client/test_client_live_cohere.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 import os
 
-import anthropic
+import cohere
 import pytest
 
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
-from openapi_service_client.providers import AnthropicLLMProvider
+from openapi_service_client.providers import CohereLLMProvider
 
+# Copied from Cohere's documentation
+preamble = """
+## Task & Context
+You help people answer their questions and other requests interactively. You will be asked a very wide array of
+ requests on all kinds of topics. You will be equipped with a wide range of search engines or similar tools to
+ help you, which you use to research your answer. You should focus on serving the user's needs as best you can,
+ which will be wide-ranging.
+
+## Style Guide
+Unless the user asks for a different style of answer, you should answer in full sentences, using proper grammar and
+ spelling.
+"""
 
-class TestClientLiveAnthropic:
+
+class TestClientLiveCohere:
 
     @pytest.mark.skipif("SERPERDEV_API_KEY" not in os.environ, reason="SERPERDEV_API_KEY not set")
-    @pytest.mark.skipif("ANTHROPIC_API_KEY" not in os.environ, reason="ANTHROPIC_API_KEY not set")
-    def test_serperdev(self):
+    @pytest.mark.skipif("COHERE_API_KEY" not in os.environ, reason="COHERE_API_KEY not set")
+    def test_serperdev(self, test_files_path):
         builder = ClientConfigurationBuilder()
         config = (
-            builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
+            builder.with_openapi_spec(test_files_path / "serper.yaml")
             .with_credentials(os.getenv("SERPERDEV_API_KEY"))
-            .with_provider(AnthropicLLMProvider())
+            .with_provider(CohereLLMProvider())
             .build()
         )
-        client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
-        tool_choice = config.get_tools_definitions()
-        response = client.beta.tools.messages.create(
-            model="claude-3-opus-20240229",
-            max_tokens=1024,
-            tools=[tool_choice[0]],
-            messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
+        client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
+
+        tool_choices = config.get_tools_definitions()
+        response = client.chat(
+            model="command-r",
+            preamble=preamble,
+            tools=tool_choices,
+            message="Do a google search: Who was Nikola Tesla?",
         )
-        tool_payload = response.content[1].to_dict()
         serper_api = OpenAPIServiceClient(config)
-        response = serper_api.invoke(tool_payload)
-        assert "inventions" in str(response)
+        service_response = serper_api.invoke(response)
+        assert "inventions" in str(service_response)
+
+        # make a few more requests to test the same tool
+        service_response = serper_api.invoke(response)
+        assert "Serbian" in str(service_response)
 
-    @pytest.mark.skipif("ANTHROPIC_API_KEY" not in os.environ, reason="ANTHROPIC_API_KEY not set")
+        service_response = serper_api.invoke(response)
+        assert "American" in str(service_response)
+
+    @pytest.mark.skipif("COHERE_API_KEY" not in os.environ, reason="COHERE_API_KEY not set")
     def test_github(self, test_files_path):
         builder = ClientConfigurationBuilder()
         config = (
-            builder.with_openapi_spec(test_files_path / "github_compare.yml")
-            .with_provider(AnthropicLLMProvider())
-            .build()
+            builder.with_openapi_spec(test_files_path / "github_compare.yml").with_provider(CohereLLMProvider()).build()
         )
 
-        client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
-        tool_choice = config.get_tools_definitions()
-        response = client.beta.tools.messages.create(
-            model="claude-3-opus-20240229",
-            max_tokens=1024,
-            tools=[tool_choice[0]],
-            messages=[
-                {
-                    "role": "user",
-                    "content": "Compare branches main and add_default_adapter_filters in repo"
-                    " haystack and owner deepset-ai",
-                }
-            ],
+        client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
+        tool_choices = config.get_tools_definitions()
+        response = client.chat(
+            model="command-r",
+            preamble=preamble,
+            tools=tool_choices,
+            message="Compare branches main and add_default_adapter_filters in repo haystack and owner deepset-ai",
         )
-        tool_payload = response.content[1].to_dict()
         serper_api = OpenAPIServiceClient(config)
-        response = serper_api.invoke(tool_payload)
-        assert "deepset" in str(response)
+        service_response = serper_api.invoke(response)
+        assert "deepset" in str(service_response)
```

### Comparing `openapi_service_client-0.0.8/tests/client/test_cohere_conversion.py` & `openapi_service_client-0.0.9/tests/client/test_cohere_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/client/test_openai_conversion.py` & `openapi_service_client-0.0.9/tests/client/test_openai_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import pytest
 
-from openapi_service_client.providers.anthropic import AnthropicSchemaConverter
 from openapi_service_client.providers.openai import OpenAISchemaConverter
 from openapi_service_client.spec import OpenAPISpecification
 
 
 class TestOpenAPISchemaConversion:
 
     @pytest.mark.parametrize("provider", ["openai", "anthropic"])
     def test_serperdev(self, test_files_path, provider):
         spec = OpenAPISpecification.from_file(test_files_path / "serper.yaml")
         converter = (
-            OpenAISchemaConverter(schema=spec) if provider == "openai" else AnthropicSchemaConverter(schema=spec)
+            OpenAISchemaConverter(schema=spec)
+            if provider == "openai"
+            else OpenAISchemaConverter(schema=spec, parameters_name="input_schema")  # anthropic is using input_schema
         )
         functions = converter.convert()
         assert functions
         assert len(functions) == 1
         function = functions[0]
         assert function["name"] == "serperdev_search"
         assert function["description"] == "Search the web with Google"
@@ -26,15 +27,17 @@
             == {"type": "object", "properties": {"q": {"type": "string"}}, "required": ["q"]}
         )
 
     @pytest.mark.parametrize("provider", ["openai", "anthropic"])
     def test_github(self, test_files_path, provider: str):
         spec = OpenAPISpecification.from_file(test_files_path / "github_compare.yml")
         converter = (
-            OpenAISchemaConverter(schema=spec) if provider == "openai" else AnthropicSchemaConverter(schema=spec)
+            OpenAISchemaConverter(schema=spec)
+            if provider == "openai"
+            else OpenAISchemaConverter(schema=spec, parameters_name="input_schema")  # anthropic is using input_schema
         )
         functions = converter.convert()
         assert functions
         assert len(functions) == 1
         function = functions[0]
         assert function["name"] == "compare_branches"
         assert function["description"] == "Compares two branches against one another."
@@ -60,15 +63,17 @@
             }
         )
 
     @pytest.mark.parametrize("provider", ["openai", "anthropic"])
     def test_complex_types(self, test_files_path, provider: str):
         spec = OpenAPISpecification.from_file(test_files_path / "complex_types_openapi_service.json")
         converter = (
-            OpenAISchemaConverter(schema=spec) if provider == "openai" else AnthropicSchemaConverter(schema=spec)
+            OpenAISchemaConverter(schema=spec)
+            if provider == "openai"
+            else OpenAISchemaConverter(schema=spec, parameters_name="input_schema")  # anthropic is using input_schema
         )
         functions = converter.convert()
         assert functions
         assert len(functions) == 1
         function = functions[0]
         assert function["name"] == "processPayment"
         assert function["description"] == "Process a new payment using the specified payment method"
```

### Comparing `openapi_service_client-0.0.8/tests/test_files/complex_types_openapi_service.json` & `openapi_service_client-0.0.9/tests/test_files/complex_types_openapi_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.9/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/openapi_error_handling.yml` & `openapi_service_client-0.0.9/tests/test_files/openapi_error_handling.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.9/tests/test_files/openapi_greeting_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.9/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.9/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/tests/test_files/serper.yaml` & `openapi_service_client-0.0.9/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/.gitignore` & `openapi_service_client-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/LICENSE` & `openapi_service_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/README.md` & `openapi_service_client-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
 The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function-calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads, and processing responses, it allows users to easily invoke underlying services with LLM-generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere. Each LLM provider uses a unique function-calling schema definition format; OpenAPI Service Client abstracts these differences, enabling a uniform approach to service invocation. Additionally, the library provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
+The library works with several LLM providers, including OpenAI, Anthropic, and Cohere. It uses a common method, `config.get_tools_definitions()`, to manage each provider's unique way of defining function calls. Similarly, differences in how these providers output function calls are handled uniformly through the `LLMProvider` and its `FunctionPayloadExtractor`. Additionally, the library's flexible and extensible design allows users to easily add support for more LLM providers and function-calling formats.
 
 ## Features
 
-- Easy integration with LLM-generated function calls
-- Support for various LLM providers, including OpenAI, Anthropic, and Cohere
-- Automatic handling of REST invocations based on OpenAPI specifications
-- Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
-- Flexible configuration options for adapting the client behavior
-- Extensible architecture for adding support for additional LLM providers and function-calling formats
-
+- **Plug-and-Play LLM Integration**: Easily integrate with LLM-generated function calls for various providers, including OpenAI, Anthropic, and Cohere.
+- **OpenAPI Compliance**: Automatically handle REST service invocations and support various authentication strategies (API key, HTTP authentication, OAuth2).
+- **Customizable and Extensible**: Offers flexible configuration options and an extensible architecture to accommodate additional LLM providers and function-calling formats.
 
 ## Installation
 
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
@@ -51,28 +47,29 @@
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the OpenAI API client and send the chat message
+# Setup the OpenAI API client...
 client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
-tool_choice = config.get_tools_definitions()
+
+# and send the chat message to create a function-calling response completion
 response = client.chat.completions.create(
     model="gpt-3.5-turbo",
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
-    tools=[{"type": "function", "function": tool_choice[0]}],
-    tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
+    tools=config.get_tools_definitions()
 )
 
-# Extract the function-calling payload from response and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 
 ### Anthropic Example
 
 To run the Anthropic Claude Opus example below, you need:
@@ -94,29 +91,30 @@
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(AnthropicLLMProvider())
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the Anthropic API client and send the chat message
+# Setup the Anthropic API client
 client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
 
-# Create a message request using the Anthropic API client
+# and send the chat message to create a function-calling response completion
 response = client.beta.tools.messages.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
     tools=config.get_tools_definitions(),
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
 )
 
-# Extract the function-calling payload from the response and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 ### Cohere Example
 
 To run the Cohere Command-R example below, you need:
 
@@ -137,42 +135,46 @@
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(CohereLLMProvider())
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the Cohere client 
+# Setup the Cohere client...
 client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
 
-# And send the chat message
+# and send the chat message to create a function-calling response completion
 response = client.chat(
     model="command-r",
     preamble="A preamble aka system prompt goes here.",
     tools=config.get_tools_definitions(),
     message="Do a google search: Who was Nikola Tesla?",
 )
 
-# Extract the function-calling payload and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
 The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
 
 By leveraging the OpenAPI specification, `OpenAPIServiceClient` eliminates the need for manual request setup and simplifies the integration process. It allows you to focus on working with LLM-generated function calls and seamlessly invoke the underlying services.
 
+Note how in the examples above, the service invocation function in `OpenAPIServiceClient` directly accepts and processes function-calling payloads from various LLM providers. The client ensures that payloads are correctly identified and extracted, regardless of the LLM source, offering a truly plug-and-play experience.
+
 ## Contributing
 
 Contributions to OpenAPI Service Client are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 OpenAPI Service Client is open-source software licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for more information.
```

### Comparing `openapi_service_client-0.0.8/pyproject.toml` & `openapi_service_client-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.8/PKG-INFO` & `openapi_service_client-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openapi-service-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client library for invoking APIs based on provided OpenAPI specifications
 Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
 Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
 Project-URL: Source, https://github.com/vblagoje/openapi-service-client
 Author-email: Vladimir Blagojevic <dovlex@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -27,25 +27,21 @@
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
 The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function-calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads, and processing responses, it allows users to easily invoke underlying services with LLM-generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere. Each LLM provider uses a unique function-calling schema definition format; OpenAPI Service Client abstracts these differences, enabling a uniform approach to service invocation. Additionally, the library provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
+The library works with several LLM providers, including OpenAI, Anthropic, and Cohere. It uses a common method, `config.get_tools_definitions()`, to manage each provider's unique way of defining function calls. Similarly, differences in how these providers output function calls are handled uniformly through the `LLMProvider` and its `FunctionPayloadExtractor`. Additionally, the library's flexible and extensible design allows users to easily add support for more LLM providers and function-calling formats.
 
 ## Features
 
-- Easy integration with LLM-generated function calls
-- Support for various LLM providers, including OpenAI, Anthropic, and Cohere
-- Automatic handling of REST invocations based on OpenAPI specifications
-- Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
-- Flexible configuration options for adapting the client behavior
-- Extensible architecture for adding support for additional LLM providers and function-calling formats
-
+- **Plug-and-Play LLM Integration**: Easily integrate with LLM-generated function calls for various providers, including OpenAI, Anthropic, and Cohere.
+- **OpenAPI Compliance**: Automatically handle REST service invocations and support various authentication strategies (API key, HTTP authentication, OAuth2).
+- **Customizable and Extensible**: Offers flexible configuration options and an extensible architecture to accommodate additional LLM providers and function-calling formats.
 
 ## Installation
 
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
@@ -73,28 +69,29 @@
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the OpenAI API client and send the chat message
+# Setup the OpenAI API client...
 client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
-tool_choice = config.get_tools_definitions()
+
+# and send the chat message to create a function-calling response completion
 response = client.chat.completions.create(
     model="gpt-3.5-turbo",
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
-    tools=[{"type": "function", "function": tool_choice[0]}],
-    tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
+    tools=config.get_tools_definitions()
 )
 
-# Extract the function-calling payload from response and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 
 ### Anthropic Example
 
 To run the Anthropic Claude Opus example below, you need:
@@ -116,29 +113,30 @@
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(AnthropicLLMProvider())
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the Anthropic API client and send the chat message
+# Setup the Anthropic API client
 client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
 
-# Create a message request using the Anthropic API client
+# and send the chat message to create a function-calling response completion
 response = client.beta.tools.messages.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
     tools=config.get_tools_definitions(),
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
 )
 
-# Extract the function-calling payload from the response and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 ### Cohere Example
 
 To run the Cohere Command-R example below, you need:
 
@@ -159,42 +157,46 @@
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(CohereLLMProvider())
     .build()
 )
 
-# Initialize the OpenAPIServiceClient with configuration
-serper_api = OpenAPIServiceClient(config)
-
-# Setup the Cohere client 
+# Setup the Cohere client...
 client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
 
-# And send the chat message
+# and send the chat message to create a function-calling response completion
 response = client.chat(
     model="command-r",
     preamble="A preamble aka system prompt goes here.",
     tools=config.get_tools_definitions(),
     message="Do a google search: Who was Nikola Tesla?",
 )
 
-# Extract the function-calling payload and invoke the service
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+
+# Simply pass the LLM response and invoke the service
+# The LLM specific function-calling payload is extracted and processed automatically
 service_response = serper_api.invoke(response)
 print(service_response)
 ```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
 The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
 
 By leveraging the OpenAPI specification, `OpenAPIServiceClient` eliminates the need for manual request setup and simplifies the integration process. It allows you to focus on working with LLM-generated function calls and seamlessly invoke the underlying services.
 
+Note how in the examples above, the service invocation function in `OpenAPIServiceClient` directly accepts and processes function-calling payloads from various LLM providers. The client ensures that payloads are correctly identified and extracted, regardless of the LLM source, offering a truly plug-and-play experience.
+
 ## Contributing
 
 Contributions to OpenAPI Service Client are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 OpenAPI Service Client is open-source software licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for more information.
```

