# Comparing `tmp/pyverilator-mm-0.7.1.tar.gz` & `tmp/pyverilator-mm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyverilator-mm-0.7.1.tar", last modified: Wed May 24 20:47:07 2023, max compression
+gzip compressed data, was "pyverilator-mm-0.7.2.tar", last modified: Tue Jun 13 21:00:08 2023, max compression
```

## Comparing `pyverilator-mm-0.7.1.tar` & `pyverilator-mm-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 20:47:07.519529 pyverilator-mm-0.7.1/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.1/LICENSE.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4196 2023-05-24 20:47:07.518820 pyverilator-mm-0.7.1/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3402 2023-05-23 20:49:54.000000 pyverilator-mm-0.7.1/README.rst
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 20:47:07.513480 pyverilator-mm-0.7.1/pyverilator/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.1/pyverilator/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.1/pyverilator/__main__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    37982 2023-05-24 00:05:53.000000 pyverilator-mm-0.7.1/pyverilator/pyverilator.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.1/pyverilator/verilator_tools.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6567 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.1/pyverilator/verilatorcpp.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 20:47:07.517128 pyverilator-mm-0.7.1/pyverilator_mm.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4196 2023-05-24 20:47:07.000000 pyverilator-mm-0.7.1/pyverilator_mm.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-05-24 20:47:07.000000 pyverilator-mm-0.7.1/pyverilator_mm.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-24 20:47:07.000000 pyverilator-mm-0.7.1/pyverilator_mm.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-05-24 20:47:07.000000 pyverilator-mm-0.7.1/pyverilator_mm.egg-info/top_level.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-05-24 20:47:07.519872 pyverilator-mm-0.7.1/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-05-23 21:23:28.000000 pyverilator-mm-0.7.1/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.050223 pyverilator-mm-0.7.2/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1086 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/LICENSE.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4419 2023-06-13 21:00:08.049692 pyverilator-mm-0.7.2/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3625 2023-05-24 20:52:32.000000 pyverilator-mm-0.7.2/README.rst
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.041449 pyverilator-mm-0.7.2/pyverilator/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/pyverilator/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      435 2022-12-26 22:28:03.000000 pyverilator-mm-0.7.2/pyverilator/__main__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    38127 2023-06-13 20:41:33.000000 pyverilator-mm-0.7.2/pyverilator/pyverilator.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      565 2023-05-23 21:21:28.000000 pyverilator-mm-0.7.2/pyverilator/verilator_tools.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6892 2023-06-13 19:27:06.000000 pyverilator-mm-0.7.2/pyverilator/verilatorcpp.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-13 21:00:08.045807 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4419 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      317 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       12 2023-06-13 21:00:07.000000 pyverilator-mm-0.7.2/pyverilator_mm.egg-info/top_level.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2023-06-13 21:00:08.050411 pyverilator-mm-0.7.2/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1556 2023-06-13 20:56:38.000000 pyverilator-mm-0.7.2/setup.py
```

### Comparing `pyverilator-mm-0.7.1/LICENSE.txt` & `pyverilator-mm-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.1/PKG-INFO` & `pyverilator-mm-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
@@ -15,14 +15,21 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
 
+PyVerilator-mm
+==============
+
+This is a fork of the original pyverilator package, that manages a newer verilator syntax 
+and works with WSL (by importing tclwraper only if gtkwave is required).
+Below the original readme.
+
 PyVerilator
 ===========
 
 This package provides a wrapper to generate and use verilator
 hardware models in python.
```

### Comparing `pyverilator-mm-0.7.1/README.rst` & `pyverilator-mm-0.7.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+PyVerilator-mm
+==============
+
+This is a fork of the original pyverilator package, that manages a newer verilator syntax 
+and works with WSL (by importing tclwraper only if gtkwave is required).
+Below the original readme.
+
 PyVerilator
 ===========
 
 This package provides a wrapper to generate and use verilator
 hardware models in python.
```

### Comparing `pyverilator-mm-0.7.1/pyverilator/pyverilator.py` & `pyverilator-mm-0.7.2/pyverilator/pyverilator.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,16 +365,17 @@
     """
 
     default_vcd_filename = 'gtkwave.vcd'
 
     @classmethod
     def build(cls, top_verilog_file, preceding_files='', verilog_path = [],
             build_dir = 'obj_dir',
-              json_data = None, gen_only = False, quiet=False,
-              command_args=(), verilog_defines=(), args=[]):
+            json_data = None, gen_only = False, quiet=False,
+            command_args=(), verilog_defines=(), args=[], cargs='', dump_fst = False,
+        ):
         """Build an object file from verilog and load it into python.
 
         Creates a folder build_dir in which it puts all the files necessary to create
         a model of top_verilog_file using verilator and the C compiler. All the files are created in build_dir.
 
         If the project is made of more than one verilog file, all the files used by the top_verilog_file will be searched
         for in the verilog_path list.
@@ -423,29 +424,38 @@
         # Verilator is a perl program that is run as an executable
         # Old versions of Verilator are interpreted as a perl script by the shell,
         # while more recent versions are interpreted as a bash script that calls perl on itself
         which_verilator = shutil.which('verilator')
         if which_verilator is None:
             raise Exception("'verilator' executable not found")
         verilog_defines = ["+define+" + x for x in verilog_defines]
-        # tracing (--trace) is required in order to see internal signals
+        cflags = '-fPIC -shared --std=c++11 -DVL_USER_FINISH ' + cargs
+        if dump_fst:
+            cflags += '-DDUMP_FST'
+
+        vargs = ['-CFLAGS',
+                cflags,
+                '--trace', # tracing (--trace) is required in order to see internal signals
+                '--cc',
+                preceding_files,
+                top_verilog_file,
+                # '--top',
+                # verilog_module_name,
+                '--exe',
+                verilator_cpp_wrapper_path,
+                ]
+
+        if dump_fst:
+            vargs += ['--trace-fst'] # allow fst saving that is faster
+
         verilator_args = ['perl', which_verilator, '-Wno-fatal', '-Mdir', build_dir] \
                          + args \
                          + verilog_path_args \
                          + verilog_defines \
-                         + ['-CFLAGS',
-                           '-fPIC -shared --std=c++11 -DVL_USER_FINISH',
-                            '--trace',
-                            '--cc',
-                            preceding_files,
-                            top_verilog_file,
-                            # '--top',
-                            # verilog_module_name,
-                            '--exe',
-                            verilator_cpp_wrapper_path]
+                         + vargs
         call_process(verilator_args)
 
         # get inputs, outputs, and internal signals by parsing the generated verilator output
         inputs = []
         outputs = []
         internal_signals = []
         verilator_h_file = os.path.join(build_dir, 'V' + verilog_module_name + '.h')
@@ -778,15 +788,15 @@
         if self.vcd_trace is None:
             raise ValueError('stop_vcd_trace() requires VCD tracing to be active')
         stop_vcd_trace = self.lib.stop_vcd_trace
         stop_vcd_trace.argtypes = [ctypes.c_void_p]
         stop_vcd_trace(self.vcd_trace)
         self.vcd_trace = None
         self.auto_tracing_mode = None
-        self.vcd_filename = None
+        # self.vcd_filename = None
 
     def reload_dump_file(self):
         if self.gtkwave_active:
             # this gets the max time before and after the dump file is reloaded to see if it changed
             old_max_time = float(self.gtkwave_tcl.eval('gtkwave::getMaxTime'))
             self.gtkwave_tcl.eval('gtkwave::reLoadFile')
             new_max_time = float(self.gtkwave_tcl.eval('gtkwave::getMaxTime'))
```

### Comparing `pyverilator-mm-0.7.1/pyverilator/verilator_tools.py` & `pyverilator-mm-0.7.2/pyverilator/verilator_tools.py`

 * *Files identical despite different names*

### Comparing `pyverilator-mm-0.7.1/pyverilator/verilatorcpp.py` & `pyverilator-mm-0.7.2/pyverilator/verilatorcpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 from pyverilator.verilator_tools import verilator_flushcall_ok
 
 def header_cpp(top_module):
-    s = """#include <cstddef>
-#include "verilated.h"
-#include "verilated_vcd_c.h"
-#include "{module_filename}.h"
-    """.format(module_filename='V' + top_module)
-    return s
-
+    return f"""#include <cstddef>
+    #include "verilated.h"
+    #if VM_TRACE
+        #ifndef DUMPLEVEL
+            #define DUMP_LEVEL 0
+        #endif
+        #ifdef DUMP_FST
+            #include <verilated_fst_c.h>
+            #define DUMP_TYPE VerilatedFstC
+            // #define DUMP_FILE "dump.fst"
+        #else
+            #include <verilated_vcd_c.h>
+            #define DUMP_TYPE VerilatedVcdC
+            // #define DUMP_FILE "dump.vcd"
+        #endif
+    #endif
+    #include "{'V' + top_module}.h"
+    """
 
 def var_declaration_cpp(top_module, inputs, outputs, internal_signals, json_data):
     s = """// pyverilator defined values
 // first declare variables as extern
 extern const char* _pyverilator_module_name;
 extern const uint32_t _pyverilator_num_inputs;
 extern const char* _pyverilator_inputs[];
@@ -96,29 +107,29 @@
 int destruct({module_filename}* top) {{
     if (top != nullptr) {{
         delete top;
         top = nullptr;
     }}
     return 0;
 }}
-VerilatedVcdC* start_vcd_trace({module_filename}* top, const char* filename) {{
-    VerilatedVcdC* tfp = new VerilatedVcdC;
-    top->trace(tfp, 99);
+DUMP_TYPE* start_vcd_trace({module_filename}* top, const char* filename) {{
+    DUMP_TYPE* tfp = new DUMP_TYPE;
+    top->trace(tfp, DUMP_LEVEL);
     tfp->open(filename);
     return tfp;
 }}
-int add_to_vcd_trace(VerilatedVcdC* tfp, int time) {{
+int add_to_vcd_trace(DUMP_TYPE* tfp, int time) {{
     tfp->dump(time);
     return 0;
 }}
-int flush_vcd_trace(VerilatedVcdC* tfp) {{
+int flush_vcd_trace(DUMP_TYPE* tfp) {{
     tfp->flush();
     return 0;
 }}
-int stop_vcd_trace(VerilatedVcdC* tfp) {{
+int stop_vcd_trace(DUMP_TYPE* tfp) {{
     tfp->close();
     return 0;
 }}
 bool get_finished() {{
     return Verilated::gotFinish();
 }}
 void set_finished(bool b) {{
@@ -145,15 +156,15 @@
             "int set_{portname}({module_filename}* top, uint64_t new_value)"
             "{{ top->{portname} = new_value; return 0;}}" if port[1] > 32 else
             "int set_{portname}({module_filename}* top, uint32_t new_value)"
             "{{ top->{portname} = new_value; return 0;}}")).format(module_filename='V' + top_module, portname=port[0])
                                   , inputs))
     footer = "}"
     
-    if not(verilator_flushcall_ok()):
+    if not verilator_flushcall_ok():
         constant_part = constant_part.replace('Verilated::flushCall();','Verilated::runFlushCallbacks();')
     
     return "\n".join([constant_part, get_functions, set_functions, footer])
 
 
 def template_cpp(top_module, inputs, outputs, internal_signals, json_data):
     return "\n".join([header_cpp(top_module),
```

### Comparing `pyverilator-mm-0.7.1/pyverilator_mm.egg-info/PKG-INFO` & `pyverilator-mm-0.7.2/pyverilator_mm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverilator-mm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python interface to Verilator models
 Home-page: https://github.com/bat52/pyverilator
 Author: CSAIL CSG, Marco Merlin
 Author-email: acwright@mit.edu, bthom@mit.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bat52/pyverilator/issues
 Project-URL: Source, https://github.com/bat52/pyverilator
@@ -15,14 +15,21 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
 
+PyVerilator-mm
+==============
+
+This is a fork of the original pyverilator package, that manages a newer verilator syntax 
+and works with WSL (by importing tclwraper only if gtkwave is required).
+Below the original readme.
+
 PyVerilator
 ===========
 
 This package provides a wrapper to generate and use verilator
 hardware models in python.
```

### Comparing `pyverilator-mm-0.7.1/setup.py` & `pyverilator-mm-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyverilator-mm',
-    version='0.7.1',
+    version='0.7.2',
     description='Python interface to Verilator models',
     long_description=long_description,
     url='https://github.com/bat52/pyverilator',
     author='CSAIL CSG, Marco Merlin',
     author_email='acwright@mit.edu, bthom@mit.edu',
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

