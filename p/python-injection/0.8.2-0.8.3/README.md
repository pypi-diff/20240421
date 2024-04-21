# Comparing `tmp/python_injection-0.8.2.tar.gz` & `tmp/python_injection-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.8.2.tar", max compression
+gzip compressed data, was "python_injection-0.8.3.tar", max compression
```

## Comparing `python_injection-0.8.2.tar` & `python_injection-0.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3047 2024-04-11 08:00:09.618740 python_injection-0.8.2/documentation/basic-usage.md
--rw-r--r--   0        0        0      609 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/__init__.py
--rw-r--r--   0        0        0     5395 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/__init__.pyi
--rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/__init__.py
--rw-r--r--   0        0        0     1316 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/event.py
--rw-r--r--   0        0        0      558 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/invertible.py
--rw-r--r--   0        0        0     1401 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/lazy.py
--rw-r--r--   0        0        0     1443 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/queue.py
--rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/__init__.py
--rw-r--r--   0        0        0      271 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/threading.py
--rw-r--r--   0        0        0     1276 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/type.py
--rw-r--r--   0        0        0       22 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/core/__init__.py
--rw-r--r--   0        0        0    19663 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/core/module.py
--rw-r--r--   0        0        0      653 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/integrations/__init__.py
--rw-r--r--   0        0        0      723 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/integrations/blacksheep.py
--rw-r--r--   0        0        0      676 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/utils.py
--rw-r--r--   0        0        0     1206 2024-04-11 08:00:32.710757 python_injection-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 python_injection-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     3048 2024-04-21 14:28:43.510689 python_injection-0.8.3/documentation/basic-usage.md
+-rw-r--r--   0        0        0      685 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/__init__.py
+-rw-r--r--   0        0        0     5755 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/__init__.py
+-rw-r--r--   0        0        0     1316 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/event.py
+-rw-r--r--   0        0        0      558 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/invertible.py
+-rw-r--r--   0        0        0     1401 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/lazy.py
+-rw-r--r--   0        0        0     1443 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/queue.py
+-rw-r--r--   0        0        0        0 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/tools/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/tools/threading.py
+-rw-r--r--   0        0        0     1276 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/common/tools/type.py
+-rw-r--r--   0        0        0       22 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/core/__init__.py
+-rw-r--r--   0        0        0    20545 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/core/module.py
+-rw-r--r--   0        0        0      653 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/integrations/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/integrations/blacksheep.py
+-rw-r--r--   0        0        0      676 2024-04-21 14:28:43.514689 python_injection-0.8.3/injection/utils.py
+-rw-r--r--   0        0        0     1206 2024-04-21 14:29:02.051055 python_injection-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 python_injection-0.8.3/PKG-INFO
```

### Comparing `python_injection-0.8.2/documentation/basic-usage.md` & `python_injection-0.8.3/documentation/basic-usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     ...
 
 @injectable(on=(AbstractService, ConcreteService))
 class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
-If a class is registered in a package and you want to override it, there is the `mode` parameter:
+If a class is registered in a package, and you want to override it, there is the `mode` parameter:
 
 ```python
 @injectable
 class InaccessibleService:
     ...
 
 # ...
```

### Comparing `python_injection-0.8.2/injection/__init__.py` & `python_injection-0.8.3/injection/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .core import Injectable, Module
+from .core import Injectable, InjectableMode, Module, ModulePriority
 
 __all__ = (
     "Injectable",
+    "InjectableMode",
     "Module",
+    "ModulePriority",
     "default_module",
     "get_instance",
     "get_lazy_instance",
     "inject",
     "injectable",
     "set_constant",
     "should_be_injectable",
```

### Comparing `python_injection-0.8.2/injection/__init__.pyi` & `python_injection-0.8.3/injection/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import abstractmethod
 from collections.abc import Callable, Iterable
 from contextlib import ContextDecorator
+from enum import Enum
 from types import UnionType
 from typing import (
     Any,
     ContextManager,
     Final,
     Literal,
     Protocol,
@@ -50,30 +51,30 @@
         self,
         wrapped: Callable[..., Any] = ...,
         /,
         *,
         cls: type[Injectable] = ...,
         inject: bool = ...,
         on: type | Iterable[type] | UnionType = ...,
-        mode: Literal["fallback", "normal", "override"] = ...,
+        mode: InjectableMode | Literal["fallback", "normal", "override"] = ...,
     ):
         """
         Decorator applicable to a class or function. It is used to indicate how the
         injectable will be constructed. At injection time, a new instance will be
         injected each time.
         """
 
     def singleton(
         self,
         wrapped: Callable[..., Any] = ...,
         /,
         *,
         inject: bool = ...,
         on: type | Iterable[type] | UnionType = ...,
-        mode: Literal["fallback", "normal", "override"] = ...,
+        mode: InjectableMode | Literal["fallback", "normal", "override"] = ...,
     ):
         """
         Decorator applicable to a class or function. It is used to indicate how the
         singleton will be constructed. At injection time, the injected instance will
         always be the same.
         """
 
@@ -85,15 +86,15 @@
         """
 
     def set_constant(
         self,
         instance: _T,
         on: type | Iterable[type] | UnionType = ...,
         *,
-        mode: Literal["fallback", "normal", "override"] = ...,
+        mode: InjectableMode | Literal["fallback", "normal", "override"] = ...,
     ) -> _T:
         """
         Function for registering a specific instance to be injected. This is useful for
         registering global variables. The difference with the singleton decorator is
         that no dependencies are resolved, so the module doesn't need to be locked.
         """
 
@@ -115,15 +116,20 @@
         parameter or `None`. Return a `Invertible` object. To access the instance
         contained in an invertible object, simply use a wavy line (~).
         With `cache=True`, the instance retrieved will always be the same.
 
         Example: instance = ~lazy_instance
         """
 
-    def use(self, module: Module, *, priority: Literal["low", "high"] = ...):
+    def use(
+        self,
+        module: Module,
+        *,
+        priority: ModulePriority | Literal["low", "high"] = ...,
+    ):
         """
         Function for using another module. Using another module replaces the module's
         dependencies with those of the module used. If the dependency is not found, it
         will be searched for in the module's dependency container.
         """
 
     def stop_using(self, module: Module):
@@ -131,35 +137,50 @@
         Function to remove a module in use.
         """
 
     def use_temporarily(
         self,
         module: Module,
         *,
-        priority: Literal["low", "high"] = ...,
+        priority: ModulePriority | Literal["low", "high"] = ...,
     ) -> ContextManager | ContextDecorator:
         """
         Context manager or decorator for temporary use of a module.
         """
 
-    def change_priority(self, module: Module, priority: Literal["low", "high"]):
+    def change_priority(
+        self,
+        module: Module,
+        priority: ModulePriority | Literal["low", "high"],
+    ):
         """
         Function for changing the priority of a module in use.
         There are two priority values:
 
         * **LOW**: The module concerned becomes the least important of the modules used.
         * **HIGH**: The module concerned becomes the most important of the modules used.
         """
 
     def unlock(self):
         """
         Function to unlock the module by deleting cached instances of singletons.
         """
 
+@final
+class ModulePriority(str, Enum):
+    LOW = ...
+    HIGH = ...
+
 @runtime_checkable
 class Injectable(Protocol[_T]):
     def __init__(self, factory: Callable[[], _T] = ..., /): ...
     @property
     def is_locked(self) -> bool: ...
     def unlock(self): ...
     @abstractmethod
     def get_instance(self) -> _T: ...
+
+@final
+class InjectableMode(str, Enum):
+    FALLBACK = ...
+    NORMAL = ...
+    OVERRIDE = ...
```

### Comparing `python_injection-0.8.2/injection/common/event.py` & `python_injection-0.8.3/injection/common/event.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/common/invertible.py` & `python_injection-0.8.3/injection/common/invertible.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/common/lazy.py` & `python_injection-0.8.3/injection/common/lazy.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/common/queue.py` & `python_injection-0.8.3/injection/common/queue.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/common/tools/type.py` & `python_injection-0.8.3/injection/common/tools/type.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/core/module.py` & `python_injection-0.8.3/injection/core/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     Iterable,
     Iterator,
     Mapping,
     MutableMapping,
 )
 from contextlib import ContextDecorator, contextmanager, suppress
 from dataclasses import dataclass, field
+from enum import Enum
 from functools import partialmethod, singledispatchmethod, update_wrapper
 from inspect import Signature, isclass
 from types import MethodType, UnionType
 from typing import (
     Any,
     ClassVar,
     ContextManager,
     Literal,
     NamedTuple,
     NoReturn,
     Protocol,
     TypeVar,
     cast,
-    get_args,
     runtime_checkable,
 )
 
 from injection.common.event import Event, EventChannel, EventListener
 from injection.common.invertible import Invertible, SimpleInvertible
 from injection.common.lazy import Lazy, LazyMapping
 from injection.common.queue import LimitedQueue
@@ -41,45 +41,36 @@
     InjectionError,
     ModuleError,
     ModuleLockError,
     ModuleNotUsedError,
     NoInjectable,
 )
 
-__all__ = ("Injectable", "Module")
+__all__ = ("Injectable", "InjectableMode", "Module", "ModulePriority")
 
 _logger = logging.getLogger(__name__)
 
 _T = TypeVar("_T")
 _Types = Iterable[type] | UnionType
 
 
 """
-Literal types
-"""
-
-
-_Mode = Literal["fallback", "normal", "override"]
-_Priority = Literal["low", "high"]
-
-
-"""
 Events
 """
 
 
 @dataclass(frozen=True, slots=True)
 class ContainerEvent(Event, ABC):
     on_container: Container
 
 
 @dataclass(frozen=True, slots=True)
 class ContainerDependenciesUpdated(ContainerEvent):
     classes: Collection[type]
-    mode: _Mode
+    mode: InjectableMode
 
     def __str__(self) -> str:
         length = len(self.classes)
         formatted_classes = ", ".join(f"`{format_type(cls)}`" for cls in self.classes)
         return (
             f"{length} container dependenc{'ies' if length > 1 else 'y'} have been "
             f"updated{f': {formatted_classes}' if formatted_classes else ''}."
@@ -109,14 +100,15 @@
     def origin(self) -> Event:
         return next(self.history)
 
 
 @dataclass(frozen=True, slots=True)
 class ModuleAdded(ModuleEvent):
     module_added: Module
+    priority: ModulePriority
 
     def __str__(self) -> str:
         return f"`{self.on_module}` now uses `{self.module_added}`."
 
 
 @dataclass(frozen=True, slots=True)
 class ModuleRemoved(ModuleEvent):
@@ -125,15 +117,15 @@
     def __str__(self) -> str:
         return f"`{self.on_module}` no longer uses `{self.module_removed}`."
 
 
 @dataclass(frozen=True, slots=True)
 class ModulePriorityUpdated(ModuleEvent):
     module_updated: Module
-    priority: _Priority
+    priority: ModulePriority
 
     def __str__(self) -> str:
         return (
             f"In `{self.on_module}`, the priority `{self.priority}` "
             f"has been applied to `{self.module_updated}`."
         )
 
@@ -237,58 +229,76 @@
 
 
 """
 Container
 """
 
 
+class InjectableMode(str, Enum):
+    FALLBACK = "fallback"
+    NORMAL = "normal"
+    OVERRIDE = "override"
+
+    @property
+    def rank(self) -> int:
+        return tuple(type(self)).index(self)
+
+    @classmethod
+    def get_default(cls):
+        return cls.NORMAL
+
+
+_Mode = InjectableMode | Literal["fallback", "normal", "override"]
+
+
 class Record(NamedTuple):
     injectable: Injectable
-    mode: _Mode
+    mode: InjectableMode
 
 
 @dataclass(repr=False, frozen=True, slots=True)
 class Container(Broker):
-    __data: dict[type, Record] = field(default_factory=dict, init=False)
+    __records: dict[type, Record] = field(default_factory=dict, init=False)
     __channel: EventChannel = field(default_factory=EventChannel, init=False)
 
     def __getitem__(self, cls: type[_T] | UnionType, /) -> Injectable[_T]:
         for cls in get_origins(cls):
             try:
-                injectable, _ = self.__data[cls]
+                injectable, _ = self.__records[cls]
             except KeyError:
                 continue
 
             return injectable
 
         raise NoInjectable(cls)
 
     def __contains__(self, cls: type | UnionType, /) -> bool:
-        return any(cls in self.__data for cls in get_origins(cls))
+        return any(cls in self.__records for cls in get_origins(cls))
 
     @property
     def is_locked(self) -> bool:
         return any(injectable.is_locked for injectable in self.__injectables)
 
     @property
     def __injectables(self) -> frozenset[Injectable]:
-        return frozenset(injectable for injectable, _ in self.__data.values())
+        return frozenset(injectable for injectable, _ in self.__records.values())
 
     @synchronized()
     def update(self, classes: Iterable[type], injectable: Injectable, mode: _Mode):
+        mode = InjectableMode(mode)
         records = {
             cls: Record(injectable, mode)
             for cls in self.__filter_classes(classes, mode)
         }
 
         if records:
             event = ContainerDependenciesUpdated(self, records.keys(), mode)
 
             with self.notify(event):
-                self.__data.update(records)
+                self.__records.update(records)
 
         return self
 
     @synchronized()
     def unlock(self):
         for injectable in self.__injectables:
             injectable.unlock()
@@ -298,42 +308,57 @@
     def add_listener(self, listener: EventListener):
         self.__channel.add_listener(listener)
         return self
 
     def notify(self, event: Event) -> ContextManager | ContextDecorator:
         return self.__channel.dispatch(event)
 
-    def __filter_classes(self, classes: Iterable[type], mode: _Mode) -> Iterator[type]:
-        modes = get_args(_Mode)
-        rank = modes.index(mode)
+    def __filter_classes(
+        self,
+        classes: Iterable[type],
+        mode: InjectableMode,
+    ) -> Iterator[type]:
+        rank = mode.rank
 
         for cls in frozenset(get_origins(*classes)):
             try:
-                _, current_mode = self.__data[cls]
+                _, current_mode = self.__records[cls]
 
             except KeyError:
                 pass
 
             else:
                 if mode == current_mode:
                     raise RuntimeError(
                         f"An injectable already exists for the class `{format_type(cls)}`."
                     )
 
-                elif rank < modes.index(current_mode):
+                elif rank < current_mode.rank:
                     continue
 
             yield cls
 
 
 """
 Module
 """
 
 
+class ModulePriority(str, Enum):
+    LOW = "low"
+    HIGH = "high"
+
+    @classmethod
+    def get_default(cls):
+        return cls.LOW
+
+
+_Priority = ModulePriority | Literal["low", "high"]
+
+
 @dataclass(repr=False, eq=False, frozen=True, slots=True)
 class Module(EventListener, Broker):
     name: str = field(default=None)
     __channel: EventChannel = field(default_factory=EventChannel, init=False)
     __container: Container = field(default_factory=Container, init=False)
     __modules: OrderedDict[Module, None] = field(
         default_factory=OrderedDict,
@@ -372,15 +397,15 @@
         self,
         wrapped: Callable[..., Any] = None,
         /,
         *,
         cls: type[Injectable] = NewInjectable,
         inject: bool = True,
         on: type | _Types = None,
-        mode: _Mode = "normal",
+        mode: _Mode = InjectableMode.get_default(),
     ):
         def decorator(wp):
             factory = self.inject(wp, return_factory=True) if inject else wp
             injectable = cls(factory)
             classes = find_types(wp, on)
             self.update(classes, injectable, mode)
             return wp
@@ -390,26 +415,26 @@
     singleton = partialmethod(injectable, cls=SingletonInjectable)
 
     def should_be_injectable(self, wrapped: type = None, /):
         def decorator(wp):
             self.update(
                 (wp,),
                 ShouldBeInjectable(wp),
-                mode="fallback",
+                mode=InjectableMode.FALLBACK,
             )
             return wp
 
         return decorator(wrapped) if wrapped else decorator
 
     def set_constant(
         self,
         instance: _T,
         on: type | _Types = None,
         *,
-        mode: _Mode = "normal",
+        mode: _Mode = InjectableMode.get_default(),
     ) -> _T:
         cls = type(instance)
         self.injectable(
             lambda: instance,
             inject=False,
             on=(cls, on),
             mode=mode,
@@ -464,27 +489,33 @@
         function.set_owner(cls)
         return SimpleInvertible(function)
 
     def update(
         self,
         classes: Iterable[type],
         injectable: Injectable,
-        mode: _Mode = "normal",
+        mode: _Mode = InjectableMode.get_default(),
     ):
         self.__container.update(classes, injectable, mode)
         return self
 
-    def use(self, module: Module, *, priority: _Priority = "low"):
+    def use(
+        self,
+        module: Module,
+        *,
+        priority: _Priority = ModulePriority.get_default(),
+    ):
         if module is self:
             raise ModuleError("Module can't be used by itself.")
 
         if module in self.__modules:
             raise ModuleError(f"`{self}` already uses `{module}`.")
 
-        event = ModuleAdded(self, module)
+        priority = ModulePriority(priority)
+        event = ModuleAdded(self, module, priority)
 
         with self.notify(event):
             self.__modules[module] = None
             self.__move_module(module, priority)
             module.add_listener(self)
 
         return self
@@ -500,21 +531,22 @@
         return self
 
     @contextmanager
     def use_temporarily(
         self,
         module: Module,
         *,
-        priority: _Priority = "low",
+        priority: _Priority = ModulePriority.get_default(),
     ) -> ContextManager | ContextDecorator:
         self.use(module, priority=priority)
         yield
         self.stop_using(module)
 
     def change_priority(self, module: Module, priority: _Priority):
+        priority = ModulePriority(priority)
         event = ModulePriorityUpdated(self, module, priority)
 
         with self.notify(event):
             self.__move_module(module, priority)
 
         return self
 
@@ -545,16 +577,16 @@
             yield
             _logger.debug(event)
 
     def __check_locking(self):
         if self.is_locked:
             raise ModuleLockError(f"`{self}` is locked.")
 
-    def __move_module(self, module: Module, priority: _Priority):
-        last = priority != "high"
+    def __move_module(self, module: Module, priority: ModulePriority):
+        last = priority != ModulePriority.HIGH
 
         try:
             self.__modules.move_to_end(module, last=last)
         except KeyError as exc:
             raise ModuleNotUsedError(
                 f"`{module}` can't be found in the modules used by `{self}`."
             ) from exc
@@ -642,22 +674,15 @@
         "__wrapped__",
         "__dependencies",
         "__owner",
         "__setup_queue",
     )
 
     def __init__(self, wrapped: Callable[..., Any], /):
-        try:
-            variables = vars(wrapped)
-        except TypeError:
-            pass
-        else:
-            self.__update_vars(variables)
-            del variables
-
+        self.__update_vars_from(wrapped)
         update_wrapper(self, wrapped, updated=())
         self.__dependencies = Dependencies.empty()
         self.__owner = None
         self.__setup_queue = LimitedQueue[Callable[[], Any]]()
         self.on_setup(self.__set_signature)
 
     def __repr__(self) -> str:
@@ -741,15 +766,23 @@
         yield
         self.update(event.on_module)
 
     def __set_signature(self):
         self.__signature__ = inspect.signature(self.wrapped, eval_str=True)
         return self
 
-    def __update_vars(self, variables: Mapping[str, Any], /):
+    def __update_vars_from(self, obj: Any):
+        try:
+            variables = vars(obj)
+        except TypeError:
+            pass
+        else:
+            self.__update_vars(variables)
+
+    def __update_vars(self, variables: Mapping[str, Any]):
         def is_dunder(var: str) -> bool:
             return var.startswith("__") and var.endswith("__")
 
         restricted_vars = frozenset(var for var in dir(self) if not is_dunder(var))
         variables = (
             (var, value)
             for var, value in variables.items()
```

### Comparing `python_injection-0.8.2/injection/exceptions.py` & `python_injection-0.8.3/injection/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/integrations/blacksheep.py` & `python_injection-0.8.3/injection/integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/injection/utils.py` & `python_injection-0.8.3/injection/utils.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.2/pyproject.toml` & `python_injection-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.8.2"
+version = "0.8.3"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "documentation/basic-usage.md"
 repository = "https://github.com/100nm/python-injection"
```

### Comparing `python_injection-0.8.2/PKG-INFO` & `python_injection-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.8.2
+Version: 0.8.3
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/100nm/python-injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -132,15 +132,15 @@
     ...
 
 @injectable(on=(AbstractService, ConcreteService))
 class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
-If a class is registered in a package and you want to override it, there is the `mode` parameter:
+If a class is registered in a package, and you want to override it, there is the `mode` parameter:
 
 ```python
 @injectable
 class InaccessibleService:
     ...
 
 # ...
```

