# Comparing `tmp/restcraft-0.0.12.tar.gz` & `tmp/restcraft-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restcraft-0.0.12.tar", last modified: Sat Apr 20 16:51:59 2024, max compression
+gzip compressed data, was "restcraft-0.0.14.tar", last modified: Sun Apr 21 03:21:16 2024, max compression
```

## Comparing `restcraft-0.0.12.tar` & `restcraft-0.0.14.tar`

### file list

```diff
@@ -1,40 +1,45 @@
--rw-r--r--   0        0        0     1070 2024-04-09 16:19:20.648925 restcraft-0.0.12/LICENSE
--rw-r--r--   0        0        0     3265 2024-04-20 16:50:18.496783 restcraft-0.0.12/README.md
--rw-r--r--   0        0        0     2045 2024-04-20 16:51:59.777990 restcraft-0.0.12/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-20 16:51:47.581844 restcraft-0.0.12/src/restcraft/__init__.py
--rw-r--r--   0        0        0     1796 2024-04-15 12:22:50.204723 restcraft-0.0.12/src/restcraft/conf.py
--rw-r--r--   0        0        0      130 2024-04-19 09:13:24.283989 restcraft-0.0.12/src/restcraft/core/__init__.py
--rw-r--r--   0        0        0    15590 2024-04-20 08:03:13.594246 restcraft-0.0.12/src/restcraft/core/application.py
--rw-r--r--   0        0        0     7159 2024-04-19 09:14:52.533539 restcraft-0.0.12/src/restcraft/core/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-19 08:57:08.513231 restcraft-0.0.12/src/restcraft/core/middleware/__init__.py
--rw-r--r--   0        0        0     1500 2024-04-19 09:24:31.930712 restcraft-0.0.12/src/restcraft/core/middleware/manager.py
--rw-r--r--   0        0        0     2904 2024-04-19 08:58:45.730324 restcraft-0.0.12/src/restcraft/core/middleware/middleware.py
--rw-r--r--   0        0        0       40 2024-04-19 10:46:50.142712 restcraft-0.0.12/src/restcraft/core/routing/__init__.py
--rw-r--r--   0        0        0     8773 2024-04-20 13:11:28.376612 restcraft-0.0.12/src/restcraft/core/routing/manager.py
--rw-r--r--   0        0        0    18162 2024-04-20 12:55:55.688620 restcraft-0.0.12/src/restcraft/core/routing/request.py
--rw-r--r--   0        0        0    10890 2024-04-20 13:12:49.065631 restcraft-0.0.12/src/restcraft/core/routing/response.py
--rw-r--r--   0        0        0     1708 2024-04-19 09:21:20.791825 restcraft-0.0.12/src/restcraft/core/routing/route.py
--rw-r--r--   0        0        0     4449 2024-04-19 06:44:04.550843 restcraft-0.0.12/src/restcraft/core/routing/types.py
--rw-r--r--   0        0        0     2145 2024-04-19 10:46:50.142712 restcraft-0.0.12/src/restcraft/core/routing/utils.py
--rw-r--r--   0        0        0     3229 2024-04-20 13:05:35.552136 restcraft-0.0.12/src/restcraft/core/routing/view.py
--rw-r--r--   0        0        0        0 2024-04-08 20:34:43.104122 restcraft-0.0.12/src/restcraft/utils/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-20 08:02:38.109751 restcraft-0.0.12/src/restcraft/utils/context.py
--rw-r--r--   0        0        0      938 2024-04-20 08:03:46.890710 restcraft-0.0.12/src/restcraft/utils/helpers.py
--rw-r--r--   0        0        0     4248 2024-04-20 07:03:54.920134 restcraft-0.0.12/src/restcraft/utils/multidict.py
--rw-r--r--   0        0        0      604 2024-04-20 06:31:16.903695 restcraft-0.0.12/src/restcraft/utils/uploadfile.py
--rw-r--r--   0        0        0      391 2024-04-15 12:23:28.421225 restcraft-0.0.12/src/restcraft/wsgi.py
--rw-r--r--   0        0        0       68 2024-04-18 04:26:48.282478 restcraft-0.0.12/tests/__init__.py
--rw-r--r--   0        0        0       83 2024-04-14 17:27:52.271258 restcraft-0.0.12/tests/test_app/__init__.py
--rw-r--r--   0        0        0      314 2024-04-14 17:24:18.663808 restcraft-0.0.12/tests/test_app/exceptions/http_exc.py
--rw-r--r--   0        0        0      853 2024-04-19 09:15:41.878382 restcraft-0.0.12/tests/test_app/middlewares/test_middleware.py
--rw-r--r--   0        0        0      439 2024-04-18 18:10:18.852644 restcraft-0.0.12/tests/test_app/settings.py
--rw-r--r--   0        0        0      386 2024-04-19 09:19:30.890115 restcraft-0.0.12/tests/test_app/views/methods_view.py
--rw-r--r--   0        0        0      827 2024-04-19 09:19:07.205740 restcraft-0.0.12/tests/test_app/views/test_middlewares_view.py
--rw-r--r--   0        0        0      251 2024-04-19 09:15:54.282591 restcraft-0.0.12/tests/test_app/views/test_multipart_view.py
--rw-r--r--   0        0        0     1724 2024-04-20 08:04:08.351009 restcraft-0.0.12/tests/test_app/views/test_view.py
--rw-r--r--   0        0        0       86 2024-04-15 00:31:45.564733 restcraft-0.0.12/tests/test_app/wsgi.py
--rw-r--r--   0        0        0     1764 2024-04-19 09:20:19.586878 restcraft-0.0.12/tests/test_json_response.py
--rw-r--r--   0        0        0     5072 2024-04-20 06:29:21.386369 restcraft-0.0.12/tests/test_request.py
--rw-r--r--   0        0        0     5556 2024-04-19 09:13:25.468010 restcraft-0.0.12/tests/test_router.py
--rw-r--r--   0        0        0     3635 2024-04-17 16:32:54.575981 restcraft-0.0.12/tests/test_wsgi.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 restcraft-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 16:19:20.648925 restcraft-0.0.14/LICENSE
+-rw-r--r--   0        0        0     4710 2024-04-21 03:18:35.140359 restcraft-0.0.14/README.md
+-rw-r--r--   0        0        0     2045 2024-04-21 03:21:16.122592 restcraft-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-21 03:17:37.995565 restcraft-0.0.14/src/restcraft/__init__.py
+-rw-r--r--   0        0        0     1796 2024-04-15 12:22:50.204723 restcraft-0.0.14/src/restcraft/conf.py
+-rw-r--r--   0        0        0      130 2024-04-19 09:13:24.283989 restcraft-0.0.14/src/restcraft/core/__init__.py
+-rw-r--r--   0        0        0    16410 2024-04-21 03:02:32.102658 restcraft-0.0.14/src/restcraft/core/application.py
+-rw-r--r--   0        0        0       53 2024-04-20 22:30:23.937504 restcraft-0.0.14/src/restcraft/core/di/__init__.py
+-rw-r--r--   0        0        0     5368 2024-04-21 02:44:28.358756 restcraft-0.0.14/src/restcraft/core/di/container.py
+-rw-r--r--   0        0        0     7159 2024-04-19 09:14:52.533539 restcraft-0.0.14/src/restcraft/core/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-19 08:57:08.513231 restcraft-0.0.14/src/restcraft/core/middleware/__init__.py
+-rw-r--r--   0        0        0     1638 2024-04-21 03:02:18.458456 restcraft-0.0.14/src/restcraft/core/middleware/manager.py
+-rw-r--r--   0        0        0     2904 2024-04-19 08:58:45.730324 restcraft-0.0.14/src/restcraft/core/middleware/middleware.py
+-rw-r--r--   0        0        0       40 2024-04-19 10:46:50.142712 restcraft-0.0.14/src/restcraft/core/routing/__init__.py
+-rw-r--r--   0        0        0     8909 2024-04-21 02:48:39.994193 restcraft-0.0.14/src/restcraft/core/routing/manager.py
+-rw-r--r--   0        0        0    18162 2024-04-20 12:55:55.688620 restcraft-0.0.14/src/restcraft/core/routing/request.py
+-rw-r--r--   0        0        0    10890 2024-04-20 13:12:49.065631 restcraft-0.0.14/src/restcraft/core/routing/response.py
+-rw-r--r--   0        0        0     1708 2024-04-19 09:21:20.791825 restcraft-0.0.14/src/restcraft/core/routing/route.py
+-rw-r--r--   0        0        0     4449 2024-04-19 06:44:04.550843 restcraft-0.0.14/src/restcraft/core/routing/types.py
+-rw-r--r--   0        0        0     2189 2024-04-21 03:01:29.029718 restcraft-0.0.14/src/restcraft/core/routing/utils.py
+-rw-r--r--   0        0        0     3229 2024-04-20 13:05:35.552136 restcraft-0.0.14/src/restcraft/core/routing/view.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:34:43.104122 restcraft-0.0.14/src/restcraft/utils/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-20 08:02:38.109751 restcraft-0.0.14/src/restcraft/utils/context.py
+-rw-r--r--   0        0        0      938 2024-04-20 08:03:46.890710 restcraft-0.0.14/src/restcraft/utils/helpers.py
+-rw-r--r--   0        0        0     4248 2024-04-20 07:03:54.920134 restcraft-0.0.14/src/restcraft/utils/multidict.py
+-rw-r--r--   0        0        0      604 2024-04-20 06:31:16.903695 restcraft-0.0.14/src/restcraft/utils/uploadfile.py
+-rw-r--r--   0        0        0      391 2024-04-15 12:23:28.421225 restcraft-0.0.14/src/restcraft/wsgi.py
+-rw-r--r--   0        0        0       68 2024-04-18 04:26:48.282478 restcraft-0.0.14/tests/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-14 17:27:52.271258 restcraft-0.0.14/tests/test_app/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-14 17:24:18.663808 restcraft-0.0.14/tests/test_app/exceptions/http_exc.py
+-rw-r--r--   0        0        0      853 2024-04-19 09:15:41.878382 restcraft-0.0.14/tests/test_app/middlewares/test_middleware.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:15:17.454691 restcraft-0.0.14/tests/test_app/services/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-20 22:21:22.026692 restcraft-0.0.14/tests/test_app/services/transient.py
+-rw-r--r--   0        0        0      561 2024-04-20 22:23:27.108295 restcraft-0.0.14/tests/test_app/settings.py
+-rw-r--r--   0        0        0      386 2024-04-19 09:19:30.890115 restcraft-0.0.14/tests/test_app/views/methods_view.py
+-rw-r--r--   0        0        0      827 2024-04-19 09:19:07.205740 restcraft-0.0.14/tests/test_app/views/test_middlewares_view.py
+-rw-r--r--   0        0        0      251 2024-04-19 09:15:54.282591 restcraft-0.0.14/tests/test_app/views/test_multipart_view.py
+-rw-r--r--   0        0        0     2110 2024-04-20 22:30:57.917923 restcraft-0.0.14/tests/test_app/views/test_view.py
+-rw-r--r--   0        0        0       86 2024-04-15 00:31:45.564733 restcraft-0.0.14/tests/test_app/wsgi.py
+-rw-r--r--   0        0        0     2079 2024-04-21 02:42:47.769369 restcraft-0.0.14/tests/test_di.py
+-rw-r--r--   0        0        0     1764 2024-04-19 09:20:19.586878 restcraft-0.0.14/tests/test_json_response.py
+-rw-r--r--   0        0        0     5072 2024-04-20 06:29:21.386369 restcraft-0.0.14/tests/test_request.py
+-rw-r--r--   0        0        0     5556 2024-04-19 09:13:25.468010 restcraft-0.0.14/tests/test_router.py
+-rw-r--r--   0        0        0     3635 2024-04-17 16:32:54.575981 restcraft-0.0.14/tests/test_wsgi.py
+-rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 restcraft-0.0.14/PKG-INFO
```

### Comparing `restcraft-0.0.12/LICENSE` & `restcraft-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/pyproject.toml` & `restcraft-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 keywords = [
     "wsgi",
     "framework",
     "rest",
     "api",
 ]
-version = "0.0.12"
+version = "0.0.14"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/lsfratel/restcraft"
```

### Comparing `restcraft-0.0.12/src/restcraft/conf.py` & `restcraft-0.0.14/src/restcraft/conf.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/application.py` & `restcraft-0.0.14/src/restcraft/core/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 import traceback
 import typing as t
 from types import ModuleType
 
 from ..conf import settings
 from ..core.exceptions import RestCraftException
-from ..core.middleware.manager import middleware_manager
+from ..core.middleware.manager import MiddlewareManager
 from ..core.middleware.middleware import Middleware
-from ..core.routing.manager import route_manager
+from ..core.routing.manager import RouteManager
 from ..core.routing.request import Request
 from ..core.routing.response import JSONResponse, Response
 from ..utils.context import context
+from .di.container import DependencyManager
 from .routing.view import View
 
 
 class RestCraft:
     """
     The RestCraft class is the main entry point for the RestCraft web
     framework. It provides methods for bootstrapping the application, managing
@@ -41,15 +42,15 @@
     The `__call__` and `wsgi` methods handle the WSGI callable interface,
     processing the incoming request and returning the response.
 
     The `process_request` method is the core of the request processing logic,
     executing any registered middleware and the matched view's handler.
     """
 
-    __slots__ = ('route_manager', 'middleware_manager', 'ctx')
+    __slots__ = ('route_manager', 'middleware_manager', 'ctx', 'di')
 
     def __init__(self) -> None:
         """
         The `__init__` method initializes the RestCraft application by setting
         up the internal data structures for managing routes, middleware, and
         configuration.
 
@@ -60,28 +61,34 @@
         registered routes for the application.
 
         The `self._middlewares` attribute is a list of `Middleware` objects,
         representing the registered middleware for the application.
         """
         self.ctx = context
 
-        self.route_manager = route_manager
+        self.di = DependencyManager.instance()
 
-        self.middleware_manager = middleware_manager
+        self.route_manager = RouteManager.instance()
+
+        self.middleware_manager = MiddlewareManager.instance()
 
     def bootstrap(self) -> None:
         """
         Bootstraps the application by importing views, and middleware.
         """
         for view in settings.VIEWS:
             self._import_view(view)
 
         for middleware in settings.MIDDLEWARES:
             self._import_middleware(middleware)
 
+        for scope, dependencies in settings.SERVICES.items():
+            for dependency in dependencies:
+                self._import_di_dependencies(scope, dependency)
+
     def _add_view(self, view: View) -> None:
         """
         Adds a view to the application's routing table.
 
         Args:
             view (View): The view to be added.
 
@@ -90,15 +97,15 @@
         supports. If a list of routes for a particular HTTP method does not
         yet exist, it is created.
         """
         for method in view.methods:
             method = method.upper()
             self.route_manager.add_route(view)
 
-    def _import_module(self, path: str) -> t.Union[ModuleType, t.Any]:
+    def _import_module(self, path: str) -> t.Union[ModuleType, t.Type]:
         """
         Import a module given its filename.
 
         Args:
             filename (str): The filename of the module to import.
 
         Returns:
@@ -148,15 +155,16 @@
 
         result = self._import_module(path)
 
         if inspect.isclass(result):
             if not issubclass(result, View):
                 raise TypeError(f'View {path} must be a subclass of View.')
             self._add_view(result(self))
-        else:
+
+        if inspect.ismodule(result):
             for _, view in self._get_module_members(result):
                 if not issubclass(view, View):
                     continue
                 self._add_view(view(self))
 
     def _import_middleware(self, path: str) -> None:
         """
@@ -171,20 +179,35 @@
 
         if inspect.isclass(result):
             if not issubclass(result, Middleware):
                 raise TypeError(
                     f'Middleware {path} must be a subclass of Middleware.'
                 )
             self.add_middleware(result(self))
-        else:
+
+        if inspect.ismodule(result):
             for _, middleware in self._get_module_members(result):
                 if not issubclass(middleware, Middleware):
                     continue
                 self.add_middleware(middleware(self))
 
+    def _import_di_dependencies(self, scope: str, dependency: str):
+        """
+        Imports and adds a dependency to the application's dependency
+        injection container.
+
+        Args:
+            scope (str): The scope of the dependency.
+            dependency (Any): The dependency to be added.
+        """
+        result = self._import_module(dependency)
+
+        if inspect.isclass(result):
+            self.di.register(result, scope)
+
     def add_middleware(self, middleware: Middleware) -> None:
         """
         Adds a middleware to the application.
 
         Args:
             middleware: The middleware object to be added.
 
@@ -411,7 +434,8 @@
 
             return out.get_response()
         finally:
             """
             Clears the context associated with the current request.
             """
             self.ctx.clear()
+            self.di.clear_scoped()
```

### Comparing `restcraft-0.0.12/src/restcraft/core/exceptions.py` & `restcraft-0.0.14/src/restcraft/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/middleware/manager.py` & `restcraft-0.0.14/src/restcraft/core/middleware/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,22 @@
     responses.
 
     The `MiddlewareManager` provides methods to add middleware components, and
     to invoke the `before_route`, `before_handler`, and `after_handler` methods
     on each middleware component during the request/response lifecycle.
     """
 
+    _instance = None
+
+    @classmethod
+    def instance(cls) -> MiddlewareManager:
+        if cls._instance is None:
+            cls._instance = cls()
+        return cls._instance
+
     def __init__(self) -> None:
         self._middlewares: t.List[Middleware] = []
 
     def add_middleware(self, middleware: Middleware) -> None:
         self._middlewares.append(middleware)
 
     def before_route(self, req: Request) -> t.Optional[Response]:
@@ -37,10 +45,7 @@
             res = middleware.before_handler(req)
             if isinstance(res, Response):
                 return res
 
     def after_handler(self, req: Request, res: Response) -> None:
         for middleware in self._middlewares:
             middleware.after_handler(req, res)
-
-
-middleware_manager = MiddlewareManager()
```

### Comparing `restcraft-0.0.12/src/restcraft/core/middleware/middleware.py` & `restcraft-0.0.14/src/restcraft/core/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/manager.py` & `restcraft-0.0.14/src/restcraft/core/routing/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
 class RouteManager:
     """
     The `RouteManager` class is used to manage the routes in the application.
     It provides methods to add, remove, and get routes from the router.
     """
 
+    _instance = None
+
+    @classmethod
+    def instance(cls):
+        if cls._instance is None:
+            cls._instance = RouteManager()
+        return cls._instance
+
     def __init__(self):
         self._routes: t.Dict[str, t.List[Route]] = {}
 
         self._view_name_mapping: t.Dict[str, str] = {}
 
         self._route_type_mapping: t.Dict[str, t.Type[ParamType]] = {
             'default': StringType,
@@ -245,10 +253,7 @@
 
                 if params is None:
                     continue
 
                 return route, params
 
         raise RouteNotFound('No route matches the given URL.')
-
-
-route_manager = RouteManager()
```

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/request.py` & `restcraft-0.0.14/src/restcraft/core/routing/request.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/response.py` & `restcraft-0.0.14/src/restcraft/core/routing/response.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/route.py` & `restcraft-0.0.14/src/restcraft/core/routing/route.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/types.py` & `restcraft-0.0.14/src/restcraft/core/routing/types.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/utils.py` & `restcraft-0.0.14/src/restcraft/core/routing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from .manager import route_manager
+from .manager import RouteManager
 
 
 def url_for(view_name: str, **kwargs) -> str:
     """
     Generate a URL string for a named route, replacing any dynamic parameters
     in the route pattern with the provided keyword arguments.
 
@@ -15,14 +15,16 @@
 
     Returns:
         str: The generated URL string.
 
     Raises:
         ValueError: If a required parameter is missing or has an invalid value.
     """
+    route_manager = RouteManager.instance()
+
     pattern = route_manager._view_name_mapping[view_name]
     segments = pattern.split('/')
     url_parts = []
 
     for segment in segments:
         dynamic_parts = re.findall(r'(<[^>]+>)', segment)
         for part in dynamic_parts:
```

### Comparing `restcraft-0.0.12/src/restcraft/core/routing/view.py` & `restcraft-0.0.14/src/restcraft/core/routing/view.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/utils/context.py` & `restcraft-0.0.14/src/restcraft/utils/context.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/utils/helpers.py` & `restcraft-0.0.14/src/restcraft/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/utils/multidict.py` & `restcraft-0.0.14/src/restcraft/utils/multidict.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/src/restcraft/utils/uploadfile.py` & `restcraft-0.0.14/src/restcraft/utils/uploadfile.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_app/middlewares/test_middleware.py` & `restcraft-0.0.14/tests/test_app/middlewares/test_middleware.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_app/views/test_middlewares_view.py` & `restcraft-0.0.14/tests/test_app/views/test_middlewares_view.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_app/views/test_view.py` & `restcraft-0.0.14/tests/test_app/views/test_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from restcraft.core import (
     FileResponse,
     HTTPException,
     JSONResponse,
     RedirectResponse,
     View,
 )
+from restcraft.core.di import inject
+
+from tests.test_app.services.transient import MyTransientService
 
 if t.TYPE_CHECKING:
     from restcraft.core import Request
 
 
 class TestHandlerReturnView(View):
     route = '/test-handler-return'
@@ -64,7 +67,20 @@
 
 class TestRouteParamsView(View):
     route = '/test-route-params/<?age:str>'
     methods = ['GET']
 
     def handler(self, req: Request) -> JSONResponse:
         return JSONResponse(body=req.params)
+
+
+class TestDIView(View):
+    route = '/test-di'
+    methods = ['GET']
+
+    @inject
+    def handler(
+        self, req: Request, logger: MyTransientService
+    ) -> JSONResponse:
+        return JSONResponse(
+            body={'message': logger.return_msg('heelo from di')}
+        )
```

### Comparing `restcraft-0.0.12/tests/test_json_response.py` & `restcraft-0.0.14/tests/test_json_response.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_request.py` & `restcraft-0.0.14/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_router.py` & `restcraft-0.0.14/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/tests/test_wsgi.py` & `restcraft-0.0.14/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `restcraft-0.0.12/PKG-INFO` & `restcraft-0.0.14/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: restcraft
-Version: 0.0.12
-Summary: A minimalist Python WSGI framework for building RESTful APIs.
-Keywords: wsgi,framework,rest,api
-Author-Email: Lucas Santana <lsfratel@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Programming Language :: Python :: 3
-Project-URL: Source, https://github.com/lsfratel/restcraft
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # RestCraft WSGI Framework
 
 RestCraft is a lightweight WSGI framework for Python, following the principles of minimalist design. It provides a solid foundation for developing web applications.
 
 ## Framework Structure
 
 RestCraft is divided into two main parts:
@@ -62,18 +39,30 @@
   - **methods:** List of HTTP methods supported by this route (e.g., GET, POST).
 
 ### Routes
 
 - **Dynamic Routing:** RestCraft allows you to specify parts of the URL to be dynamic. These dynamic segments can capture parts of the URL as variables, which can then be passed to your request handlers. For example, defining a route like "/user/<username>" can capture any username and pass it to the handler.
 - **Wildcard Filters:** You can use wildcard filters in the routes to capture data with specific formats. For instance, you can define a route to only accept integers int or str, uuid and slug. This lets you tailor the handler functions to specific data types or patterns, improving flexibility and reducing the need for validating URLs within your handlers.
 
+### Dependency Injection System
+
+Our custom Dependency Injection (DI) system is designed to manage and inject dependencies dynamically, promoting loose coupling and enhanced modularity within the application. The DI system supports various types of dependency lifetimes, ensuring that components can be instantiated and used according to the specific needs of the application. Below are the types of lifetimes supported:
+
+#### Supported Dependency Lifetimes
+
+- **Singleton**: Singleton dependencies are created once and shared throughout the application's lifetime. Once instantiated, the same instance of a singleton dependency is returned every time it is requested. This is useful for services that maintain a consistent state or provide a shared resource across the application.
+
+- **Transient**: Transient dependencies are recreated every time they are requested. This ensures that a new instance is provided to every consumer, guaranteeing that no shared state is carried over from previous uses. Transient dependencies are ideal for stateless services where each operation is expected to be independent.
+
+- **Scoped**: Scoped dependencies are instantiated once per request, a user session, or a specific task. All requests within the same scope share the same instance, while different scopes will have their own separate instances. This is particularly useful for operations where a common context or state needs to be maintained throughout the operation but should not be shared with other operations.
+
 ### Exceptions
 
 - **Easy Custom Exceptions:** Framework supports of custom exceptions, which can be integrated into the application's error handling strategy easily.
 
-### Project Example
+### Project Template
 
-Explore a sample project using RestCraft to see how everything comes together: [Manganato API](https://github.com/lsfratel/manganatoapi)
+[restcraft-template](https://github.com/lsfratel/restcraft-template)
 
 ## In Development
 
 It's important to note that RestCraft is under development. Features and functionality may change as the framework evolves.
```

