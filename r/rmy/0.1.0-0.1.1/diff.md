# Comparing `tmp/rmy-0.1.0.tar.gz` & `tmp/rmy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmy-0.1.0.tar", max compression
+gzip compressed data, was "rmy-0.1.1.tar", max compression
```

## Comparing `rmy-0.1.0.tar` & `rmy-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1566 2023-06-11 20:31:23.956902 rmy-0.1.0/README.md
--rw-r--r--   0        0        0     1306 2023-06-12 21:31:46.731295 rmy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      393 2023-06-12 15:02:00.423365 rmy-0.1.0/rmy/__init__.py
--rw-r--r--   0        0        0      350 2023-06-11 20:31:23.957694 rmy-0.1.0/rmy/abc.py
--rw-r--r--   0        0        0     8723 2023-06-12 16:26:24.036816 rmy-0.1.0/rmy/client_async.py
--rw-r--r--   0        0        0     2999 2023-06-12 21:32:00.473539 rmy-0.1.0/rmy/client_sync.py
--rw-r--r--   0        0        0     1613 2023-06-12 15:07:40.161918 rmy-0.1.0/rmy/common.py
--rw-r--r--   0        0        0     2409 2023-06-12 14:24:18.612991 rmy-0.1.0/rmy/connection.py
--rw-r--r--   0        0        0      429 2023-06-12 14:14:59.271940 rmy-0.1.0/rmy/pubsub.py
--rw-r--r--   0        0        0     8264 2023-06-12 15:07:52.346068 rmy-0.1.0/rmy/server.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 rmy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      824 2023-06-13 20:55:51.596825 rmy-0.1.1/README.md
+-rw-r--r--   0        0        0     1306 2023-06-13 20:58:00.585595 rmy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-13 20:28:42.319559 rmy-0.1.1/rmy/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-11 20:31:23.957694 rmy-0.1.1/rmy/abc.py
+-rw-r--r--   0        0        0     8790 2023-06-13 20:16:31.807840 rmy-0.1.1/rmy/client_async.py
+-rw-r--r--   0        0        0     2973 2023-06-13 20:14:14.297858 rmy-0.1.1/rmy/client_sync.py
+-rw-r--r--   0        0        0     1604 2023-06-13 11:34:38.724113 rmy-0.1.1/rmy/common.py
+-rw-r--r--   0        0        0     2410 2023-06-13 09:29:04.848659 rmy-0.1.1/rmy/connection.py
+-rw-r--r--   0        0        0      429 2023-06-12 14:14:59.271940 rmy-0.1.1/rmy/pubsub.py
+-rw-r--r--   0        0        0     8339 2023-06-13 20:28:06.769688 rmy-0.1.1/rmy/server.py
+-rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 rmy-0.1.1/PKG-INFO
```

### Comparing `rmy-0.1.0/LICENSE` & `rmy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rmy-0.1.0/pyproject.toml` & `rmy-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 ignore_errors = true
 
 
 [tool.coverage.run]
 source = "rmy/*"
 [tool.poetry]
 name = "rmy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Stateful rpc for Python"
 authors = ["fdv1 <francois@pytek.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4.0"
-anyio = "^3.6.2"
+anyio = "^3.7.0"
 janus = "^1.0.0"
 asyncstdlib = "^3.10.7"
 mpmc = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 mypy = "^1.3.0"
```

### Comparing `rmy-0.1.0/rmy/client_async.py` & `rmy-0.1.1/rmy/client_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from itertools import count
 from typing import Any, AsyncIterator, Callable, Optional
 
 import anyio
 from anyio.abc import TaskStatus
 
 from .abc import Connection
-from .common import UserException, closing_scope, scoped_execute_coroutine, scoped_insert
+from .common import UserException, cancel_task_on_exit, closing_scope, scoped_insert
 from .connection import connect_to_tcp_server
 
 
 OK = "OK"
 CLOSE_SENTINEL = "Close sentinel"
 CLOSE_STREAM = "Close stream"
 CANCELLED_TASK = "Cancelled task"
@@ -39,15 +39,15 @@
         self.object_id = object_id
         self.function = function
         self.args = args
         self.kwargs = kwargs
 
     def __await__(self):
         return asyncio.create_task(
-            self.client.send_request(
+            self.client.execute_request(
                 AWAITABLE,
                 (self.object_id, self.function, self.args, self.kwargs),
                 is_cancellable=True,
                 include_code=False,
             )
         ).__await__()
 
@@ -112,90 +112,92 @@
             elif code == ITER_ASYNC_ITERATOR:
                 sink = self.async_generators_streams.get(message_id)
                 if sink:
                     try:
                         sink.send_nowait((status, result))
                     except anyio.WouldBlock as e:
                         sink.close()
+            elif code == CANCELLED_TASK:
+                print("Task cancelled.", message_id, status, result)
             else:
                 print(f"Unexpected code {code} received.")
 
     @contextlib.contextmanager
-    def create_request(self, code, args, is_cancellable=False):
+    def submit_request(self, code, args, is_cancellable=False):
         request_id = next(self.request_id)
         future = asyncio.Future()
         with scoped_insert(self.pending_requests, request_id, future):
             self.send_nowait(code, request_id, args)
             try:
                 yield future
             except anyio.get_cancelled_exc_class():
                 if is_cancellable:
-                    with anyio.CancelScope(shield=True):
-                        self.send_nowait(code, request_id, None)
+                    self.cancel_task(request_id)
                 raise
 
-    async def send_request(self, code, args, is_cancellable=False, include_code=True) -> Any:
-        with self.create_request(code, args, is_cancellable) as future:
+    async def execute_request(self, code, args, is_cancellable=False, include_code=True) -> Any:
+        with self.submit_request(code, args, is_cancellable) as future:
             return decode_result(*(await future), include_code=include_code)
 
     async def get_attribute(self, object_id: int, name: str):
-        return await self.send_request(GET_ATTRIBUTE, (object_id, name), include_code=False)
+        return await self.execute_request(GET_ATTRIBUTE, (object_id, name), include_code=False)
 
     def remote_method(self, object_id: int, function: Callable, *args, **kwargs) -> Any:
         return Result(self, object_id, function, args, kwargs)
 
+    def cancel_task(self, request_id: int):
+        self.send_nowait(CANCELLED_TASK, request_id, None)
+        self.pending_requests.pop(request_id, None)
+
     async def evaluate_async_generator(self, object_id, function, args, kwargs):
-        iterator_id = await self.send_request(
+        iterator_id = await self.execute_request(
             FUNCTION,
             (object_id, function, args, kwargs),
             is_cancellable=True,
             include_code=False,
         )
         async for value in self.iter_async_generator(iterator_id):
             yield value
 
     async def iter_async_generator(self, iterator_id: int):
         sink, stream = anyio.create_memory_object_stream(STREAM_BUFFER_SIZE)
-        stream_id = next(self.request_id)
-        with scoped_insert(self.async_generators_streams, stream_id, sink):
-            await self.send(ITER_ASYNC_ITERATOR, stream_id, iterator_id)
+        request_id = next(self.request_id)
+        with scoped_insert(self.async_generators_streams, request_id, sink):
+            await self.send(ITER_ASYNC_ITERATOR, request_id, iterator_id)
             try:
                 async for code, value in stream:
                     if code == OK:
                         yield value
                     elif code in (CLOSE_SENTINEL, CANCELLED_TASK):
                         break
                     elif code == USER_EXCEPTION:
                         raise UserException(value)
                     else:
                         raise Exception(value)
-            except Exception as e:
-                print(e)
             finally:
-                with anyio.CancelScope(shield=True):
-                    await self.send(ASYNC_ITERATOR, stream_id, None)
+                self.cancel_task(request_id)
 
     @contextlib.asynccontextmanager
     async def create_remote_object(
         self, object_class, args=(), kwarg={}, sync_client: Optional["SyncClient"] = None
     ):
-        object_id = await self.send_request(
+        object_id = await self.execute_request(
             CREATE_OBJECT, (object_class, args, kwarg), include_code=False
         )
         try:
             yield await self.fetch_remote_object(object_id, sync_client)
         finally:
             with anyio.CancelScope(shield=True):
                 await self.send(DELETE_OBJECT, 0, object_id)
 
     async def fetch_remote_object(
         self, object_id: int = SERVER_OBJECT_ID, sync_client: Optional["SyncClient"] = None
     ) -> Any:
         if object_id not in self.remote_objects:
-            object_class = await self.send_request(FETCH_OBJECT, object_id, include_code=False)
+            object_class = await self.execute_request(FETCH_OBJECT, object_id, include_code=False)
             __getattr__ = partial(self.get_attribute, object_id)
             if sync_client:
                 __getattr__ = sync_client.wrap_awaitable(__getattr__)
             object_class = type(
                 f"{object_class.__name__}Proxy",
                 (RemoteObject, object_class),
                 {"__getattr__": __getattr__},
@@ -214,15 +216,15 @@
             self.remote_objects[object_id] = remote_object
         return self.remote_objects[object_id]
 
 
 @contextlib.asynccontextmanager
 async def _create_async_client(task_group, connection: Connection) -> AsyncIterator[AsyncClient]:
     with closing_scope(AsyncClient(task_group, connection)) as client:
-        with scoped_execute_coroutine(client.process_messages_from_server()):
+        with cancel_task_on_exit(client.process_messages_from_server()):
             yield client
 
 
 @contextlib.asynccontextmanager
 async def connect(host_name: str, port: int) -> AsyncIterator[AsyncClient]:
     async with anyio.create_task_group() as task_group:
         async with connect_to_tcp_server(host_name, port) as connection:
```

### Comparing `rmy-0.1.0/rmy/client_sync.py` & `rmy-0.1.1/rmy/client_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import asyncio
 import contextlib
 from typing import Iterator
 
 import anyio
 import janus
 
-from rmy import CLOSE_STREAM, EXCEPTION, OK
-
 from .client_async import (
     ASYNC_ITERATOR,
     AWAITABLE,
+    CLOSE_STREAM,
+    EXCEPTION,
     FUNCTION,
+    OK,
     SERVER_OBJECT_ID,
     AsyncClient,
     connect,
 )
-from .common import scoped_execute_coroutine
+from .common import cancel_task_on_exit
 
 
 class SyncClient:
     def __init__(self, portal, async_client) -> None:
         self.portal = portal
         self.async_client: AsyncClient = async_client
 
@@ -45,27 +45,27 @@
                     queue.close()
                     break
                 if code is EXCEPTION:
                     queue.close()
                     raise message
                 yield message
 
-        with scoped_execute_coroutine(forward_to_main_thread()):
+        with cancel_task_on_exit(forward_to_main_thread()):
             yield result_sync_iterator()
 
     def sync_generator(self, iterator_id: int):
         with self.portal.wrap_async_context_manager(
             self.remote_async_iterate(iterator_id)
         ) as sync_iterator:
             yield from sync_iterator
 
     def wrap_function(self, object_id, function):
         def result(*args, **kwargs):
             code, result = self.portal.call(
-                self.async_client.send_request, FUNCTION, (object_id, function, args, kwargs)
+                self.async_client.execute_request, FUNCTION, (object_id, function, args, kwargs)
             )
             if code == AWAITABLE:
                 return result
             elif code == ASYNC_ITERATOR:
                 return self.sync_generator(result)
 
         return result
```

### Comparing `rmy-0.1.0/rmy/common.py` & `rmy-0.1.1/rmy/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,36 +36,38 @@
         iterable.close()
 
 
 closing_scope = scoped_iter
 
 
 @contextlib.contextmanager
-def scoped_execute_coroutine(coroutine: Coroutine):
+def cancel_task_on_exit(coroutine: Coroutine):
     task = asyncio.create_task(coroutine)
     try:
         yield task
     finally:
         task.cancel()
 
+
 @contextlib.asynccontextmanager
-async def scoped_execute_coroutine_new(method, *args, **kwargs):
+async def execute_cancellable_coroutine(method, *args, **kwargs):
     async with anyio.create_task_group() as task_group:
         task_group.start_soon(method, *args, **kwargs)
-        yield task_group.cancel_scope.cancel
-
-
-class UserException(Exception):
-    """Use this to signal expected errors to users."""
+        yield task_group.cancel_scope
 
-    pass
 
 async def cancel_task_group_on_signal(task_group: anyio.abc.TaskGroup):
     with anyio.open_signal_receiver(signal.SIGINT, signal.SIGTERM) as signals:
         async for signum in signals:
             if signum == signal.SIGINT:
                 print("Ctrl+C pressed!")
             else:
                 print(f"Received signal {signum}, terminating.")
 
             task_group.cancel_scope.cancel()
             return
+
+
+class UserException(Exception):
+    """Use this to signal expected errors to users."""
+
+    pass
```

### Comparing `rmy-0.1.0/rmy/connection.py` & `rmy-0.1.1/rmy/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import contextlib
 import struct
 from asyncio.streams import StreamReader, StreamWriter, open_connection
 import sys
+
 if sys.version_info < (3, 8):
     from asyncio.streams import IncompleteReadError
 else:
     from asyncio.exceptions import IncompleteReadError
 from pickle import dumps, loads
 from typing import Any, Tuple, Callable
```

### Comparing `rmy-0.1.0/rmy/server.py` & `rmy-0.1.1/rmy/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     ITER_ASYNC_ITERATOR,
     OK,
     USER_EXCEPTION,
 )
 from .common import (
     UserException,
     cancel_task_group_on_signal,
+    cancel_task_on_exit,
+    execute_cancellable_coroutine,
     print_error_stack,
-    scoped_execute_coroutine,
-    scoped_execute_coroutine_new,
     scoped_insert,
 )
 from .connection import TCPConnection
 
 
 class ClientSession:
     def __init__(self, server, task_group, connection: Connection) -> None:
@@ -72,15 +72,15 @@
             raise
         finally:
             with anyio.CancelScope(shield=True):
                 await self.send(task_type, request_id, code, result)
 
     async def run_task(self, request_id, task_type, coroutine_or_async_context):
         try:
-            async with scoped_execute_coroutine_new(
+            async with execute_cancellable_coroutine(
                 self.evaluate_coroutine_or_async_generator,
                 request_id,
                 task_type,
                 coroutine_or_async_context,
             ) as self.running_tasks[request_id]:
                 pass
         finally:
@@ -110,38 +110,40 @@
         try:
             value = getattr(self.session_manager.objects[object_id], name)
             await self.send(GET_ATTRIBUTE, request_id, OK, value)
         except Exception as e:
             code, message = EXCEPTION, e
         await self.send(GET_ATTRIBUTE, request_id, code, message)
 
+    async def cancel_running_task(self, request_id: int):
+        running_task = self.running_tasks.get(request_id)
+        if running_task:
+            running_task.cancel()
+            await running_task
+
     async def process_messages(self):
         async for code, request_id, payload in self.connection:
             try:
-                if code in (FUNCTION, AWAITABLE, ASYNC_ITERATOR):
-                    if payload is None:
-                        running_task = self.running_tasks.get(request_id)
-                        if running_task:
-                            running_task()
-                            await running_task
-                    else:
-                        object_id, function, args, kwargs = payload
-                        coroutine_or_async_context = function(
-                            self.session_manager.objects[object_id], *args, **kwargs
+                if code in (FUNCTION, AWAITABLE):
+                    object_id, function, args, kwargs = payload
+                    coroutine_or_async_context = function(
+                        self.session_manager.objects[object_id], *args, **kwargs
+                    )
+                    if code != FUNCTION or asyncio.iscoroutine(coroutine_or_async_context):
+                        self.task_group.start_soon(
+                            self.run_task,
+                            request_id,
+                            code,
+                            coroutine_or_async_context,
                         )
-                        if code != FUNCTION or asyncio.iscoroutine(coroutine_or_async_context):
-                            self.task_group.start_soon(
-                                self.run_task,
-                                request_id,
-                                code,
-                                coroutine_or_async_context,
-                            )
-                        else:
-                            self.pending_async_generators[request_id] = coroutine_or_async_context
-                            await self.send(code, request_id, ASYNC_ITERATOR, request_id)
+                    else:
+                        self.pending_async_generators[request_id] = coroutine_or_async_context
+                        await self.send(code, request_id, ASYNC_ITERATOR, request_id)
+                elif code == CANCELLED_TASK:
+                    await self.cancel_running_task(request_id)
                 elif code == ITER_ASYNC_ITERATOR:
                     self.task_group.start_soon(
                         self.run_task,
                         request_id,
                         code,
                         self.pending_async_generators.pop(payload),
                     )
@@ -205,7 +207,11 @@
     async with anyio.create_task_group() as task_group:
         task_group.start_soon(cancel_task_group_on_signal, task_group)
         task_group.start_soon(main, *args, **kwargs)
 
 
 async def start_tcp_server(port: int, server_object: Any):
     await handle_signals(_serve_tcp, port, server_object)
+
+
+def run_tcp_server(port: int, server_object: Any):
+    anyio.run(start_tcp_server, port, server_object)
```

