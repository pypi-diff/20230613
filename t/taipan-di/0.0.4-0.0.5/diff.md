# Comparing `tmp/taipan_di-0.0.4.tar.gz` & `tmp/taipan_di-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.4.tar", max compression
+gzip compressed data, was "taipan_di-0.0.5.tar", max compression
```

## Comparing `taipan_di-0.0.4.tar` & `taipan_di-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-06-08 10:19:39.479355 taipan_di-0.0.4/LICENSE
--rw-r--r--   0        0        0     2988 2023-06-08 10:19:39.479355 taipan_di-0.0.4/README.md
--rw-r--r--   0        0        0     1004 2023-06-08 10:19:39.479355 taipan_di-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      152 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/__init__.py
--rw-r--r--   0        0        0       21 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/__version__.py
--rw-r--r--   0        0        0      115 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     4296 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      676 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      702 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3696 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0       83 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      474 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      594 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      364 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/__init__.py
--rw-r--r--   0        0        0      872 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_factory.py
--rw-r--r--   0        0        0      538 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_link.py
--rw-r--r--   0        0        0     1902 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_registrator.py
--rw-r--r--   0        0        0      780 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_factory.py
--rw-r--r--   0        0        0      652 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_link.py
--rw-r--r--   0        0        0     1740 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_registrator.py
--rw-r--r--   0        0        0      267 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       38 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      105 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      108 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_registration_error.py
--rw-r--r--   0        0        0      100 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      108 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      157 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      938 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0     1029 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      519 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/py.typed
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 taipan_di-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 15:12:31.390871 taipan_di-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2988 2023-06-13 15:12:31.390871 taipan_di-0.0.5/README.md
+-rw-r--r--   0        0        0     1004 2023-06-13 15:12:31.390871 taipan_di-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      534 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_collection.py
+-rw-r--r--   0        0        0      703 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_container.py
+-rw-r--r--   0        0        0      736 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_provider.py
+-rw-r--r--   0        0        0     3689 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/instanciate_service.py
+-rw-r--r--   0        0        0      130 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      625 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0      559 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/__init__.py
+-rw-r--r--   0        0        0      929 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_factory.py
+-rw-r--r--   0        0        0      590 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_link.py
+-rw-r--r--   0        0        0     2047 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_registrator.py
+-rw-r--r--   0        0        0      811 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_factory.py
+-rw-r--r--   0        0        0      665 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_link.py
+-rw-r--r--   0        0        0     1775 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_registrator.py
+-rw-r--r--   0        0        0      415 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      142 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      148 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_registration_error.py
+-rw-r--r--   0        0        0      132 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_type_error.py
+-rw-r--r--   0        0        0      148 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      236 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_dependency_container.py
+-rw-r--r--   0        0        0     1059 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_dependency_provider.py
+-rw-r--r--   0        0        0      544 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/py.typed
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 taipan_di-0.0.5/PKG-INFO
```

### Comparing `taipan_di-0.0.4/LICENSE` & `taipan_di-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.4/README.md` & `taipan_di-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.4/pyproject.toml` & `taipan_di-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.4"
+version = "0.0.5"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/dependency_collection.py` & `taipan_di-0.0.5/taipan_di/classes/dependency_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .tools import (
     PipelineLink,
     PipelineRegistrator,
     ChainOfResponsibilityLink,
     ChainOfResponsibilityRegistrator,
 )
 
+__all__ = ["DependencyCollection"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class DependencyCollection:
     def __init__(self) -> None:
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/dependency_container.py` & `taipan_di-0.0.5/taipan_di/classes/dependency_container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import Dict, Type, TypeVar, cast
 
 from taipan_di.interfaces import BaseDependencyContainer, BaseDependencyProvider, BaseScope
 
 from .dependency_provider import DependencyProvider
 
+__all__ = ["DependencyContainer"]
+
 T = TypeVar("T")
 
 
 class DependencyContainer(BaseDependencyContainer):
     def __init__(self) -> None:
         self._services = cast(Dict[Type, BaseScope], {})
 
     def contains(self, type: Type[T]) -> bool:
         return type in self._services
 
     def register(self, type: Type, service: BaseScope) -> None:
         self._services[type] = service
-        
+
     def build(self) -> BaseDependencyProvider:
         provider = DependencyProvider(self._services)
         return provider
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/dependency_provider.py` & `taipan_di-0.0.5/taipan_di/classes/dependency_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Dict, Type, TypeVar
 
 from taipan_di.errors import TaipanUnregisteredError
 from taipan_di.interfaces import BaseDependencyProvider, BaseScope
 
+__all__ = ["DependencyProvider"]
+
 T = TypeVar("T")
 
 
 class DependencyProvider(BaseDependencyProvider):
     def __init__(self, services: Dict[Type, BaseScope]) -> None:
         self._services = services.copy()
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.5/taipan_di/classes/instanciate_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,18 @@
     cast,
 )
 from typing_extensions import Protocol
 
 from taipan_di.interfaces import BaseDependencyProvider
 from taipan_di.errors import TaipanInjectionError, TaipanTypeError
 
+__all__ = ["instanciate_service"]
 
 S = TypeVar("S")
 
-ServiceDefinition = Type[S]
-ServiceResult = S
-
 Undefined = NewType("Undefined", int)
 
 
 class _ProtocolInit(Protocol):
     pass
 
 
@@ -101,18 +99,18 @@
     return resolved_kwargs
 
 
 def instanciate_service(service: Type[S], provider: BaseDependencyProvider) -> S:
     constructor = getattr(service, "__init__")
 
     # ignore abstract class initialiser and protocol initialisers
-    if (
-        constructor in [ABC.__init__, _no_init] or constructor.__name__ == "_no_init"
-    ):
-        raise TaipanTypeError(f"{str(service)} has no __init__, cannot instanciate the service")
+    if constructor in [ABC.__init__, _no_init] or constructor.__name__ == "_no_init":
+        raise TaipanTypeError(
+            f"{str(service)} has no __init__, cannot instanciate the service"
+        )
 
     # Add class definition to dependency injection
     parameters = _inspect_function_arguments(constructor)
     parameters_name = tuple([p for p in parameters.keys() if p != "self"])
 
     def _resolve_kwargs() -> dict:
         if len(parameters_name) == 0:
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.5/taipan_di/classes/scopes/singleton_scope.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Any, Callable, Type, TypeVar, cast
 
 from taipan_di.interfaces import BaseDependencyProvider, BaseScope
 
+__all__ = ["SingletonScope"]
+
 T = TypeVar("T")
 
+
 class SingletonScope(BaseScope):
     def __init__(self, creator: Callable[[BaseDependencyProvider], Any]) -> None:
         self._creator = creator
         self._memoized_instance = None
 
     def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
         if self._memoized_instance is None:
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_factory.py` & `taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from typing import Generic, List, TypeVar
 
 from taipan_di.classes.tools import ChainOfResponsibilityLink
 from taipan_di.errors import TaipanRegistrationError
 
+__all__ = ["ChainOfResponsibilityFactory"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class ChainOfResponsibilityFactory(Generic[T, U]):
     def __init__(self) -> None:
         self._links: List[ChainOfResponsibilityLink[T, U]] = []
-        
-    def add(self, link: ChainOfResponsibilityLink[T, U]) -> "ChainOfResponsibilityFactory[T, U]":
+
+    def add(
+        self, link: ChainOfResponsibilityLink[T, U]
+    ) -> "ChainOfResponsibilityFactory[T, U]":
         self._links.append(link)
         return self
-    
+
     def build(self) -> ChainOfResponsibilityLink[T, U]:
         if len(self._links) == 0:
-            raise TaipanRegistrationError(f"ChainOfResponsibility[{str(T)}, {str(U)}] is empty ! Add at least one link")
-        
+            raise TaipanRegistrationError(
+                f"ChainOfResponsibility[{str(T)}, {str(U)}] is empty ! Add at least one link"
+            )
+
         for i in range(len(self._links) - 1):
             self._links[i]._set_next(self._links[i + 1])
-            
-        return self._links[0]
+
+        return self._links[0]
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_link.py` & `taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_link.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import abc
 from typing import Generic, TypeVar
 
+__all__ = ["ChainOfResponsibilityLink"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class ChainOfResponsibilityLink(Generic[T, U], metaclass=abc.ABCMeta):
     def __init__(self) -> None:
         self._next = None
-    
-    def _set_next(self, next: "ChainOfResponsibilityLink[T, U]") -> "ChainOfResponsibilityLink[T, U]":
+
+    def _set_next(
+        self, next: "ChainOfResponsibilityLink[T, U]"
+    ) -> "ChainOfResponsibilityLink[T, U]":
         self._next = next
         return self._next
 
     @abc.abstractmethod
     def handle(self, request: T) -> U:
         if self._next is not None:
             return self._next.handle(request)
 
-        return None
+        return None
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_registrator.py` & `taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_registrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from taipan_di.interfaces import BaseDependencyProvider
 
 from taipan_di.classes import instanciate_service
 
 if TYPE_CHECKING:
     from taipan_di.classes import DependencyCollection
 
+__all__ = ["ChainOfResponsibilityRegistrator"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class ChainOfResponsibilityRegistrator(Generic[T, U]):
     def __init__(
         self,
@@ -22,30 +24,38 @@
         as_singleton=False,
     ) -> None:
         self._interface_type = interface_type
         self._services = services
         self._as_singleton = as_singleton
         self._link_types: List[Type[ChainOfResponsibilityLink[T, U]]] = []
 
-    def add(self, link: Type[ChainOfResponsibilityLink[T, U]]) -> ChainOfResponsibilityRegistrator[T, U]:
+    def add(
+        self, link: Type[ChainOfResponsibilityLink[T, U]]
+    ) -> ChainOfResponsibilityRegistrator[T, U]:
         self._link_types.append(link)
         return self
 
     def register(self) -> None:
         if len(self._link_types) == 0:
             raise TaipanRegistrationError(
                 f"Pipeline[{str(T)}, {str(U)}] is empty ! Add at least one link"
             )
 
-        def create_chain_of_responsibility(provider: BaseDependencyProvider) -> ChainOfResponsibilityLink[T, U]:
+        def create_chain_of_responsibility(
+            provider: BaseDependencyProvider,
+        ) -> ChainOfResponsibilityLink[T, U]:
             factory = ChainOfResponsibilityFactory[T, U]()
 
             for link_type in self._link_types:
                 link = instanciate_service.instanciate_service(link_type, provider)
                 factory.add(link)
 
             return factory.build()
 
         if self._as_singleton:
-            self._services.register_singleton_creator(self._interface_type, create_chain_of_responsibility)
+            self._services.register_singleton_creator(
+                self._interface_type, create_chain_of_responsibility
+            )
         else:
-            self._services.register_factory_creator(self._interface_type, create_chain_of_responsibility)
+            self._services.register_factory_creator(
+                self._interface_type, create_chain_of_responsibility
+            )
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/pipeline_factory.py` & `taipan_di-0.0.5/taipan_di/classes/tools/pipeline_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Generic, List, TypeVar
 
 from taipan_di.classes.tools import PipelineLink
 from taipan_di.errors import TaipanRegistrationError
 
+__all__ = ["PipelineFactory"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class PipelineFactory(Generic[T, U]):
     def __init__(self) -> None:
         self._links: List[PipelineLink[T, U]] = []
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/pipeline_link.py` & `taipan_di-0.0.5/taipan_di/classes/tools/pipeline_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import abc
 from typing import Callable, Generic, TypeVar
 
+__all__ = ["PipelineLink"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class PipelineLink(Generic[T, U], metaclass=abc.ABCMeta):
     def __init__(self) -> None:
         self._next = None
-    
+
     def _set_next(self, next: "PipelineLink[T, U]") -> "PipelineLink[T, U]":
         self._next = next
         return self._next
-    
+
     def exec(self, request: T) -> U:
         next_function = self._next.exec if self._next is not None else lambda req: None
-        
+
         return self._handle(request, next_function)
 
     @abc.abstractmethod
     def _handle(self, request: T, next: Callable[[T], U]) -> U:
-        return next(request)
+        return next(request)
```

### Comparing `taipan_di-0.0.4/taipan_di/classes/tools/pipeline_registrator.py` & `taipan_di-0.0.5/taipan_di/classes/tools/pipeline_registrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from taipan_di.interfaces import BaseDependencyProvider
 
 from taipan_di.classes import instanciate_service
 
 if TYPE_CHECKING:
     from taipan_di.classes import DependencyCollection
 
+__all__ = ["PipelineRegistrator"]
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class PipelineRegistrator(Generic[T, U]):
     def __init__(
         self,
```

### Comparing `taipan_di-0.0.4/taipan_di/interfaces/base_dependency_container.py` & `taipan_di-0.0.5/taipan_di/interfaces/base_dependency_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import abc
 from typing import Type, TypeVar
 
 from .base_dependency_provider import BaseDependencyProvider
 from .base_scope import BaseScope
 
+__all__ = ["BaseDependencyContainer"]
+
 T = TypeVar("T")
 
+
 class BaseDependencyContainer(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
             hasattr(subclass, "contains")
             and callable(subclass.contains)
             and hasattr(subclass, "register")
             and callable(subclass.register)
             and hasattr(subclass, "build")
             and callable(subclass.build)
             or NotImplemented
         )
 
-    @abc.abstractmethod    
+    @abc.abstractmethod
     def contains(self, type: Type[T]) -> bool:
         raise NotImplementedError
 
-    @abc.abstractmethod    
+    @abc.abstractmethod
     def register(self, type: Type, service: BaseScope) -> None:
         raise NotImplementedError
-    
-    @abc.abstractmethod    
+
+    @abc.abstractmethod
     def build(self) -> BaseDependencyProvider:
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `taipan_di-0.0.4/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.5/taipan_di/interfaces/base_dependency_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import abc
 from typing import Type, TypeVar
 
+__all__ = ["BaseDependencyProvider"]
+
 T = TypeVar("T")
 
 
 class BaseDependencyProvider(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
@@ -23,12 +25,12 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def resolve(self, type: Type[T]) -> T:
         """
         Resolve a service along with its dependencies if it is registered in the provider.
         It it isn't, a TaipanUnregisteredError is raised.
-        
+
         Warning : Depending on how the services were registered, the instance provided might
         not be of the requested type.
         """
         raise NotImplementedError
```

### Comparing `taipan_di-0.0.4/taipan_di/interfaces/base_scope.py` & `taipan_di-0.0.5/taipan_di/interfaces/base_scope.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc
 from typing import Type, TypeVar
 
 from .base_dependency_provider import BaseDependencyProvider
 
+__all__ = ["BaseScope"]
+
 T = TypeVar("T")
 
 
 class BaseScope(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
```

### Comparing `taipan_di-0.0.4/PKG-INFO` & `taipan_di-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.4
+Version: 0.0.5
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
```

