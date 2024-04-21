# Comparing `tmp/beepy_web-0.9.8.tar.gz` & `tmp/beepy_web-0.9.9.tar.gz`

## Comparing `beepy_web-0.9.8.tar` & `beepy_web-0.9.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.env.template
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.python-version
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.readthedocs.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.8/requirements.txt
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/__init__.py
--rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/attrs.py
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/children.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/components.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/context.py
--rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/framework.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/listeners.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/router.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/style.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/tags.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/trackable.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/types.py
--rwxr-xr-x   0        0        0     5190 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/__main__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/actions.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/plot.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/table.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/dev.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/internal.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/js_py.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 beepy_web-0.9.8/scripts/dev.sh
--rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.8/scripts/publish.sh
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/package-lock.json
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/webpack.prod.js
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.8/LICENSE
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.8/README.md
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 beepy_web-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.env.template
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.python-version
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.readthedocs.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.9/requirements.txt
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/__init__.py
+-rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/attrs.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/children.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/components.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/context.py
+-rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/listeners.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/router.py
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/style.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/trackable.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/types.py
+-rwxr-xr-x   0        0        0     5190 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/table.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 beepy_web-0.9.9/scripts/dev.sh
+-rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.9/scripts/publish.sh
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/package-lock.json
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/webpack.prod.js
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.9/README.md
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 beepy_web-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.9/PKG-INFO
```

### Comparing `beepy_web-0.9.8/.pre-commit-config.yaml` & `beepy_web-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/__init__.py` & `beepy_web-0.9.9/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/attrs.py` & `beepy_web-0.9.9/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/children.py` & `beepy_web-0.9.9/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/components.py` & `beepy_web-0.9.9/beepy/components.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/context.py` & `beepy_web-0.9.9/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/framework.py` & `beepy_web-0.9.9/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __config__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _py_tag_attribute
 
-__version__ = '0.9.8'  # For internal development set to 0.0a0
+__version__ = '0.9.9'  # For internal development set to 0.0a0
 __config__['version'] = __version__
 
 
 _tag_initialized = False
 
 
 class _MetaTag(_MetaComponent):
```

### Comparing `beepy_web-0.9.8/beepy/listeners.py` & `beepy_web-0.9.9/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/router.py` & `beepy_web-0.9.9/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/style.py` & `beepy_web-0.9.9/beepy/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from collections.abc import Iterable
 from typing import Any, Protocol
 
+from beepy.attrs import attr, state
 from beepy.context import Context
-from beepy.framework import Tag, __config__, attr, state
+from beepy.framework import Tag, __config__
 from beepy.tags import Head
 from beepy.types import AttrValue, safe_html, safe_html_content
 from beepy.utils import js
 from beepy.utils.common import MISSING, get_random_name, log10_ceil, safe_issubclass, to_kebab_case
 
 
 def dict_of_properties_to_css(properties):
```

### Comparing `beepy_web-0.9.8/beepy/tags.py` & `beepy_web-0.9.9/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/trackable.py` & `beepy_web-0.9.9/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/types.py` & `beepy_web-0.9.9/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/dev/__init__.py` & `beepy_web-0.9.9/beepy/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/modules/context_menu.py` & `beepy_web-0.9.9/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/modules/local_storage.py` & `beepy_web-0.9.9/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/modules/modal.py` & `beepy_web-0.9.9/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/modules/table.py` & `beepy_web-0.9.9/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/modules/tabs.py` & `beepy_web-0.9.9/beepy/modules/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/api.py` & `beepy_web-0.9.9/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/asyncio.py` & `beepy_web-0.9.9/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/common.py` & `beepy_web-0.9.9/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/dev.py` & `beepy_web-0.9.9/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/import_hooks.py` & `beepy_web-0.9.9/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/internal.py` & `beepy_web-0.9.9/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/js.py` & `beepy_web-0.9.9/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/beepy/utils/js_py.py` & `beepy_web-0.9.9/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/scripts/publish.sh` & `beepy_web-0.9.9/scripts/publish.sh`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/package-lock.json` & `beepy_web-0.9.9/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.9'}}", "'version'": "'0.9.9'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.8"
+            "version": "0.9.9"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.9.8"
+    "version": "0.9.9"
 }
```

### Comparing `beepy_web-0.9.8/web/package.json` & `beepy_web-0.9.9/web/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.9'"}*

```diff
@@ -31,9 +31,9 @@
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.8"
+    "version": "0.9.9"
 }
```

### Comparing `beepy_web-0.9.8/web/webpack.prod.js` & `beepy_web-0.9.9/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/src/beepy.js` & `beepy_web-0.9.9/web/src/beepy.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.8'
+    __version__ = '0.9.9'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.9.8/web/src/dev-server.js` & `beepy_web-0.9.9/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/src/files.js` & `beepy_web-0.9.9/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/src/main.css` & `beepy_web-0.9.9/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/src/python.js` & `beepy_web-0.9.9/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/web/src/utils.js` & `beepy_web-0.9.9/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/.gitignore` & `beepy_web-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/LICENSE` & `beepy_web-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/README.md` & `beepy_web-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/pyproject.toml` & `beepy_web-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.8/PKG-INFO` & `beepy_web-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.8
+Version: 0.9.9
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://beepy-web-ba63e5a12994.herokuapp.com/e/
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Project-URL: Community, https://t.me/bee_py/
 Project-URL: Sandbox, https://kor0p.github.io/BeePy-examples/sandbox
 Project-URL: NPM, https://www.npmjs.com/package/@kor0p/beepy
```

