# Comparing `tmp/mybar-0.7.2.tar.gz` & `tmp/mybar-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.7.2.tar", last modified: Mon Jun 12 09:15:14 2023, max compression
+gzip compressed data, was "mybar-0.8.tar", last modified: Tue Jun 13 05:46:33 2023, max compression
```

## Comparing `mybar-0.7.2.tar` & `mybar-0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7.2/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-12 09:15:14.052176 mybar-0.7.2/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7.2/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)      601 2023-06-12 09:13:43.000000 mybar-0.7.2/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7.2/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7.2/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7.2/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13417 2023-06-12 09:11:45.000000 mybar-0.7.2/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7.2/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7.2/mybar/defaults.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7.2/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13999 2023-06-06 11:33:06.000000 mybar-0.7.2/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28082 2023-06-06 12:01:35.000000 mybar-0.7.2/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7.2/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7.2/mybar/sync.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/templates.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7.2/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7.2/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7.2/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      892 2023-06-12 09:15:14.052176 mybar-0.7.2/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 05:46:33.946949 mybar-0.8/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.8/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-13 05:46:33.946949 mybar-0.8/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.8/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 05:46:33.946949 mybar-0.8/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)      599 2023-06-13 05:44:35.000000 mybar-0.8/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.8/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.8/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.8/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    46624 2023-06-13 05:32:56.000000 mybar-0.8/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16057 2023-06-13 04:53:29.000000 mybar-0.8/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-12 10:18:51.000000 mybar-0.8/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.8/mybar/defaults.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.8/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    29233 2023-06-12 10:17:43.000000 mybar-0.8/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13999 2023-06-06 11:33:06.000000 mybar-0.8/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28082 2023-06-06 12:01:35.000000 mybar-0.8/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.8/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2136 2023-06-13 05:39:28.000000 mybar-0.8/mybar/namespaces.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.8/mybar/sync.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.8/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-13 05:46:33.946949 mybar-0.8/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-13 05:46:33.000000 mybar-0.8/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      469 2023-06-13 05:46:33.000000 mybar-0.8/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-13 05:46:33.000000 mybar-0.8/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-13 05:46:33.000000 mybar-0.8/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-13 05:46:33.000000 mybar-0.8/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.8/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.8/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      890 2023-06-13 05:46:33.946949 mybar-0.8/setup.cfg
```

### Comparing `mybar-0.7.2/LICENSE` & `mybar-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/PKG-INFO` & `mybar-0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7.2
+Version: 0.8
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7.2/mybar/__init__.py` & `mybar-0.8/mybar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 :copyright: (c) 2021-present by LonelyAbsol.
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'mybar'
 __description__ = "An async status bar with a highly customizable API."
 __url__ = "https://github.com/lonelyabsol/mybar"
-__version__ = '0.7.2'
+__version__ = '0.8'
 __author__ = "LonelyAbsol"
 __license__ = 'MIT'
 __copyright__ = "Copyright (c) 2021-present LonelyAbsol"
 
 
 from .constants import *
 from . import utils
```

### Comparing `mybar-0.7.2/mybar/_setups.py` & `mybar-0.8/mybar/_setups.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/_types.py` & `mybar-0.8/mybar/_types.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/bar.py` & `mybar-0.8/mybar/bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from . import cli
 from . import field_funcs
 from . import utils
 from .errors import *
 from .field import Field, FieldPrecursor, FieldSpec
 from .formatting import FormatStr, FmtStrStructure, FormatterFieldSig
-from .templates import BarConfigSpec, BarSpec, FieldSpec
+from .namespaces import BarConfigSpec, BarSpec, FieldSpec
 from ._types import (
     Args,
     ConsoleControlCode,
     FieldName,
     FieldOrder,
     Icon,
     JSONText,
@@ -162,44 +162,45 @@
         :type write_new_file_dft: :class:`bool`
 
         :returns: A new :class:`BarConfig`
         :rtype: :class:`BarConfig`
         '''
         parser = cli.Parser()
         try:
-            bar_options = parser.parse_args()
+            bar_options, command_options = parser.parse_args()
         except CLIUsageError as e:
             parser.error(e.msg)  # Shows usage
 
-        if 'field_options' in bar_options:
-            fields = parser.process_field_options(
-                bar_options.pop('field_options')
-            )
-            bar_options['field_definitions'] = fields
+        # Handle options that alter the behavior of the command itself:
+        if command_options:
+            if 'dump_config' in command_options:
+                indent = command_options.pop('dump_config', None)
+                config = cls(bar_options)
+                parser.quit(cls._as_json(config, indent=indent))
 
         # Handle missing config files:
         if 'config_file' not in bar_options:
-            if (first_use := (not os.path.exists(CONFIG_FILE))):
-                cls.welcome_new_users()
-                cls.maybe_make_config_dir()
+            file = CONFIG_FILE
+            if not os.path.exists(file):
                 wants_to_write = cls.write_with_approval(overrides=bar_options)
                 if not wants_to_write:
                     # Forget all this config file business.
-                    # Our new user is in a rush. Let's give them a bar.
+                    # Our new user is in a hurry, so
+                    # just give them what they need:
                     return cls(bar_options)
 
-        file = bar_options.pop('config_file', None)
+        else:
+            file = bar_options.pop('config_file', None)
 
         try:
-            # config_file is in overrides or it defaults to CONFIG_FILE:
+            # If 'config_file' is not in `overrides`,
+            # it defaults to CONFIG_FILE.
             config = cls.from_file(file, overrides=bar_options)
 
         except FileNotFoundError as e:
-            file = e.filename
-            cls.maybe_make_config_dir()
             write_ok = cls.write_with_approval(file, overrides=bar_options)
             if not write_ok:
                 parser.quit("Exiting...")
             config = cls.from_file(file, overrides=bar_options)
 
         except OSError as e:
             e.add_note("Exiting...")
@@ -224,15 +225,15 @@
         :type file: :class:`PathLike`
 
         :returns: ``True`` if the file was written, ``False`` if not
         '''
         if file is None:
             file = CONFIG_FILE
 
-        approved = cls._get_write_new_approval(
+        approved = cli.FileManager._get_write_new_approval(
             file,
             dft_choice=True
         )
         if approved:
             try:
                 cls._write_file(file, overrides)
             except FileNotFoundError as e:
@@ -245,60 +246,14 @@
                     raise e from None
 
             print(f"Wrote new config file to {file!r}")
             return True
 
         return False
 
-    @classmethod
-    def _get_write_new_approval(
-        cls,
-        file: PathLike,
-        dft_choice: bool
-    ) -> bool:
-        '''
-        Get approval to write a new config file using
-            :class:`cli.OptionsAsker`.
-
-        :param file: The path to the config file
-        :type file: :class:`PathLike`
-
-        :param dft_choice: The default option to present to the user
-        :type dft_choice: :class:``
-        '''
-        dft = (file == CONFIG_FILE)
-        msg = (
-            f"The {'default' if dft else ''}"
-            f" config file at {file!r} does not exist."
-        )
-        question = "Would you like to make it now?"
-        write_options = {'y': True, 'n': False}
-        default = 'ny'[dft_choice]
-        handler = cli.OptionsAsker(write_options, default, question)
-
-        print(msg)
-        write_new_file_ok = handler.ask()
-        return write_new_file_ok
-
-    @classmethod
-    def maybe_make_config_dir(cls) -> None:
-        '''
-        Make a config directory in the default location if nonexistent.
-        '''
-        directory = os.path.dirname(CONFIG_FILE)
-        if not os.path.exists(directory):
-            os.mkdir(directory)
-
-    @classmethod
-    def welcome_new_users(cls) -> None:
-        msg = (
-            f"-- {__package__} --"
-        )
-        print(msg)
-
     @staticmethod
     def _read_file(file: PathLike) -> tuple[BarConfigSpec, JSONText]:
         '''
         Read a given config file.
         Convert its JSON contents to a dict and return it along with the
         raw text of the file.
 
@@ -314,55 +269,96 @@
             text = f.read()
         return data, text
 
     @classmethod
     def _write_file(
         cls,
         file: PathLike,
-        obj: BarSpec = {},
+        spec: BarSpec = {},
+        indent: int = 4,
         *,
         defaults: BarSpec = None
     ) -> None:
-        '''Write :class:`BarConfig` params to a JSON file.
+        '''
+        Write :class:`BarConfig` params to a JSON file.
 
         :param file: The file to write to
         :type file: :class:`PathLike`
 
-        :param obj: The :class:`_types.BarConfigSpec` to write
-        :type obj: :class:`_types.BarConfigSpec`, optional
+        :param spec: The :class:`_types.BarSpec` to write
+        :type spec: :class:`_types.BarSpec`, optional
+
+        :param indent: How many spaces to indent by, defaults to ``4``
+        :type indent: :class:`int`
 
-        :param defaults: Any default parameters that `obj` should override,
+        :param defaults: Any default parameters that `spec` should override,
+            defaults to :attr:`Bar._default_params`
+        :type defaults: :class:`_types.BarSpec`
+        '''
+        un_pythoned = cls._remove_unserializable(spec, defaults=defaults)
+        absolute = os.path.abspath(os.path.expanduser(file))
+        if absolute == CONFIG_FILE and not os.path.exists(absolute):
+            cli.FileManager._maybe_make_config_dir()
+        with open(os.path.expanduser(absolute), 'w') as f:
+            json.dump(un_pythoned, f, indent=indent, ) #separators=(',\n', ': '))
+
+    @classmethod
+    def _remove_unserializable(
+        cls,
+        spec: BarConfigSpec,
+        *,
+        defaults: BarSpec = None
+    ) -> BarConfigSpec:
+        '''
+        Remove Python-specific API elements like functions which cannot
+        be serialized for writing to files.
+
+        :param spec: The :class:`_types.BarConfigSpec` to convert
+        :type spec: :class:`_types.BarConfigSpec`
+
+        :param defaults: Any default parameters that `spec` should override,
             defaults to :attr:`Bar._default_params`
         :type defaults: :class:`_types.BarSpec`
         '''
         if defaults is None:
             defaults = Bar._default_params.copy()
 
-        newobj = obj.copy()
+        newobj = spec.copy()
         newobj.pop('config_file', None)
-        newobj = defaults | obj
+        newobj = defaults | spec
 
-        fields = Field._default_fields.copy()
+        fields = newobj.pop('field_definitions', {})
 
         # Clean the dict of irrelevant Field implementation details:
         for name, field in fields.items():
             new = fields[name] = field.copy()
             for param in ('name', 'func', 'setup'):
                 try:
                     del new[param]
                 except KeyError:
                     pass
 
-        newobj['field_definitions'] = fields
+        if fields:
+            newobj['field_definitions'] = fields
 
-        absolute = os.path.abspath(os.path.expanduser(file))
-        if absolute == CONFIG_FILE and not os.path.exists(absolute):
-            cls.maybe_make_config_dir()
-        with open(os.path.expanduser(absolute), 'w') as f:
-            json.dump(newobj, f, indent=4, ) #separators=(',\n', ': '))
+        return newobj
+
+    @classmethod
+    def _as_json(cls, spec: BarSpec = {}, indent: int = 4) -> JSONText:
+        '''
+        Return a :class:`BarConfig` as a string with JSON formatting.
+
+        :param spec: The :class:`_types.BarSpec` to convert
+        :type spec: :class:`_types.BarSpec`, optional
+
+        :param indent: How many spaces to indent by, defaults to ``4``
+        :type indent: :class:`int`
+        '''
+        cleaned = cls._remove_unserializable(spec)
+        return json.dumps(cleaned, indent=indent)
 
 
 class Bar:
     '''
     Create highly customizable status bars.
 
     :param fields: An iterable of default field names or :class:`Field` instances, defaults to ``None``
@@ -1024,31 +1020,29 @@
         :type bg: :class:`bool`
 
         :returns: ``None``
 
         .. note::
             This method cannot be called within an async event loop.
         '''
+        if self.count == 0:
+            return
+
         try:
             if stream is not None:
                 self._stream = stream
             if once is None:
                 once = self.run_once
             else:
                 self.run_once = once
 
             # Allow the bar to run repeatedly in the same interpreter:
             if self._loop.is_closed():
                 self._loop = asyncio.new_event_loop()
-            #NOTE: Need a way to handle stale coroutines.
-            # Like, run prepare_fields() again.
 
-##            self._coros = {}
-##            self._threads = {}
-##            self._timely_fields = []
             self._prepare_fields()
             self._can_run.set()
             for thread in tuple(self._threads.values()):
                 thread.start()
             self._preload_timely_fields()
 
             if not once:
```

### Comparing `mybar-0.7.2/mybar/cli.py` & `mybar-0.8/mybar/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 __all__ = (
     'Parser',
     'OptionsAsker',
 )
 
 
+import os.path
 from argparse import ArgumentParser, SUPPRESS, Namespace, HelpFormatter
 from enum import Enum
+from os import PathLike
 
+from . import __version__
+from .constants import CONFIG_FILE
 from .errors import AskWriteNewFile, CLIFatalError, CLIUsageError
-from .templates import BarConfigSpec, FieldSpec
+from .namespaces import BarConfigSpec, CmdOptionSpec, FieldSpec
 from ._types import (
     AssignmentOption,
     FieldName,
     OptName,
     OptSpec,
 )
 
@@ -52,27 +56,43 @@
     def __init__(self) -> None:
         super().__init__(
             prog=PROG,
             argument_default=SUPPRESS,
         )
         self.add_arguments()
 
-    def parse_args(self, args: None | list[str] = None) -> BarConfigSpec:
+    def parse_args(
+        self,
+        args: list[str] = None
+    ) -> tuple[BarConfigSpec, CmdOptionSpec]:
         '''
         Parse command line arguments and return a dict of options.
         This will additionally process args with key-value pairs.
         If `args` is None, process from STDIN.
 
         :param args: The args to parse, get from STDIN by default
         :type args: :class:`list[str]`
         '''
         # Use vars() because dict items are more portable than attrs.
         opts = vars(super().parse_args(args))
         params = self.process_assignment_args(opts)
-        return params
+
+        # For options that control specific fields:
+        if 'field_options' in params:
+            fields = self.process_field_options(
+                params.pop('field_options')
+            )
+            params['field_definitions'] = fields
+
+        # For options that control what the command does:
+        keys = (
+            CmdOptionSpec.__optional_keys__ ^ CmdOptionSpec.__required_keys__
+        )
+        cmd_options = {k: params.pop(k) for k in keys if k in params}
+        return params, cmd_options
 
     def process_assignment_args(
         self,
         opts: BarConfigSpec,
         assignments: dict[FieldName, str] = None
     ) -> BarConfigSpec:
         '''
@@ -174,59 +194,59 @@
 
         return field_definitions
 
     def add_arguments(self) -> None:
         '''Equip the parser with all its arguments.'''
         fields_or_tmpl = self.add_mutually_exclusive_group()
         fields_or_tmpl.add_argument(
-            '-t', '--template',
-            metavar="'TEMPLATE'",
+            '--template', '-t',
             dest='template',
             help=(
                 "A curly-brace-delimited format string."
                 " Not valid with --fields/-f options."
             ),
+            metavar="'TEMPLATE'",
         )
 
         fields_or_tmpl.add_argument(
-            '-f', '--fields',
+            '--fields', '-f',
             action='extend',
-            nargs='+',
-            metavar=('FIELDNAME1', 'FIELDNAME2'),
             dest='field_order',
-            # type=ArgFormatter.SplitFirst(','),
             help=(
                 "A list of fields to be displayed."
                 " Not valid with --template/-t options."
             ),
+            metavar=('FIELDNAME1', 'FIELDNAME2'),
+            nargs='+',
+            # type=ArgFormatter.SplitFirst(','),
         )
 
         fields_group = self.add_argument_group(
             title="Options for fields",
             description="These options are not valid when using --template/-t."
         )
 
         fields_group.add_argument(
             '--icons',
             action='extend',
-            nargs='+',
-            metavar=("FIELDNAME1='ICON1'", "FIELDNAME2='ICON2'"),
             dest='icon_pairs',
             help="A mapping of field names to icons.",
+            metavar=("FIELDNAME1='ICON1'", "FIELDNAME2='ICON2'"),
+            nargs='+',
         )
 
         fields_group.add_argument(
-            '-s', '--separator',
-            type=ArgFormatter.ToTuple(length=2),
-            metavar="'FIELD_SEPARATOR'",
+            '--separator', '-s',
             dest='separators',
             help=(
                 "The character used for joining fields."
                 " Only valid with --field/-f options."
             ),
+            metavar="'FIELD_SEPARATOR'",
+            type=ArgFormatter.ToTuple(length=2),
         )
 
         fields_group.add_argument(
             '--join-empty', '-j',
             action='store_true',
             dest='join_empty_fields',
             help=(
@@ -234,71 +254,86 @@
                 " Only valid with --field/-f options."
             ),
         )
 
         fields_group.add_argument(
             '--options', '-o',
             action='extend',
-            nargs='+',
-            metavar=("'FIELD1.OPTION=VAL'", "'FIELD2.OPTION=VAL'"),
             dest='field_options',
             help=(
                 "Set arbitrary options for discrete Fields using"
                 " dot-attribute syntax."
             ),
+            metavar=("'FIELD1.OPTION=VAL'", "'FIELD2.OPTION=VAL'"),
+            nargs='+',
         )
 
         self.add_argument(
             '-r', '--refresh',
-            type=float,
             dest='refresh_rate',
             help=(
                 "The bar's refresh rate in seconds per cycle."
             ),
+            type=float,
         )
 
         self.add_argument(
             '--count', '-n',
-            type=int,
-            metavar='TIMES',
             dest='count',
             help=(
                 "Print the bar this many times, then exit."
             ),
+            metavar='TIMES',
+            type=int,
         )
 
         self.add_argument(
             '--config', '-c',
-            metavar='FILE',
             dest='config_file',
             help=(
                 "The config file to use for default settings."
             ),
+            metavar='FILE',
         )
 
-##        self.add_argument(
-##            '--dump', '-d',
-##            type=int,
-##            nargs='?',
-##            metavar='INDENT',
-##            dest='dump_config',
-##            help=(
-##                "Instead of running the bar, print a JSON config using"
-##                " options specified in the command."
-##                " Optionally pass a number of spaces to indent by,"
-##                " which defaults to 4."
-##            ),
-##        )
+        self.add_argument(
+            '--dump', '-d',
+            action='store_const',
+            const=4,
+            dest='dump_config',
+            help=(
+                "Instead of running the Bar, print a JSON config using"
+                " options specified in the command."
+                " Optionally pass a number of spaces by which to indent."
+            ),
+        )
+
+        self.add_argument(
+            '--dump-raw', '-D',
+            action='store_const',
+            const=None,
+            dest='dump_config',
+            help=(
+                "Instead of running the Bar, print a JSON config using"
+                " options specified in the command."
+            ),
+        )
 
         self.add_argument(
             '--debug',
             action='store_true',
             help="Use debug mode. (Not implemented)",
         )
 
+        self.add_argument(
+            '--version', '-v',
+            action='version',
+            version=f"{__package__} {__version__}",
+        )
+
     def quit(self, message: str = "Exiting...") -> NoReturn:
         '''Print a message and exit the program.'''
         self.exit(1, message + '\n')
 
 
 class HighlightMethod(Enum):
     '''Ways to present default option names.'''
@@ -412,7 +447,65 @@
             if not self.case_sensitive:
                 answer = answer.casefold()
             if repeat_prompt or prompted:
                 continue
             prompt = options + " "
         return self.choices.get(answer)
 
+
+def welcome_new_users() -> None:
+    msg = (
+        f"-- {PROG} --"
+    )
+    print(msg)
+
+
+##class ConfigWizard:
+class FileManager:
+
+    @classmethod
+    def _get_write_new_approval(
+        cls,
+        file: PathLike,
+        dft_choice: bool
+    ) -> bool:
+        '''
+        Get approval to write a new config file using
+            :class:`cli.OptionsAsker`.
+
+        :param file: The path to the config file
+        :type file: :class:`PathLike`
+
+        :param dft_choice: The default option to present to the user
+            (``False`` means do not write)
+        :type dft_choice: :class:`bool`
+        '''
+        question = f"Would you like to write a new config file at {file!r}?"
+
+        if not os.path.exists(file):
+            maybe_default = ' '
+            if file == CONFIG_FILE:
+                welcome_new_users()
+                cls._maybe_make_config_dir()
+                maybe_default = ' default '
+            msg = (
+                f"The{maybe_default}config file at {file!r} does not exist."
+            )
+            print(msg)
+            question = "Would you like to make it now?"
+
+        write_options = {'y': True, 'n': False}
+        default = 'ny'[dft_choice]
+        handler = OptionsAsker(write_options, default, question)
+
+        write_new_file_ok = handler.ask()
+        return write_new_file_ok
+
+    @staticmethod
+    def _maybe_make_config_dir() -> None:
+        '''
+        Make a '.config' directory if nonexistent.
+        '''
+        directory = os.path.dirname(CONFIG_FILE)
+        if not os.path.exists(directory):
+            os.mkdir(directory)
+
```

### Comparing `mybar-0.7.2/mybar/constants.py` & `mybar-0.8/mybar/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,19 @@
 HIDE_CURSOR: ConsoleControlCode = '?25l'
 '''VT100 escape code to hide the cursor.'''
 
 UNHIDE_CURSOR: ConsoleControlCode = '?25h'
 '''VT100 escape code to unhide the cursor.'''
 
 
-FONTAWESOME_ICONS = tuple('')
+FONTAWESOME_ICONS = {
+    'uptime': '',
+    'cpu_usage': '',
+    'cpu_temp': '',
+    'mem_usage': '',
+    'disk_usage': '',
+    'battery': '',
+    'net_stats': '',
+}
+
 USING_FONTAWESOME = False
```

### Comparing `mybar-0.7.2/mybar/defaults.py` & `mybar-0.8/mybar/defaults.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/errors.py` & `mybar-0.8/mybar/errors.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/field.py` & `mybar-0.8/mybar/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import field_funcs
 from . import _setups
 from . import utils
 from .constants import DEBUG
 from .errors import *
 from .formatting import FormatterFieldSig
-from .templates import FieldSpec
+from .namespaces import FieldSpec
 from ._types import (
     FieldName,
     Icon,
     PTY_Icon,
     TTY_Icon,
     FormatStr,
     Args,
@@ -128,84 +128,108 @@
             'run_once': True
         },
 
         'host': {
             'name': 'host',
             'func': field_funcs.get_host,
             'kwargs': {
-                'fmt': '{nodename}',
+                'fmt': "{nodename}",
             },
             'run_once': True
         },
 
         'uptime': {
             'name': 'uptime',
             'func': field_funcs.get_uptime,
-            'setup': _setups.setup_uptime,
-            'timely': True,
-            'align_to_seconds': True,
             'kwargs': {
                 'fmt': '{days}d:{hours}h:{mins}m',
-                'sep': ':'
+                'dynamic': True,
+                'sep': ':',
             },
-            'icons': [' ', 'Up '],
+            'setup': _setups.setup_uptime,
+            'timely': True,
+            'align_to_seconds': True,
+            'icon': 'Up ',
         },
 
         'cpu_usage': {
             'name': 'cpu_usage',
             'func': field_funcs.get_cpu_usage,
+            'kwargs': {
+                'fmt': "{:02.0f}%",
+            },
             'interval': 5,
             'threaded': True,
-            'icons': [' ', 'CPU '],
+            'icon': 'CPU ',
         },
 
         'cpu_temp': {
             'name': 'cpu_temp',
             'func': field_funcs.get_cpu_temp,
+            'kwargs': {
+                'fmt': "{temp:02.0f}{scale}",
+            },
             'interval': 5,
             'threaded': True,
-            'icons': [' ', ''],
         },
 
         'mem_usage': {
             'name': 'mem_usage',
             'func': field_funcs.get_mem_usage,
+            'kwargs': {
+                'fmt': "{used:.1f}{unit}",
+                'unit': 'G',
+            },
             'interval': 5,
-            'icons': [' ', 'Mem '],
+            'icon': 'Mem ',
         },
 
         'disk_usage': {
             'name': 'disk_usage',
             'func': field_funcs.get_disk_usage,
+            'kwargs': {
+                'fmt': "{free:.1f}{unit}",
+                'path': '/',
+                'unit': 'G',
+            },
             'interval': 5,
-            'icons': [' ', '/:'],
+            'icon': '/:',
         },
 
         'battery': {
             'name': 'battery',
+            'kwargs': {
+                'fmt': "{pct:02.0f}{state}",
+            },
             'func': field_funcs.get_battery_info,
             'threaded': True,
-            'icons': [' ', 'Bat '],
+            'icon': 'Bat ',
         },
 
         'net_stats': {
             'name': 'net_stats',
             'func': field_funcs.get_net_stats,
+            'kwargs': {
+                # 'device': None,
+                'fmt': "{name}",
+                'nm': True,
+                'nm_filt': None,
+                'default': "",
+            },
             'interval': 5,
-            'icons': [' ', ''],
         },
 
         'datetime': {
             'name': 'datetime',
             'func': field_funcs.get_datetime,
-            'align_to_seconds': True,
-            'timely': True,
             'kwargs': {
-                'fmt': "%Y-%m-%d %H:%M:%S"
+                'fmt': "%Y-%m-%d %H:%M:%S",
             },
+            'align_to_seconds': True,
+            'timely': True,
         }
 
     }
 
     def __init__(
         self,
         *,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mybar-0.7.2/mybar/field_funcs.py` & `mybar-0.8/mybar/field_funcs.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/formatting.py` & `mybar-0.8/mybar/formatting.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/sync.py` & `mybar-0.8/mybar/sync.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar/templates.py` & `mybar-0.8/mybar/namespaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = (
     'FieldSpec',
     'BarSpec',
-    'BarConfigSpec'
+    'BarConfigSpec',
+    'CMDLineSpec',
 )
 
 
 from os import PathLike
 
 # from .field import FieldSpec
 # from .bar import BarConfig, BarConfigSpec, BarSpec
@@ -26,15 +27,18 @@
 from typing import ParamSpec, Required, TypedDict, TypeVar
 
 
 Bar = TypeVar('Bar')
 P = ParamSpec('P')
 
 class FieldSpec(TypedDict, total=False):
-    '''A dict representation of :class:`mybar.Field` constructor parameters.'''
+    '''
+    Specifies the structure of :class:`mybar.Field` constructor
+    parameters.
+    '''
     name: Required[FieldName]
     func: Callable[P, str]
     icon: Icon
     template: FormatStr
     interval: float
     align_to_seconds: bool
     overrides_refresh: bool
@@ -48,15 +52,17 @@
     # setup: Callable[P, Kwargs]
     setup: Callable[P, P.kwargs]
     # Set this to use different icons for different output streams:
     icons: Sequence[PTY_Icon, TTY_Icon]
 
 
 class BarSpec(TypedDict, total=False):
-    '''A dict representation of :class:`mybar.Bar` constructor parameters.'''
+    '''
+    Specifies the structure of :class:`mybar.Bar` constructor parameters.
+    '''
     refresh_rate: float
     run_once: bool
     align_to_seconds: bool
     join_empty_fields: bool
     override_cooldown: float
     thread_cooldown: float
 
@@ -67,12 +73,22 @@
     separators: Sequence[PTY_Separator, TTY_Separator]
 
     # The `template` param is mutually exclusive with all field params.
     template: FormatStr
 
 
 class BarConfigSpec(BarSpec, total=False):
-    '''A dict representation of :class:`mybar.bar.BarConfig` constructor parameters.'''
+    '''
+    Specifies the structure of :class:`mybar.bar.BarConfig` constructor
+    parameters.
+    '''
     config_file: PathLike
     debug: bool
     field_icons: dict[FieldName, Icon]
 
+
+class CmdOptionSpec(TypedDict, total=False):
+    '''
+    Specifies the structure of command options.
+    '''
+    dump_config: bool | int = 4
+
```

### Comparing `mybar-0.7.2/mybar/utils.py` & `mybar-0.8/mybar/utils.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.2/mybar.egg-info/PKG-INFO` & `mybar-0.8/mybar.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7.2
+Version: 0.8
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7.2/setup.cfg` & `mybar-0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mybar
-version = 0.7.2
+version = 0.8
 description = An async status bar with a highly customizable API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = lonelyabsol
 url = https://github.com/lonelyabsol/mybar
 project_urls = 
 	GitHub: repo = https://github.com/lonelyabsol/mybar
```

