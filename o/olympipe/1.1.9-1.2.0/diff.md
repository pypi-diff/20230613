# Comparing `tmp/olympipe-1.1.9.tar.gz` & `tmp/olympipe-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympipe-1.1.9.tar", max compression
+gzip compressed data, was "olympipe-1.2.0.tar", max compression
```

## Comparing `olympipe-1.1.9.tar` & `olympipe-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-23 20:52:54.717589 olympipe-1.1.9/LICENSE
--rw-r--r--   0        0        0     3887 2023-05-23 20:52:54.719590 olympipe-1.1.9/README.md
--rw-r--r--   0        0        0    10652 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/dispatcher.py
--rw-r--r--   0        0        0        0 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/__init__.py
--rw-r--r--   0        0        0     1718 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/batch.py
--rw-r--r--   0        0        0      530 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/explode.py
--rw-r--r--   0        0        0      524 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/filter.py
--rw-r--r--   0        0        0     2508 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/generic.py
--rw-r--r--   0        0        0     1649 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/instance.py
--rw-r--r--   0        0        0     1180 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/reduce.py
--rw-r--r--   0        0        0      408 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/task.py
--rw-r--r--   0        0        0     1899 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/pipes/timebatch.py
--rw-r--r--   0        0        0        0 2023-05-23 20:52:54.719590 olympipe-1.1.9/olympipe/py.typed
--rw-r--r--   0        0        0      646 2023-05-23 20:52:54.720589 olympipe-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-13 18:41:57.702530 olympipe-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3452 2023-06-13 18:41:57.705530 olympipe-1.2.0/README.md
+-rw-r--r--   0        0        0     8154 2023-06-13 18:41:57.705530 olympipe-1.2.0/olympipe/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:41:57.728529 olympipe-1.2.0/olympipe/pipes/__init__.py
+-rw-r--r--   0        0        0     1764 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/batch.py
+-rw-r--r--   0        0        0      660 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/explode.py
+-rw-r--r--   0        0        0      677 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/filter.py
+-rw-r--r--   0        0        0     2981 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/generic.py
+-rw-r--r--   0        0        0     1654 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/instance.py
+-rw-r--r--   0        0        0     1248 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/reduce.py
+-rw-r--r--   0        0        0      565 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/task.py
+-rw-r--r--   0        0        0     1974 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/pipes/timebatch.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:41:57.729529 olympipe-1.2.0/olympipe/py.typed
+-rw-r--r--   0        0        0      895 2023-06-13 18:41:57.706530 olympipe-1.2.0/olympipe/shuttable_queue.py
+-rw-r--r--   0        0        0      646 2023-06-13 18:41:57.706530 olympipe-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 olympipe-1.2.0/PKG-INFO
```

### Comparing `olympipe-1.1.9/LICENSE` & `olympipe-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.9/README.md` & `olympipe-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: olympipe
+Version: 1.2.0
+Summary: A powerful parallel pipelining tool
+Home-page: https://gitlab.com/gabraken/olympipe
+License: MIT
+Keywords: pipeline,multiprocessing
+Author: Gabriel Kasser
+Author-email: gabriel.kasser@gmail.com
+Requires-Python: >=3.7.2,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://gitlab.com/gabraken/olympipe
+Description-Content-Type: text/markdown
+
 # Olympipe
 
 ![coverage](https://gitlab.com/gabraken/olympipe/badges/master/coverage.svg?job=tests)![status](https://gitlab.com/gabraken/olympipe/badges/master/pipeline.svg)
 
 ![Olympipe](https://gitlab.com/gabraken/olympipe/-/raw/master/Olympipe.png)
 
 
@@ -74,31 +93,14 @@
 p = Pipeline(range(20))
 p1 = p.filter(lambda x: x % 2 == 0).debug() # Keep pair numbers
 p2 = p1.batch(2).debug() # Group in arrays of 2 elements
 
 p2.wait_for_completion()
 ```
 
-## Pipeline forking
-
-For the time being, you have to adapt the code a little bit if you wish to get several outputs for a same pipeline. [This section might be updated soon]
-
-```python
-from olympipe import Pipeline
-
-p1 = Pipeline(range(10))
-p2 = p1.filter(lambda x: x % 2 == 0)
-p3 = p1.filter(lambda x: x % 2 == 1)
-
-res2, res3 = Pipeline.wait_for_all_results([p2, p3])
-
-print(res3) # [1, 3, 5, 7, 9]
-print(res2) # [0, 2, 4, 6, 8]
-
-```
 
 ## Real time processing (for sound, video...)
 
 Use the `.temporal_batch(<seconds_float>)` pipe to aggregate packets received at this point each <seconds_float> seconds.
 
 ```python
 import time
@@ -142,8 +144,8 @@
 [res] = p2.wait_for_results()
 
 print(res) # [0, 0, 3, 6, 9]
 
 ```
 
 
-This project is still an early version, feedback is very helpful.
+This project is still an early version, feedback is very helpful.
```

### Comparing `olympipe-1.1.9/olympipe/dispatcher.py` & `olympipe-1.2.0/olympipe/pipes/generic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,104 @@
-import queue
+from multiprocessing import Process
+from queue import Empty, Full
 import time
-from multiprocessing import Process, Queue
-from threading import Timer
-from typing import Any, Generic, Iterable, List, TypeVar
+from typing import Any, Generic, Optional, Tuple, TypeVar, cast
 
-from .pipes.generic import GenericPipe
+from olympipe.shuttable_queue import ShuttableQueue
 
+R = TypeVar("R")
 S = TypeVar("S")
 
 
-class Dispatcher(Process, Generic[S]):
-    def __init__(self, queue: "Queue[S]"):
+class GenericPipe(Process, Generic[R, S]):
+    DEBUG = False
+
+    def __init__(
+        self,
+        source: "ShuttableQueue[R]",
+        target: "ShuttableQueue[S]",
+        siblings_counter: "Any",
+        count: int = 1,
+    ):
+        self.siblings_counter = siblings_counter
+        self._timeout: Optional[float] = 0.1
+        self._source_queue = source
+        self._target_queue = target
+        self._siblings_count = count
         super().__init__()
-        self._source = queue
-        self.subscribers: "List[Queue[S]]" = []
-        self._subscribers_mask: List[int] = []
-        self._death_counter: List[int] = []
-        self._timeout = 0.1
-
-        Timer(0.015, self.start).start()
-
-    def dispatch_to(self, recipients: "List[Queue[S]]", count: int = 1):
-        for recipient in recipients:
-            self.subscribers.append(recipient)
-            self._subscribers_mask.append(count)
-
-    def _dispatch(self, args: Iterable[S]):
-        for s in self.subscribers:
-            for arg in args:
-                while True:
-                    try:
-                        s.put(arg, timeout=self._timeout)
-                        break
-                    except Exception as e:
-                        if e.__class__.__name__ == "Full":
-                            continue
-                        break
-
-    def _kill(self, packet: Any) -> bool:
-        _, death_count = packet
-        self._death_counter.append(death_count)
-        if len(self._death_counter) != death_count:
-            return False
-        for s in self.subscribers:
-            while not s.empty():
-                time.sleep(0.01)
-        self._source.close()
-        for i, s in enumerate(self.subscribers):
-            num_children = self._subscribers_mask[i]
-            for _ in range(num_children):
-                s.put(GenericPipe.get_kill_word(num_children), timeout=self._timeout)
-        return True
+        self.daemon = True
+        self.start()
+
+    def get_ends(self) -> "Tuple[ShuttableQueue[R], Process, ShuttableQueue[S]]":
+        return (self._source_queue, self, self._target_queue)
+
+    def _kill(self):
+        finish_queue = False
+        with self.siblings_counter.get_lock():
+            if self.DEBUG:
+                print(self, self.siblings_counter.value)
+            self.siblings_counter.value -= 1
+            if self.siblings_counter.value == 0:
+                finish_queue = True
+
+        if finish_queue:
+            if self.DEBUG:
+                print(self, "Killing...")
+            self._close_output_queue()
+
+        try:
+            self.kill()
+        except:
+            pass
+
+    def _close_output_queue(self):
+        try:
+            # This should already be closed
+            self._source_queue.shutdown()
+        except:
+            pass
+        try:
+            time.sleep(0.1)
+            while not self._target_queue.empty():
+                time.sleep(0.1)
+            if self.DEBUG:
+                print("Close output queue")
+            self._target_queue.shutdown()
+        except Exception as e:
+            print("Failed: Could not close", e)
+
+        try:
+            self.kill()
+        except:
+            pass
+
+    def _perform_task(self, data: R) -> S:
+        return cast(S, data)
+
+    def _send_to_next(self, processed: S):
+        while True:
+            try:
+                self._target_queue.put(processed, timeout=self._timeout)
+                break
+            except TimeoutError:
+                pass
+            except Full:
+                pass
+            except Empty:
+                pass
+            except Exception as e:
+                print("Error sending:", e)
 
     def run(self):
         while True:
             try:
-                packet = self._source.get(timeout=0.1)
-                if GenericPipe.is_death_packet(packet):
-                    if self._kill(packet):
-                        return
-                    else:
-                        continue
-            except queue.Empty:
-                continue
+                data = self._source_queue.get(timeout=self._timeout)
+                processed = self._perform_task(data)
+                self._send_to_next(processed)
+            except Empty:
+                pass
             except Exception as e:
-                print("Error", e)
-                return
-            self._dispatch([packet])
+                print(f"Error_{e.__class__.__name__}_{e.args}")
+                self._source_queue.shutdown()
+                self._kill()
+            if self._source_queue.shutted and self._source_queue.empty():
+                self._kill()
```

### Comparing `olympipe-1.1.9/olympipe/pipes/batch.py` & `olympipe-1.2.0/olympipe/pipes/batch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-from multiprocessing import Queue
+from multiprocessing import Value
 import queue
-from typing import Iterable, List, Optional, TypeVar
+from typing import List, Optional, TypeVar
+
+from olympipe.shuttable_queue import ShuttableQueue
 
 from .generic import GenericPipe
 
 R = TypeVar("R")
 
 
-class BatchPipe(GenericPipe[R, Iterable[R]]):
+class BatchPipe(GenericPipe[R, List[R]]):
     def __init__(
         self,
-        source: "Queue[R]",
-        target: "Queue[Iterable[R]]",
+        source: "ShuttableQueue[R]",
+        target: "ShuttableQueue[List[R]]",
         batch_size: int,
         keep_incomplete_batch: bool,
     ):
-        super().__init__(source, target)
         self._batch_size = batch_size
         self._datas: List[R] = []
         self._keep_incomplete_batch = keep_incomplete_batch
+        sibling_counter = Value("i", 1)
+        super().__init__(source, target, sibling_counter)
 
-    def _perform_task(self, data: R) -> Optional[Iterable[R]]:  # type: ignore
+    def _perform_task(self, data: R) -> Optional[List[R]]:  # type: ignore
         self._datas.append(data)
         if len(self._datas) >= self._batch_size:
             packet, self._datas = (
                 self._datas[: self._batch_size],
                 self._datas[self._batch_size :],
             )
             return packet
 
-    def _send_to_next(self, processed: Optional[Iterable[R]]) -> None:
+    def _send_to_next(self, processed: Optional[List[R]]) -> None:
         if processed is None:
             return
         super()._send_to_next(processed)
 
     def run(self):
         while True:
             try:
-                data = self._source.get(timeout=self._timeout)
-                if GenericPipe.is_death_packet(data):
-                    if self._keep_incomplete_batch:
-                        self._send_to_next(self._datas)
-                    self._kill(data)
-                    return
+                data = self._source_queue.get(timeout=self._timeout)
                 processed = self._perform_task(data)
                 self._send_to_next(processed)
             except queue.Empty:
-                continue
+                pass
             except Exception as e:
-                self._kill(GenericPipe.get_kill_word())
                 print(f"Error_{e.__class__.__name__}_{e.args}")
+                self._kill()
+                return
+            if self._source_queue.shutted:
+                if self._keep_incomplete_batch:
+                    self._send_to_next(self._datas)
+                self._kill()
                 return
```

### Comparing `olympipe-1.1.9/olympipe/pipes/explode.py` & `olympipe-1.2.0/olympipe/pipes/explode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from multiprocessing import Queue
+from multiprocessing import Value
 from typing import Callable, Iterable, TypeVar
 
 from olympipe.pipes.task import TaskPipe
+from olympipe.shuttable_queue import ShuttableQueue
 
 R = TypeVar("R")
 S = TypeVar("S")
 
 
-__version__ = "0.1.0"
-
-
 class ExplodePipe(TaskPipe[R, S]):
     def __init__(
-        self, source: "Queue[R]", task: Callable[[R], Iterable[S]], target: "Queue[S]"
+        self,
+        source: "ShuttableQueue[R]",
+        task: Callable[[R], Iterable[S]],
+        target: "ShuttableQueue[S]",
     ):
-
-        super().__init__(source, task, target)  # type: ignore
+        sibling_counter = Value("i", 1)
+        super().__init__(source, task, target, sibling_counter, 1)  # type: ignore
 
     def _send_to_next(self, processed: Iterable[S]):  # type: ignore
         for p in processed:
             super()._send_to_next(p)
```

### Comparing `olympipe-1.1.9/olympipe/pipes/instance.py` & `olympipe-1.2.0/olympipe/pipes/instance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from multiprocessing import Queue
 from multiprocessing.managers import BaseManager
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
+from olympipe.shuttable_queue import ShuttableQueue
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 S = TypeVar("S")
 
 
 class ClassInstancePipe(GenericPipe[R, S]):
     def __init__(
         self,
-        source: "Queue[R]",
+        source: "ShuttableQueue[R]",
         constructor_class: Any,
         use_method: Callable[[Any, R], S],
-        target: "Queue[S]",
+        target: "ShuttableQueue[S]",
+        siblings_counter: Any,
+        count: int,
         close_method: Optional[Callable[[Any], Any]] = None,
         args_class: List[Any] = [],
         kwargs_class: Dict[str, Any] = {},
     ):
         BaseManager.register(constructor_class.__name__, constructor_class)
         self._constructor_class = constructor_class
         self._use_method = use_method
         self._close_method = close_method
         self._args_class = args_class
         self._kwargs_class = kwargs_class
-        self._source = source
-        self._target = target
-        super().__init__(self._source, self._target)
+        super().__init__(source, target, siblings_counter, count)
 
     def start(self) -> None:
         self._instance = self._constructor_class(
             *self._args_class, **self._kwargs_class
         )
         self._task = getattr(self._instance, self._use_method.__name__)
         if self._close_method is not None:
@@ -39,11 +40,11 @@
         else:
             self._close_method = None
         return super().start()
 
     def _perform_task(self, data: R) -> S:
         return self._task(data)
 
-    def _kill(self, data: Any, error: bool = False):
+    def _kill(self):
         if self._close_method is not None:
             self._close_method()  # type: ignore
-        super()._kill(data)
+        super()._kill()
```

### Comparing `olympipe-1.1.9/olympipe/pipes/reduce.py` & `olympipe-1.2.0/olympipe/pipes/reduce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import queue
-from multiprocessing import Queue
+from multiprocessing import Value
 from typing import Callable, TypeVar
 
+from olympipe.shuttable_queue import ShuttableQueue
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 T = TypeVar("T")
 
 
 class ReducePipe(GenericPipe[R, T]):
     def __init__(
         self,
-        source: "Queue[R]",
-        target: "Queue[T]",
+        source: "ShuttableQueue[R]",
+        target: "ShuttableQueue[T]",
         accumulator: T,
         reducer: Callable[[R, T], T],
     ):
-        super().__init__(source, target)
         self._accumulator = accumulator
         self._reduce_function = reducer
+        sibling_counter = Value("i", 1)
+        super().__init__(source, target, sibling_counter)
 
     def _perform_task(self, data: R) -> None:  # type: ignore
         self._accumulator = self._reduce_function(data, self._accumulator)
 
+    def _kill(self):
+        self._send_to_next(self._accumulator)
+        super()._kill()
+
     def run(self):
         while True:
             try:
-                data = self._source.get(timeout=self._timeout)
-                if GenericPipe.is_death_packet(data):
-                    self._send_to_next(self._accumulator)
-                    self._kill(data)
-                    return
+                data = self._source_queue.get(timeout=self._timeout)
                 self._perform_task(data)
             except queue.Empty:
-                continue
+                pass
             except Exception as e:
-                self._kill(GenericPipe.get_kill_word())
                 print(f"Error_{e.__class__.__name__}_{e.args}")
-                return
+                self._kill()
+            if self._source_queue.shutted:
+                self._kill()
```

### Comparing `olympipe-1.1.9/olympipe/pipes/timebatch.py` & `olympipe-1.2.0/olympipe/pipes/timebatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import queue
 import time
-from multiprocessing import Queue
-from typing import Iterable, List, Optional, TypeVar
+from multiprocessing import Value
+from typing import List, Optional, TypeVar
+
+from olympipe.shuttable_queue import ShuttableQueue
 
 from .generic import GenericPipe
 
 R = TypeVar("R")
 S = TypeVar("S")
 T = TypeVar("T")
 
 
-class TimeBatchPipe(GenericPipe[R, Iterable[R]]):
+class TimeBatchPipe(GenericPipe[R, List[R]]):
     def __init__(
-        self, source: "Queue[R]", target: "Queue[Iterable[R]]", interval: float
+        self,
+        source: "ShuttableQueue[R]",
+        target: "ShuttableQueue[List[R]]",
+        interval: float,
     ):
         self._interval: float = interval
         self._timeout: float = interval
         self._datas: List[R] = []
         self._last_time = time.time()
-        super().__init__(source, target)
+        sibling_counter = Value("i", 1)
+        super().__init__(source, target, sibling_counter)
 
-    def _perform_task(self, data: R) -> Optional[Iterable[R]]:  # type: ignore
+    def _perform_task(self, data: R) -> Optional[List[R]]:  # type: ignore
         elapsed = time.time() - self._last_time
         self._timeout = self._last_time + self._interval - time.time()
         if elapsed >= self._interval:
             self.increment_timeout()
             packet = self._datas[:]
             self._datas.clear()
             self._datas.append(data)
@@ -32,28 +38,27 @@
         self._datas.append(data)
         return None
 
     def increment_timeout(self):
         self._last_time += self._interval
         self._timeout += self._interval
 
-    def _send_to_next(self, processed: Iterable[R]):
+    def _send_to_next(self, processed: List[R]):
         super()._send_to_next(processed)
 
     def run(self):
         while True:
             try:
-                data = self._source.get(timeout=self._timeout)
-                if GenericPipe.is_death_packet(data):
-                    self._send_to_next(self._datas)
-                    self._datas = []
-                    self._kill(data)
-                    return
+                data = self._source_queue.get(timeout=self._timeout)
                 processed = self._perform_task(data)
                 if processed is not None:
                     self._send_to_next(processed)
             except queue.Empty:
-                continue
-            except Exception:
+                pass
+            except TimeoutError:
                 self._send_to_next(self._datas)
                 self._datas = []
+            except Exception:
                 self.increment_timeout()
+            if self._source_queue.shutted:
+                self._send_to_next(self._datas)
+                self._kill()
```

### Comparing `olympipe-1.1.9/pyproject.toml` & `olympipe-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olympipe"
-version = "1.1.9"
+version = "1.2.0"
 description = "A powerful parallel pipelining tool"
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/gabraken/olympipe"
 repository = "https://gitlab.com/gabraken/olympipe"
 authors = ["Gabriel Kasser <gabriel.kasser@gmail.com>"]
 keywords = ["pipeline", "multiprocessing"]
```

### Comparing `olympipe-1.1.9/PKG-INFO` & `olympipe-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: olympipe
-Version: 1.1.9
-Summary: A powerful parallel pipelining tool
-Home-page: https://gitlab.com/gabraken/olympipe
-License: MIT
-Keywords: pipeline,multiprocessing
-Author: Gabriel Kasser
-Author-email: gabriel.kasser@gmail.com
-Requires-Python: >=3.7.2,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://gitlab.com/gabraken/olympipe
-Description-Content-Type: text/markdown
-
 # Olympipe
 
 ![coverage](https://gitlab.com/gabraken/olympipe/badges/master/coverage.svg?job=tests)![status](https://gitlab.com/gabraken/olympipe/badges/master/pipeline.svg)
 
 ![Olympipe](https://gitlab.com/gabraken/olympipe/-/raw/master/Olympipe.png)
 
 
@@ -93,31 +74,14 @@
 p = Pipeline(range(20))
 p1 = p.filter(lambda x: x % 2 == 0).debug() # Keep pair numbers
 p2 = p1.batch(2).debug() # Group in arrays of 2 elements
 
 p2.wait_for_completion()
 ```
 
-## Pipeline forking
-
-For the time being, you have to adapt the code a little bit if you wish to get several outputs for a same pipeline. [This section might be updated soon]
-
-```python
-from olympipe import Pipeline
-
-p1 = Pipeline(range(10))
-p2 = p1.filter(lambda x: x % 2 == 0)
-p3 = p1.filter(lambda x: x % 2 == 1)
-
-res2, res3 = Pipeline.wait_for_all_results([p2, p3])
-
-print(res3) # [1, 3, 5, 7, 9]
-print(res2) # [0, 2, 4, 6, 8]
-
-```
 
 ## Real time processing (for sound, video...)
 
 Use the `.temporal_batch(<seconds_float>)` pipe to aggregate packets received at this point each <seconds_float> seconds.
 
 ```python
 import time
@@ -161,8 +125,8 @@
 [res] = p2.wait_for_results()
 
 print(res) # [0, 0, 3, 6, 9]
 
 ```
 
 
-This project is still an early version, feedback is very helpful.
+This project is still an early version, feedback is very helpful.
```

