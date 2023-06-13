# Comparing `tmp/lk_utils-2.5.5-py3-none-any.whl.zip` & `tmp/lk_utils-2.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15792 bytes, number of entries: 16
+Zip file size: 15830 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     1258 b- defN 80-Jan-01 00:00 lk_utils/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 80-Jan-01 00:00 lk_utils/__main__.py
 -rw-r--r--  2.0 unx      141 b- defN 80-Jan-01 00:00 lk_utils/filesniff/__init__.py
 -rw-r--r--  2.0 unx     7001 b- defN 80-Jan-01 00:00 lk_utils/filesniff/finder.py
--rw-r--r--  2.0 unx     5576 b- defN 80-Jan-01 00:00 lk_utils/filesniff/main.py
+-rw-r--r--  2.0 unx     6041 b- defN 80-Jan-01 00:00 lk_utils/filesniff/main.py
 -rw-r--r--  2.0 unx     3357 b- defN 80-Jan-01 00:00 lk_utils/filesniff/shutil.py
 -rw-r--r--  2.0 unx      582 b- defN 80-Jan-01 00:00 lk_utils/filesniff/traceback.py
--rw-r--r--  2.0 unx     5968 b- defN 80-Jan-01 00:00 lk_utils/read_and_write.py
+-rw-r--r--  2.0 unx     6053 b- defN 80-Jan-01 00:00 lk_utils/read_and_write.py
 -rw-r--r--  2.0 unx      377 b- defN 80-Jan-01 00:00 lk_utils/subproc/__init__.py
 -rw-r--r--  2.0 unx     1797 b- defN 80-Jan-01 00:00 lk_utils/subproc/promise.py
--rw-r--r--  2.0 unx     3384 b- defN 80-Jan-01 00:00 lk_utils/subproc/subprocess.py
+-rw-r--r--  2.0 unx     3450 b- defN 80-Jan-01 00:00 lk_utils/subproc/subprocess.py
 -rw-r--r--  2.0 unx     7972 b- defN 80-Jan-01 00:00 lk_utils/subproc/threading.py
 -rw-r--r--  2.0 unx     1556 b- defN 80-Jan-01 00:00 lk_utils/time_utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_utils-2.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx     4234 b- defN 80-Jan-01 00:00 lk_utils-2.5.5.dist-info/METADATA
-?rw-r--r--  2.0 unx     1291 b- defN 16-Jan-01 00:00 lk_utils-2.5.5.dist-info/RECORD
-16 files, 45429 bytes uncompressed, 13676 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     3723 b- defN 80-Jan-01 00:00 lk_utils-2.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_utils-2.5.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1291 b- defN 16-Jan-01 00:00 lk_utils-2.5.6.dist-info/RECORD
+16 files, 45534 bytes uncompressed, 13714 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -33,17 +33,17 @@
 
 Filename: lk_utils/subproc/threading.py
 Comment: 
 
 Filename: lk_utils/time_utils.py
 Comment: 
 
-Filename: lk_utils-2.5.5.dist-info/WHEEL
+Filename: lk_utils-2.5.6.dist-info/METADATA
 Comment: 
 
-Filename: lk_utils-2.5.5.dist-info/METADATA
+Filename: lk_utils-2.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: lk_utils-2.5.5.dist-info/RECORD
+Filename: lk_utils-2.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_utils/__init__.py

```diff
@@ -33,8 +33,8 @@
 from .read_and_write import ropen
 from .read_and_write import wopen
 from .subproc import new_thread
 from .subproc import run_cmd_args
 from .subproc import run_cmd_shell
 from .subproc import run_new_thread
 
-__version__ = '2.5.5'
+__version__ = '2.5.6'
```

## lk_utils/filesniff/main.py

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import os
 import os.path as ospath
+from functools import partial
 from inspect import currentframe
 
 __all__ = [
+    'abspath',
     'basename',
     'dirname',
     'dirpath',
     'filename',
     'filepath',
     'get_current_dir',
     'isdir',
@@ -17,14 +19,15 @@
     'isfilelike',
     'islink',
     'normpath',
     'not_empty',
     'parent',
     'parent_path',
     'relpath',
+    'split',
     'xpath'
 ]
 
 _IS_WINDOWS = os.name == 'nt'
 
 
 class T:
@@ -37,14 +40,17 @@
     else:
         out = ospath.normpath(path)
     if _IS_WINDOWS:
         out = out.replace('\\', '/')
     return out
 
 
+abspath = partial(normpath, force_abspath=True)
+
+
 # ------------------------------------------------------------------------------
 
 def parent_path(path: T.Path) -> T.DirPath:
     return normpath(ospath.dirname(path))
 
 
 parent = parent_path  # alias
@@ -198,14 +204,28 @@
     
     if force_abspath:
         return normpath(out)
     else:
         return normpath(ospath.relpath(out, os.getcwd()))
 
 
+def split(path: T.Path, parts=2) -> tuple[str, ...]:
+    path = abspath(path)
+    if parts == 2:
+        a, b = path.rsplit('/', 1)
+        return a, b
+    elif parts == 3:
+        assert isfile(path)
+        a, b = path.rsplit('/', 1)
+        b, c = b.rsplit('.', 1)
+        return a, b, c
+    else:
+        raise ValueError('Unsupported parts number!')
+
+
 def _get_dir_of_frame(frame, ignore_error=False) -> T.Path:
     file = frame.f_globals.get('__file__') \
            or frame.f_code.co_filename
     if file.startswith('<') and file.endswith('>'):
         if ignore_error:
             print(':v4p2', 'Unable to locate directory from caller frame! '
                            'Fallback using current working directory instead.')
```

## lk_utils/read_and_write.py

```diff
@@ -123,15 +123,19 @@
             #   default=str
             #       when something is not serializble, callback `__str__`.
             #       it is useful to resolve `pathlib.PosixPath`.
     
     elif ftype == 'yaml':  # pip install pyyaml
         from yaml import dump as ydump  # noqa
         with wopen(file) as f:
-            ydump(data, f, **{'sort_keys': False, **kwargs})
+            ydump(data, f, **{
+                'allow_unicode': True,
+                'sort_keys': False,
+                **kwargs
+            })
     
     elif ftype == 'pickle':
         from pickle import dump as pdump
         with wopen(file, 'wb') as f:
             pdump(data, f, **kwargs)
     
     elif ftype == 'toml':  # pip install toml
```

## lk_utils/subproc/__init__.py

```diff
@@ -1,11 +1,11 @@
 from . import subprocess
 from .promise import Promise
 from .promise import defer
 from .subprocess import compose_cmd
 from .subprocess import run_cmd_args
 from .subprocess import run_cmd_shell
-from .threading import ThreadWorker
+from .threading import ThreadBroker
 from .threading import new_thread
 from .threading import retrieve_thread
 from .threading import run_new_thread
 from .threading import thread_manager
```

## lk_utils/subproc/promise.py

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from .threading import ThreadWorker as Thread
+from .threading import ThreadBroker as Thread
 
 
 def defer(func: t.Callable, *args, **kwargs) -> 'Promise':
     """
     args:
         kwargs:
             self used keys:
```

## lk_utils/subproc/subprocess.py

```diff
@@ -30,15 +30,15 @@
             if a or not filter_:
                 out.append(a)
     return out
 
 
 def run_command_args(
         *args: t.Any, verbose=False,
-        ignore_error=False, filter_=True,
+        ignore_error=False, filter_=True, shell=False,
         _refmt_args=True
 ) -> str:
     """
     https://stackoverflow.com/questions/58302588/how-to-both-capture-shell
     -command-output-and-show-it-in-terminal-at-realtime
     
     args:
@@ -46,18 +46,18 @@
     """
     if _refmt_args:
         args = compose_command(*args, filter_=filter_)
     # else:
     #     assert all(isinstance(x, str) for x in args)
     
     if not verbose:
-        sub_run(args, check=not ignore_error)
+        sub_run(args, check=not ignore_error, shell=shell)
         return ''
     
-    proc = Popen(args, stdout=PIPE, stderr=PIPE, text=True)
+    proc = Popen(args, stdout=PIPE, stderr=PIPE, text=True, shell=shell)
     
     out, err = '', ''
     for line in proc.stdout:
         print(':psr', '[dim]{}[/]'.format(
             line.rstrip().replace('[', '\\[')))
         out += line
     for line in proc.stderr:
@@ -73,19 +73,19 @@
                 raise E.SubprocessError(proc.args, err, code)
     
     return out or err
 
 
 def run_command_shell(
         cmd: str, verbose=False,
-        ignore_error=False, filter_=False
+        ignore_error=False, filter_=False, shell=False,
 ) -> str:
     return run_command_args(
         *shlex.split(cmd), verbose=verbose,
-        ignore_error=ignore_error, filter_=filter_,
+        ignore_error=ignore_error, filter_=filter_, shell=shell,
         _refmt_args=False
     )
 
 
 class E:
     class SubprocessError(Exception):
         def __init__(
```

## lk_utils/subproc/threading.py

```diff
@@ -8,27 +8,27 @@
 from types import GeneratorType
 
 
 class T:
     Group = str  # the default group is 'default'
     Id = t.Union[str, int]
     
-    # ThreadWorker
+    # ThreadBroker
     Target = t.Callable
     Args = t.Optional[tuple]
     KwArgs = t.Optional[dict]
     _Inherit = bool
     Task = t.Tuple[Target, Args, KwArgs, _Inherit]
     
     # ThreadPool
-    ThreadWorker = t.ForwardRef('ThreadWorker')
-    ThreadPool = t.Dict[Group, t.Dict[Id, ThreadWorker]]
+    ThreadBroker = t.ForwardRef('ThreadBroker')
+    ThreadPool = t.Dict[Group, t.Dict[Id, ThreadBroker]]
 
 
-class ThreadWorker:
+class ThreadBroker:
     _daemon: bool
     _illed: t.Optional[Exception]
     _interruptible: bool
     _is_executed: bool
     _is_running: bool
     _result: t.Any
     _target: T.Target
@@ -49,15 +49,15 @@
     ):
         self._tasks = deque()
         self._tasks.append((target, args, kwargs, False))
         self._daemon = daemon
         self._interruptible = interruptible
         self._is_executed = False
         self._is_running = False
-        self._result = ThreadWorker.Undefined
+        self._result = ThreadBroker.Undefined
         self._target = target
         if start_now:
             self.mainloop()
 
     # -------------------------------------------------------------------------
     
     @property
@@ -74,15 +74,15 @@
     
     # @property
     # def is_alive(self) -> bool:
     #     return self._thread.is_alive()
     
     @property
     def result(self) -> t.Any:
-        if self._result is ThreadWorker.Undefined:
+        if self._result is ThreadBroker.Undefined:
             raise RuntimeError('The result is not ready yet.')
         return self._result
 
     # -------------------------------------------------------------------------
     
     def start(self) -> None:
         if self._is_running:
@@ -176,76 +176,76 @@
         
         def decorator(func: T.Target):
             nonlocal ident
             if ident is None:
                 ident = id(func)
             
             @wraps(func)
-            def wrapper(*args, **kwargs) -> ThreadWorker:
-                return self._create_thread_worker(
+            def wrapper(*args, **kwargs) -> ThreadBroker:
+                return self._create_thread_broker(
                     group, ident, func, args,
                     kwargs, daemon, singleton, interruptible
                 )
             
             return wrapper
         
         return decorator
     
     def run_new_thread(
             self, target: T.Target,
             args=None, kwargs=None,
             daemon=True, interruptible=False
-    ) -> ThreadWorker:
+    ) -> ThreadBroker:
         """ run function in a new thread at once. """
         # # assert id(target) not in __thread_pool  # should i check it?
-        return self._create_thread_worker(
+        return self._create_thread_broker(
             'default', id(target), target,
             args, kwargs, daemon, False, interruptible
         )
     
-    def _create_thread_worker(
+    def _create_thread_broker(
             self, group: T.Group, ident: T.Id, target: T.Target,
             args=None, kwargs=None,
             daemon=True, singleton=False, interruptible=False
-    ) -> ThreadWorker:
+    ) -> ThreadBroker:
         if singleton:
             if t := self.thread_pool[group].get(ident):
                 t.add_task(args, kwargs)
                 return t
-        worker = self.thread_pool[group][ident] = ThreadWorker(
+        broker = self.thread_pool[group][ident] = ThreadBroker(
             target=target, args=args, kwargs=kwargs, daemon=daemon,
             interruptible=interruptible
         )
-        return worker
+        return broker
     
     # -------------------------------------------------------------------------
     
     class Delegate:
         
-        def __init__(self, *threads: ThreadWorker):
+        def __init__(self, *threads: ThreadBroker):
             self.threads = threads
         
         def __len__(self):
             return len(self.threads)
         
-        def fetch_one(self, index=0) -> t.Optional[ThreadWorker]:
+        def fetch_one(self, index=0) -> t.Optional[ThreadBroker]:
             if self.threads:
                 return self.threads[index]
             else:
                 return None
         
         def join_all(self):
             for t in self.threads:
                 t.join()
     
     def retrieve_thread(
             self,
             ident: T.Id,
             group: T.Group = 'default'
-    ) -> ThreadWorker | None:
+    ) -> ThreadBroker | None:
         return self.thread_pool[group].get(ident)
     
     def retrieve_threads(
             self,
             group: T.Group = 'default'
     ) -> 'ThreadManager.Delegate':
         return ThreadManager.Delegate(*self.thread_pool[group].values())
```

## Comparing `lk_utils-2.5.5.dist-info/METADATA` & `lk_utils-2.5.6.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,128 @@
 Metadata-Version: 2.1
 Name: lk-utils
-Version: 2.5.5
+Version: 2.5.6
 Summary: LK Utils is a set of utility wrappers made for data processing.
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argsense
-Requires-Dist: lk-logger (>=5.4.8,<6.0.0)
+Requires-Dist: lk-logger (>=5.6.1,<6.0.0)
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # LK Utils
 
-lk-utils is a set of utility wrappers to make data processing more simple and fluent.
+lk-utils is a set of utilities to make data processing more simple and fluent.
 
 # Install
 
 ```shell
 pip install lk-utils
 ```
 
-the default pip install doesn't include extra dependencies. to get extra support for excel or nlp processing, pip install this:
-
-```shell
-pip install lk-utils  # to add lk-logger (required dependency)
-pip install lk-utils[exl]  # to add lk-logger, xlrd, xlsxwriter
-pip install lk-utils[nlp]  # to add lk-logger, pypinyin
-pip install lk-utils[all]  # to add all of the above
-```
-
-lk-utils requires Python 3.8 or higher version.
+lk-utils requires python 3.8 or higher version.
 
 # Usage
 
 ## subproc
 
 ### new thread decorator
 
 ```python
-from lk_utils.subproc import new_thread
+from lk_utils import new_thread
+
 
-@new_thread(daemon=True, singleton=False)
-def background_loop():
-    from time import sleep
-    i = 0
-    while i < 10:
-        i += 1
-        print(i)
-        sleep(1)
+def main(files: list[str]) -> None:
+    for f in files:
+        handle_file(f)
 
-x = background_loop()
-print(type(x))  # -> threading.Thread
+
+@new_thread()
+def handle_file(file: str) -> None:
+    # do something
+    ...
 ```
 
-### run in new thread
+### fetch results from threads
 
 ```python
-from lk_utils.subproc import run_new_thread
+from lk_utils import new_thread
+
 
-def background_loop():
-    from time import sleep
-    i = 0
-    while i < 10:
-        i += 1
-        print(i)
-        sleep(1)
+def main(files: list[str]) -> None:
+    pool = []
+    for f in files:
+        thread = handle_file(f)
+        pool.append(thread)
+    
+    ...
+    
+    for thread in pool:
+        result = thread.join()
+        print(result)
 
-x = run_new_thread(background_loop, args=None, kwargs=None, daemon=True)
-print(type(x))  # -> threading.Thread
+
+@new_thread()
+def handle_file(file: str) -> str:
+    # do something
+    ...
 ```
 
 ### run cmd args
 
 ```python
-from lk_utils.subproc import run_cmd_shell, run_cmd_args
-run_cmd_shell('python -m pip list')
+from lk_utils import run_cmd_args
+from lk_utils import run_cmd_shell
 run_cmd_args('python', '-m', 'pip', 'list')
+run_cmd_shell('python -m pip list')
 ```
 
-### mklink, mklinks
+advanced filter:
 
 ```python
-"""
-example structure:
-    |= from_dir
-       |= folder_xxx
-       |- file_xxx.txt
-    |= to_dir_1    # empty
-    |= to_dir_2    # not empty
-       |- ...
-"""
+from lk_utils import run_cmd_args
+
+
+def pip_install(
+        dest: str, 
+        url_index: str = None
+) -> None:
+    run_cmd_args(
+        ('python', '-m', 'pip'),
+        ('install', '-r', 'requirements.txt'),
+        ('-t', dest),
+        ('-i', url_index),
+    )
+```
 
-from lk_utils.subproc import mklink, mklinks
+### mklink, mklinks
+
+```python
+from lk_utils import mklink, mklinks
 mklink('/from_dir', '/to_dir_1')
 mklinks('/from_dir', '/to_dir_2')
-
-"""
-result:
-    |= from_dir
-       |= folder_xxx
-       |- file_xxx.txt
-    |= to_dir_1         # this is a symlink
-    |= to_dir_2
-       |- ...
-       |= folder_xxx    # this is a symlink
-       |- file_xxx.txt  # this is a symlink
-"""
 ```
 
 ## filesniff
 
 ### get current dir, get relative path
 
 ```python
 import os
 from lk_utils import filesniff as fs
-print(fs.currdir()
-      == os.path.dirname(__file__)).replace('\\', '/'))  # -> True
-print(fs.relpath('..')
-      == os.path.dirname(fs.currdir()))  # -> True
+print(fs.currdir() == os.path.dirname(__file__).replace('\\', '/'))  # -> True
+print(fs.relpath('..') == os.path.dirname(fs.currdir()))  # -> True
 ```
 
 ### list files/dirs
 
 ```python
 from lk_utils import filesniff as fs
```

## Comparing `lk_utils-2.5.5.dist-info/RECORD` & `lk_utils-2.5.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-lk_utils/__init__.py,sha256=0ymVbWIpMFlQu9OQ70aQo2IqXPGvkjJbAlRMrhbT3ok,1258
+lk_utils/__init__.py,sha256=LNcphcZ6W4JBV1freedPEgk9Tq5ze3FknQzcHcWXqAg,1258
 lk_utils/__main__.py,sha256=KA4dDZb-xAV20iKRTg_YijCSOGepJG_j8h0O6VMYuu8,847
 lk_utils/filesniff/__init__.py,sha256=rtggL_f0-XRZga_t8jWg8sbIwDFsJUIYz-PFcHE0daM,141
 lk_utils/filesniff/finder.py,sha256=gIzdtA9TblUVKBNKWiFcnJBdHGiI5A-2oq7g1g_8qH0,7001
-lk_utils/filesniff/main.py,sha256=jmWR_tnwCkFNxPBFHHZbaKHwXaDLX7Kn-q2_Q5xYj5E,5576
+lk_utils/filesniff/main.py,sha256=-8r0quml53RFYZS1DgRkBb7fd-6uPNZXPv3hsgEQAiM,6041
 lk_utils/filesniff/shutil.py,sha256=f5SVZU2mkX5uUu1cMxpBfT-IqFr1OYugKc5CHWH1oAQ,3357
 lk_utils/filesniff/traceback.py,sha256=SoJjnT2ArSrgR3NGOtQ_awCyMQga-e7W6ij7jp0zfdA,582
-lk_utils/read_and_write.py,sha256=zUpP8qZVCuL6rHZQhghOWmPiKb9In3Nqcwwny9yIKTU,5968
-lk_utils/subproc/__init__.py,sha256=wRQpAbhJ9oorKIuHVINZSgfV0pvjF5cZGAUNKCMH0vg,377
-lk_utils/subproc/promise.py,sha256=bqxlreFnSo6MCI4AdkSjxj3HpxoQRw94QsLpdox8QKU,1797
-lk_utils/subproc/subprocess.py,sha256=P-vBKdl5hQvTk7IQY8VoM0yslZQBhBh5WsYRBObhQU0,3384
-lk_utils/subproc/threading.py,sha256=rV2m6_FA6tqfIG22o3g9LlIXCUt8Jv2G9Ew0iW9-oh0,7972
+lk_utils/read_and_write.py,sha256=xbKRZemRisEn8-p36z48KI-B5CvaAr62Tm9Qt3c6qhs,6053
+lk_utils/subproc/__init__.py,sha256=nqV63W57QOvr5MINE43Get06ChOl0_eq1xvmlq3n4wg,377
+lk_utils/subproc/promise.py,sha256=5ZXiaYal19EewJVaoE22dnhEuM9ZtHM_7cdRsdq61l8,1797
+lk_utils/subproc/subprocess.py,sha256=gkx00beQerE0bUsPDsofY3zH4OskGsblYD5y8nb-4Fo,3450
+lk_utils/subproc/threading.py,sha256=e7_n-hxbG44i4Z-v4aZrZ0OlGRI72og93yUXYAs-5c4,7972
 lk_utils/time_utils.py,sha256=6fNWTaZcDjmGGJ-tfKxn8byIja7J6AWNHwXGLdBGHFI,1556
-lk_utils-2.5.5.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_utils-2.5.5.dist-info/METADATA,sha256=Eu1_l9TG5V2E-vBvY7ca49gBn5RFarD6T8YsTTrmVZ0,4234
-lk_utils-2.5.5.dist-info/RECORD,,
+lk_utils-2.5.6.dist-info/METADATA,sha256=T-Tg5MKRXeGO99utcxAf0RUz-EcpmUtmlDnavE_AULg,3723
+lk_utils-2.5.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+lk_utils-2.5.6.dist-info/RECORD,,
```

