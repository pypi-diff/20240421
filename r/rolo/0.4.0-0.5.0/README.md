# Comparing `tmp/rolo-0.4.0.tar.gz` & `tmp/rolo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolo-0.4.0.tar", last modified: Mon Mar 11 23:18:50 2024, max compression
+gzip compressed data, was "rolo-0.5.0.tar", last modified: Sun Apr 21 12:32:17 2024, max compression
```

## Comparing `rolo-0.4.0.tar` & `rolo-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.739421 rolo-0.4.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11358 2024-01-19 14:23:57.000000 rolo-0.4.0/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)    17995 2024-03-11 23:18:50.739421 rolo-0.4.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3822 2024-03-11 23:14:41.000000 rolo-0.4.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1842 2024-03-11 23:18:23.000000 rolo-0.4.0/pyproject.toml
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.735421 rolo-0.4.0/rolo/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      213 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23639 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/asgi.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5265 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/client.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2546 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/dispatcher.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.735421 rolo-0.4.0/rolo/gateway/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      458 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/gateway/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2602 2024-03-11 23:14:35.000000 rolo-0.4.0/rolo/gateway/asgi.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13099 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/gateway/chain.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2099 2024-03-11 23:14:35.000000 rolo-0.4.0/rolo/gateway/gateway.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2738 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/gateway/handlers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1600 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/gateway/wsgi.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7158 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/proxy.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11643 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/request.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4124 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/resource.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3404 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/response.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    22345 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/router.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.735421 rolo-0.4.0/rolo/serving/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      227 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/serving/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    15148 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/serving/twisted.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.735421 rolo-0.4.0/rolo/testing/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:01:37.000000 rolo-0.4.0/rolo/testing/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8756 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/testing/pytest.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.735421 rolo-0.4.0/rolo/websocket/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      392 2024-03-11 23:14:35.000000 rolo-0.4.0/rolo/websocket/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4966 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/websocket/adapter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      685 2024-03-10 19:19:00.000000 rolo-0.4.0/rolo/websocket/errors.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9994 2024-03-11 23:14:41.000000 rolo-0.4.0/rolo/websocket/request.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      474 2024-03-11 23:14:35.000000 rolo-0.4.0/rolo/websocket/websocket.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.739421 rolo-0.4.0/rolo.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    17995 2024-03-11 23:18:50.000000 rolo-0.4.0/rolo.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      811 2024-03-11 23:18:50.000000 rolo-0.4.0/rolo.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-11 23:18:50.000000 rolo-0.4.0/rolo.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      176 2024-03-11 23:18:50.000000 rolo-0.4.0/rolo.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        5 2024-03-11 23:18:50.000000 rolo-0.4.0/rolo.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-03-11 23:18:50.739421 rolo-0.4.0/setup.cfg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:18:50.739421 rolo-0.4.0/tests/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12809 2024-03-10 19:19:00.000000 rolo-0.4.0/tests/test_asgi.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2305 2024-01-12 18:56:59.000000 rolo-0.4.0/tests/test_dispatcher.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10977 2024-01-12 18:56:59.000000 rolo-0.4.0/tests/test_proxy.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6293 2024-01-12 18:56:59.000000 rolo-0.4.0/tests/test_request.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4679 2024-01-12 18:56:59.000000 rolo-0.4.0/tests/test_resource.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19653 2024-01-12 18:56:59.000000 rolo-0.4.0/tests/test_router.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.609844 rolo-0.5.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11358 2024-01-19 14:23:57.000000 rolo-0.5.0/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    17979 2024-04-21 12:32:17.609844 rolo-0.5.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3806 2024-04-20 18:20:27.000000 rolo-0.5.0/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1842 2024-04-21 12:31:07.000000 rolo-0.5.0/pyproject.toml
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      213 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23639 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/asgi.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5265 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/client.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2569 2024-04-20 16:50:09.000000 rolo-0.5.0/rolo/dispatcher.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo/gateway/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      458 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/gateway/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2602 2024-03-11 23:14:35.000000 rolo-0.5.0/rolo/gateway/asgi.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13158 2024-04-20 22:28:15.000000 rolo-0.5.0/rolo/gateway/chain.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2099 2024-04-20 19:23:29.000000 rolo-0.5.0/rolo/gateway/gateway.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2738 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/gateway/handlers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1600 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/gateway/wsgi.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7158 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/proxy.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-20 15:37:59.000000 rolo-0.5.0/rolo/py.typed
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11643 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/request.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4124 2024-04-20 20:08:01.000000 rolo-0.5.0/rolo/resource.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4414 2024-04-20 18:20:44.000000 rolo-0.5.0/rolo/response.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23041 2024-04-20 20:08:07.000000 rolo-0.5.0/rolo/router.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo/serving/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      227 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/serving/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    15148 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/serving/twisted.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo/testing/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-11 23:01:37.000000 rolo-0.5.0/rolo/testing/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8756 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/testing/pytest.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo/websocket/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      392 2024-03-11 23:14:35.000000 rolo-0.5.0/rolo/websocket/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4966 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/websocket/adapter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      685 2024-03-10 19:19:00.000000 rolo-0.5.0/rolo/websocket/errors.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9994 2024-03-11 23:14:41.000000 rolo-0.5.0/rolo/websocket/request.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      474 2024-03-11 23:14:35.000000 rolo-0.5.0/rolo/websocket/websocket.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/rolo.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    17979 2024-04-21 12:32:17.000000 rolo-0.5.0/rolo.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      848 2024-04-21 12:32:17.000000 rolo-0.5.0/rolo.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-04-21 12:32:17.000000 rolo-0.5.0/rolo.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      176 2024-04-21 12:32:17.000000 rolo-0.5.0/rolo.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        5 2024-04-21 12:32:17.000000 rolo-0.5.0/rolo.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-04-21 12:32:17.609844 rolo-0.5.0/setup.cfg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-04-21 12:32:17.605844 rolo-0.5.0/tests/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12809 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_asgi.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2790 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_dispatcher.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10977 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_proxy.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6293 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_request.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4679 2024-01-12 18:56:59.000000 rolo-0.5.0/tests/test_resource.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2568 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_response.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    19653 2024-04-20 20:07:52.000000 rolo-0.5.0/tests/test_router.py
```

### Comparing `rolo-0.4.0/LICENSE` & `rolo-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/PKG-INFO` & `rolo-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolo
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python framework for building HTTP-based server applications
 Author-email: LocalStack Contributors <info@localstack.cloud>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -257,15 +257,15 @@
 To allow asynchronous communication, Rolo introduces an ASGI/WSGI bridge, that allows you to serve Rolo applications through ASGI servers like Hypercorn.
 
 ## Usage
 
 ### Default router example
 
 ```python
-from rolo import Router
+from rolo import Router, route, Response
 from werkzeug import Request
 from werkzeug.serving import run_simple
 
 @route("/users")
 def user(_: Request, args):
     assert not args
     return Response("user")
@@ -276,16 +276,15 @@
     return Response(f"{args['user_id']}")
 
 router = Router()
 router.add(user)
 router.add(user_id)
 
 # convert Router to a WSGI app and serve it through werkzeug
-app = Request.application(router.dispatch)
-run_simple('localhost', 8080, app, use_reloader=True)
+run_simple('localhost', 8080, router.wsgi(), use_reloader=True)
 ```
 
 ### Gateway & Handler Chain
 
 A rolo `Gateway` holds a set of request, response, and exception handlers, as well as request finalizers.
 Gateway instances can then be served as WSGI or ASGI applications by using the appropriate serving adapter.
 Here is a simple example of a Gateway with just one handler that returns the URL and method that was invoked.
```

### Comparing `rolo-0.4.0/README.md` & `rolo-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 To allow asynchronous communication, Rolo introduces an ASGI/WSGI bridge, that allows you to serve Rolo applications through ASGI servers like Hypercorn.
 
 ## Usage
 
 ### Default router example
 
 ```python
-from rolo import Router
+from rolo import Router, route, Response
 from werkzeug import Request
 from werkzeug.serving import run_simple
 
 @route("/users")
 def user(_: Request, args):
     assert not args
     return Response("user")
@@ -44,16 +44,15 @@
     return Response(f"{args['user_id']}")
 
 router = Router()
 router.add(user)
 router.add(user_id)
 
 # convert Router to a WSGI app and serve it through werkzeug
-app = Request.application(router.dispatch)
-run_simple('localhost', 8080, app, use_reloader=True)
+run_simple('localhost', 8080, router.wsgi(), use_reloader=True)
 ```
 
 ### Gateway & Handler Chain
 
 A rolo `Gateway` holds a set of request, response, and exception handlers, as well as request finalizers.
 Gateway instances can then be served as WSGI or ASGI applications by using the appropriate serving adapter.
 Here is a simple example of a Gateway with just one handler that returns the URL and method that was invoked.
```

#### html2text {}

```diff
@@ -12,31 +12,31 @@
 introduces the concept of a `Gateway` and `HandlerChain`, an implementation
 variant of the [chain-of-responsibility pattern](https://en.wikipedia.org/wiki/
 Chain-of-responsibility_pattern). Rolo is designed for environments that do not
 use asyncio, but still require asynchronous HTTP features like HTTP2 SSE or
 Websockets. To allow asynchronous communication, Rolo introduces an ASGI/WSGI
 bridge, that allows you to serve Rolo applications through ASGI servers like
 Hypercorn. ## Usage ### Default router example ```python from rolo import
-Router from werkzeug import Request from werkzeug.serving import run_simple
-@route("/users") def user(_: Request, args): assert not args return Response
-("user") @route("/users/") def user_id(_: Request, args): assert args return
-Response(f"{args['user_id']}") router = Router() router.add(user) router.add
-(user_id) # convert Router to a WSGI app and serve it through werkzeug app =
-Request.application(router.dispatch) run_simple('localhost', 8080, app,
-use_reloader=True) ``` ### Gateway & Handler Chain A rolo `Gateway` holds a set
-of request, response, and exception handlers, as well as request finalizers.
-Gateway instances can then be served as WSGI or ASGI applications by using the
-appropriate serving adapter. Here is a simple example of a Gateway with just
-one handler that returns the URL and method that was invoked. ```python from
-werkzeug import run_simple from rolo import Response from rolo.gateway import
-Gateway, HandlerChain, RequestContext from rolo.gateway.wsgi import WsgiGateway
-def echo_handler(chain: HandlerChain, context: RequestContext, response:
-Response): response.status_code = 200 response.set_json({"url":
-context.request.url, "method": context.request.method}) gateway = Gateway
-(request_handlers=[echo_handler]) app = WsgiGateway(gateway) run_simple
-("localhost", 8080, app, use_reloader=True) ``` Serving this will yield:
-```console curl http://localhost:8080/hello-world {"url": "http://localhost:
-8080/hello-world", "method": "GET"} ``` ## Develop ### Quickstart to install
-the python and other developer requirements into a venv run: make install ###
-Format code We use black and isort as code style tools. To execute them, run:
-make format ### Build distribution To build a wheel and source distribution,
-simply run make dist
+Router, route, Response from werkzeug import Request from werkzeug.serving
+import run_simple @route("/users") def user(_: Request, args): assert not args
+return Response("user") @route("/users/") def user_id(_: Request, args): assert
+args return Response(f"{args['user_id']}") router = Router() router.add(user)
+router.add(user_id) # convert Router to a WSGI app and serve it through
+werkzeug run_simple('localhost', 8080, router.wsgi(), use_reloader=True) ```
+### Gateway & Handler Chain A rolo `Gateway` holds a set of request, response,
+and exception handlers, as well as request finalizers. Gateway instances can
+then be served as WSGI or ASGI applications by using the appropriate serving
+adapter. Here is a simple example of a Gateway with just one handler that
+returns the URL and method that was invoked. ```python from werkzeug import
+run_simple from rolo import Response from rolo.gateway import Gateway,
+HandlerChain, RequestContext from rolo.gateway.wsgi import WsgiGateway def
+echo_handler(chain: HandlerChain, context: RequestContext, response: Response):
+response.status_code = 200 response.set_json({"url": context.request.url,
+"method": context.request.method}) gateway = Gateway(request_handlers=
+[echo_handler]) app = WsgiGateway(gateway) run_simple("localhost", 8080, app,
+use_reloader=True) ``` Serving this will yield: ```console curl http://
+localhost:8080/hello-world {"url": "http://localhost:8080/hello-world",
+"method": "GET"} ``` ## Develop ### Quickstart to install the python and other
+developer requirements into a venv run: make install ### Format code We use
+black and isort as code style tools. To execute them, run: make format ###
+Build distribution To build a wheel and source distribution, simply run make
+dist
```

### Comparing `rolo-0.4.0/pyproject.toml` & `rolo-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rolo"
 authors = [
     { name = "LocalStack Contributors", email = "info@localstack.cloud" }
 ]
-version = "0.4.0"
+version = "0.5.0"
 description = "A Python framework for building HTTP-based server applications"
 dependencies = [
     "requests>=2.20",
     "werkzeug>=3.0"
 ]
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `rolo-0.4.0/rolo/asgi.py` & `rolo-0.5.0/rolo/asgi.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/client.py` & `rolo-0.5.0/rolo/client.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/dispatcher.py` & `rolo-0.5.0/rolo/dispatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from .router import Dispatcher, RequestArguments
 
 ResultValue = Union[
     WerkzeugResponse,
     str,
     bytes,
     Dict[str, Any],  # a JSON dict
+    list[Any],
 ]
 
 
 def _populate_response(
     response: WerkzeugResponse, result: ResultValue, json_encoder: Type[json.JSONEncoder]
 ):
     if result is None:
         return response
 
     elif isinstance(result, (str, bytes, bytearray)):
         response.data = result
-    elif isinstance(result, dict):
+    elif isinstance(result, (dict, list)):
         response.data = json.dumps(result, cls=json_encoder)
         response.mimetype = "application/json"
     else:
         raise ValueError("unhandled result type %s", type(result))
 
     return response
```

### Comparing `rolo-0.4.0/rolo/gateway/asgi.py` & `rolo-0.5.0/rolo/gateway/asgi.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/gateway/chain.py` & `rolo-0.5.0/rolo/gateway/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,20 @@
 
             # call response filters
             self._call_response_handlers(response)
         finally:
             if not self.finalized:
                 self._call_finalizers(response)
 
-    def respond(self, status_code: int = 200, payload: t.Any = None, headers: Headers = None):
+    def respond(
+        self,
+        status_code: int = 200,
+        payload: t.Any = None,
+        headers: t.Union[Headers, t.Mapping] = None,
+    ):
         """
         Convenience method for handlers to stop the chain and set the given status and payload to the
         current response object.
 
         :param status_code: the HTTP status code
         :param payload: the payload of the response
         :param headers: additional headers
```

### Comparing `rolo-0.4.0/rolo/gateway/gateway.py` & `rolo-0.5.0/rolo/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/gateway/handlers.py` & `rolo-0.5.0/rolo/gateway/handlers.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/gateway/wsgi.py` & `rolo-0.5.0/rolo/gateway/wsgi.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/proxy.py` & `rolo-0.5.0/rolo/proxy.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/request.py` & `rolo-0.5.0/rolo/request.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/resource.py` & `rolo-0.5.0/rolo/resource.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/response.py` & `rolo-0.5.0/rolo/response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import json
-from typing import Any, Dict, Iterable, Type, Union
+import mimetypes
+import typing as t
+from importlib import resources
 
+from werkzeug.exceptions import NotFound
 from werkzeug.wrappers import Response as WerkzeugResponse
 
+if t.TYPE_CHECKING:
+    from types import ModuleType
+
 
 class Response(WerkzeugResponse):
     """
     An HTTP Response object, which simply extends werkzeug's Response object with a few convenience methods.
     """
 
     def update_from(self, other: WerkzeugResponse):
@@ -18,26 +24,26 @@
         :param other: the response object to read from
         """
         self.status_code = other.status_code
         self.response = other.response
         self._on_close.extend(other._on_close)
         self.headers.update(other.headers)
 
-    def set_json(self, doc: Any, cls: Type[json.JSONEncoder] = None):
+    def set_json(self, doc: t.Any, cls: t.Type[json.JSONEncoder] = None):
         """
         Serializes the given dictionary using localstack's ``CustomEncoder`` into a json response, and sets the
         mimetype automatically to ``application/json``.
 
         :param doc: the response dictionary to be serialized as JSON
         :param cls: the JSON encoder class to use for serializing the passed document
         """
         self.data = json.dumps(doc, cls=cls)
         self.mimetype = "application/json"
 
-    def set_response(self, response: Union[str, bytes, bytearray, Iterable[bytes]]):
+    def set_response(self, response: t.Union[str, bytes, bytearray, t.Iterable[bytes]]):
         """
         Function to set the low-level ``response`` object. This is copied from the werkzeug Response constructor. The
         response attribute always holds an iterable of bytes. Passing a str, bytes or bytearray is equivalent to
         calling ``response.data = <response>``. If None is passed, then it will create an empty list. If anything
         else is passed, the value is set directly. This value can be a list of bytes, and iterator that returns bytes
         (e.g., a generator), which can be used by the underlying server to stream responses to the client. Anything else
         (like passing dicts) will result in errors at lower levels of the server.
@@ -49,30 +55,49 @@
         elif isinstance(response, (str, bytes, bytearray)):
             self.data = response
         else:
             self.response = response
 
         return self
 
-    def to_readonly_response_dict(self) -> Dict:
+    def to_readonly_response_dict(self) -> t.Dict:
         """
         Returns a read-only version of a response dictionary as it is often expected by other libraries like boto.
         """
         return {
             "body": self.stream if self.is_streamed else self.data,
             "status_code": self.status_code,
             "headers": dict(self.headers),
         }
 
     @classmethod
-    def for_json(cls, doc: Any, *args, **kwargs) -> "Response":
+    def for_json(cls, doc: t.Any, *args, **kwargs) -> "Response":
         """
         Creates a new JSON response from the given document. It automatically sets the mimetype to ``application/json``.
 
         :param doc: the document to serialize into JSON
         :param args: arguments passed to the ``Response`` constructor
         :param kwargs: keyword arguments passed to the ``Response`` constructor
         :return: a new Response object
         """
         response = cls(*args, **kwargs)
         response.set_json(doc)
         return response
+
+    @classmethod
+    def for_resource(cls, module: "ModuleType", path: str, *args, **kwargs) -> "Response":
+        """
+        Looks up the given file in the given module, and creates a new Response object with the contents of that
+        file. It guesses the mimetype of the file and sets it in the response accordingly. If the file does not exist
+        ,it raises a ``NotFound`` error.
+
+        :param module: the module to look up the file in
+        :param path: the path/file name
+        :return: a new Response object
+        """
+        resource = resources.files(module).joinpath(path)
+        if not resource.is_file():
+            raise NotFound()
+        mimetype = mimetypes.guess_type(resource.name)
+        mimetype = mimetype[0] if mimetype and mimetype[0] else "application/octet-stream"
+
+        return cls(resource.open("rb"), *args, mimetype=mimetype, **kwargs)
```

### Comparing `rolo-0.4.0/rolo/router.py` & `rolo-0.5.0/rolo/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 )
 
 from werkzeug import Request, Response
 from werkzeug.routing import BaseConverter, Map, Rule, RuleFactory
 
 from .request import get_raw_path
 
+if t.TYPE_CHECKING:
+    from _typeshed.wsgi import WSGIApplication
+
 HTTP_METHODS = ("GET", "POST", "PUT", "PATCH", "DELETE", "HEAD", "OPTIONS", "TRACE")
 
 E = TypeVar("E")
 RequestArguments = Mapping[str, Any]
 
 
 class RegexConverter(BaseConverter):
@@ -399,14 +402,31 @@
             r = route(path, host, methods, **kwargs)
             fn = r(fn)
             self.add(fn)
             return fn
 
         return wrapper
 
+    def wsgi(self) -> "WSGIApplication":
+        """
+        Returns this router as a WSGI compatible interface. This can be used to conveniently serve a Router instance
+        through a WSGI server, for instance werkzeug's dev server::
+
+            from werkzeug.serving import run_simple
+
+            from rolo import Router
+            from rolo.dispatcher import handler_dispatcher
+
+            router = Router(dispatcher=handler_dispatcher())
+            run_simple("localhost", 5000, router.wsgi())
+
+        :return: a WSGI callable that invokes this router
+        """
+        return Request.application(self.dispatch)
+
 
 class RuleAdapter(RuleFactory):
     """
     Takes something that can also be passed to ``Router.add``, and exposes it as a ``RuleFactory`` that generates the
     appropriate Werkzeug rules. This can be used in combination with other rule factories like ``Submount``,
     and creates general compatibility with werkzeug rules. Here's an example::
```

### Comparing `rolo-0.4.0/rolo/serving/twisted.py` & `rolo-0.5.0/rolo/serving/twisted.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/testing/pytest.py` & `rolo-0.5.0/rolo/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/websocket/adapter.py` & `rolo-0.5.0/rolo/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/websocket/errors.py` & `rolo-0.5.0/rolo/websocket/errors.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo/websocket/request.py` & `rolo-0.5.0/rolo/websocket/request.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/rolo.egg-info/PKG-INFO` & `rolo-0.5.0/rolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolo
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python framework for building HTTP-based server applications
 Author-email: LocalStack Contributors <info@localstack.cloud>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -257,15 +257,15 @@
 To allow asynchronous communication, Rolo introduces an ASGI/WSGI bridge, that allows you to serve Rolo applications through ASGI servers like Hypercorn.
 
 ## Usage
 
 ### Default router example
 
 ```python
-from rolo import Router
+from rolo import Router, route, Response
 from werkzeug import Request
 from werkzeug.serving import run_simple
 
 @route("/users")
 def user(_: Request, args):
     assert not args
     return Response("user")
@@ -276,16 +276,15 @@
     return Response(f"{args['user_id']}")
 
 router = Router()
 router.add(user)
 router.add(user_id)
 
 # convert Router to a WSGI app and serve it through werkzeug
-app = Request.application(router.dispatch)
-run_simple('localhost', 8080, app, use_reloader=True)
+run_simple('localhost', 8080, router.wsgi(), use_reloader=True)
 ```
 
 ### Gateway & Handler Chain
 
 A rolo `Gateway` holds a set of request, response, and exception handlers, as well as request finalizers.
 Gateway instances can then be served as WSGI or ASGI applications by using the appropriate serving adapter.
 Here is a simple example of a Gateway with just one handler that returns the URL and method that was invoked.
```

### Comparing `rolo-0.4.0/rolo.egg-info/SOURCES.txt` & `rolo-0.5.0/rolo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 rolo/__init__.py
 rolo/asgi.py
 rolo/client.py
 rolo/dispatcher.py
 rolo/proxy.py
+rolo/py.typed
 rolo/request.py
 rolo/resource.py
 rolo/response.py
 rolo/router.py
 rolo.egg-info/PKG-INFO
 rolo.egg-info/SOURCES.txt
 rolo.egg-info/dependency_links.txt
@@ -31,8 +32,9 @@
 rolo/websocket/request.py
 rolo/websocket/websocket.py
 tests/test_asgi.py
 tests/test_dispatcher.py
 tests/test_proxy.py
 tests/test_request.py
 tests/test_resource.py
+tests/test_response.py
 tests/test_router.py
```

### Comparing `rolo-0.4.0/tests/test_asgi.py` & `rolo-0.5.0/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/tests/test_dispatcher.py` & `rolo-0.5.0/tests/test_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,29 @@
 
         def handler(_request: Request, arg1) -> Dict[str, Any]:
             return {"arg1": arg1, "hello": "there"}
 
         router.add("/foo/<arg1>", handler)
         assert router.dispatch(Request("GET", "/foo/a")).json == {"arg1": "a", "hello": "there"}
 
+    def test_handler_dispatcher_with_list_return(self):
+        router = Router(dispatcher=handler_dispatcher())
+
+        def handler(_request: Request, arg1) -> Dict[str, Any]:
+            return [{"arg1": arg1, "hello": "there"}, 1, 2, "3", [4, 5]]
+
+        router.add("/foo/<arg1>", handler)
+        assert router.dispatch(Request("GET", "/foo/a")).json == [
+            {"arg1": "a", "hello": "there"},
+            1,
+            2,
+            "3",
+            [4, 5],
+        ]
+
     def test_handler_dispatcher_with_text_return(self):
         router = Router(dispatcher=handler_dispatcher())
 
         def handler(_request: Request, arg1) -> str:
             return f"hello: {arg1}"
 
         router.add("/<arg1>", handler)
```

### Comparing `rolo-0.4.0/tests/test_proxy.py` & `rolo-0.5.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/tests/test_request.py` & `rolo-0.5.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/tests/test_resource.py` & `rolo-0.5.0/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `rolo-0.4.0/tests/test_router.py` & `rolo-0.5.0/tests/test_router.py`

 * *Files identical despite different names*

