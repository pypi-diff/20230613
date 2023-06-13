# Comparing `tmp/mwxlib-0.85.2-py3-none-any.whl.zip` & `tmp/mwxlib-0.85.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161488 bytes, number of entries: 22
+Zip file size: 161513 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-03 17:04 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    44266 b- defN 23-Jun-10 16:10 mwx/controls.py
--rw-rw-rw-  2.0 fat    72505 b- defN 23-Jun-10 16:10 mwx/framework.py
+-rw-rw-rw-  2.0 fat    72480 b- defN 23-Jun-13 15:18 mwx/framework.py
 -rw-rw-rw-  2.0 fat    68631 b- defN 23-Jun-05 07:49 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    45726 b- defN 23-Jun-10 16:10 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-Jun-03 17:04 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-Jun-03 17:04 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27598 b- defN 23-Jun-03 17:04 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   139039 b- defN 23-Jun-10 16:10 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat   139026 b- defN 23-Jun-13 15:30 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37369 b- defN 23-Jun-05 06:59 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11670 b- defN 23-Jun-10 12:36 mwx/wxmon.py
--rw-rw-rw-  2.0 fat    19367 b- defN 23-Jun-03 17:04 mwx/wxpdb.py
+-rw-rw-rw-  2.0 fat    19456 b- defN 23-Jun-13 15:30 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-Jun-03 17:04 mwx/wxwil.py
--rw-rw-rw-  2.0 fat     8196 b- defN 23-Jun-10 12:36 mwx/wxwit.py
+-rw-rw-rw-  2.0 fat     8196 b- defN 23-Jun-13 14:18 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-03 17:04 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-10 16:21 mwxlib-0.85.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-10 16:21 mwxlib-0.85.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 16:21 mwxlib-0.85.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-10 16:21 mwxlib-0.85.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-10 16:21 mwxlib-0.85.2.dist-info/RECORD
-22 files, 614772 bytes uncompressed, 158986 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-13 15:45 mwxlib-0.85.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-13 15:45 mwxlib-0.85.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 15:45 mwxlib-0.85.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-13 15:45 mwxlib-0.85.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-13 15:45 mwxlib-0.85.3.dist-info/RECORD
+22 files, 614823 bytes uncompressed, 159011 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.85.2.dist-info/LICENSE
+Filename: mwxlib-0.85.3.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.85.2.dist-info/METADATA
+Filename: mwxlib-0.85.3.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.85.2.dist-info/WHEEL
+Filename: mwxlib-0.85.3.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.85.2.dist-info/top_level.txt
+Filename: mwxlib-0.85.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.85.2.dist-info/RECORD
+Filename: mwxlib-0.85.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.85.2"
+__version__ = "0.85.3"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -119,15 +119,15 @@
     wx.WXK_UP                   : 'up',
     wx.WXK_WINDOWS_LEFT         : 'Lwin',
     wx.WXK_WINDOWS_MENU         : 'appskey',
     wx.WXK_WINDOWS_RIGHT        : 'Rwin',
 }
 
 def speckey_state(key):
-    """Returns GetKeyState for abbreviation key:str."""
+    """Returns `KeyState` for abbreviation key:str."""
     try:
         return wx.GetKeyState(_speckeys_wxkmap[key])
     except KeyError:
         pass
 _speckeys_wxkmap = dict((v, k) for k, v in _speckeys.items())
 
 
@@ -786,15 +786,14 @@
         if j != -1:
             wnd = wx.Window.FindFocus() # original focus
             org = self.CurrentPage
             if j != self.Selection:
                 self.Selection = j # the focus is moved
             if wnd and wnd is not org: # restore focus other window
                 wnd.SetFocus()
-            return win
     
     def find_tab(self, win):
         """Returns AuiTabCtrl and AuiNotebookPage for the window.
         
         cf. aui.AuiNotebook.FindTab -> bool, tab, idx
         Note:
             Argument `win` can also be page.window.Name (not page.caption).
```

## mwx/nutshell.py

```diff
@@ -1577,15 +1577,15 @@
             return
         pos = evt.Position
         if self.IndicatorValueAt(2, pos):
             p = self.IndicatorStart(2, pos)
             q = self.IndicatorEnd(2, pos)
             text = self.GetTextRange(p, q).strip()
             self.message("URL {!r}".format(text))
-            ## Note: Do postcall a confirmation dialog.
+            ## Note: Need a post-call of the confirmation dialog.
             wx.CallAfter(self.parent.load_url, text)
     
     def on_modified(self, buf):
         """Called when the buffer is modified."""
         self.SetIndicatorCurrent(2)
         self.IndicatorClearRange(0, self.TextLength)
         for m in self.grep(url_re):
@@ -1992,22 +1992,22 @@
         if res.status_code == 200: # success
             buf = self.find_buffer(url) or self.create_buffer(url)
             buf._load_textfile(res.text, url, lineno)
             self.swap_page(buf)
             return True
         return False
     
-    def load_cache(self, filename, lineno=0, globals=None):
+    def load_cache(self, filename, lineno=0):
         """Load a file from cache using linecache.
         Note:
             The filename should be an absolute path.
             The buffer will be reloaded without confirmation.
         """
         linecache.checkcache(filename)
-        lines = linecache.getlines(filename, globals)
+        lines = linecache.getlines(filename)
         if lines:
             buf = self.find_buffer(filename) or self.create_buffer(filename)
             buf._load_textfile(''.join(lines), filename, lineno)
             self.swap_page(buf)
             return True
         return False
```

## mwx/wxpdb.py

```diff
@@ -175,24 +175,14 @@
     def stamp_where(self):
         """Stamp current where(frame) message."""
         ## cf. (print_stack_entry for frame in self.stack)
         self.send_input('w')
         if not self.verbose:
             self.message("--> {}".format(where(self.curframe)), indent=0)
     
-    def stamp_marker(self, lineno, style):
-        """Set a marker to lineno, with the following style markers:
-        [1] white-arrow for breakpoints
-        [2] red-arrow for exception
-        """
-        if lineno:
-            self.editor.buffer.MarkerAdd(lineno - 1, style)
-        else:
-            self.editor.buffer.MarkerDeleteAll(style)
-    
     def send_input(self, c, echo=False):
         """Send input:str (echo message if needed)."""
         def _send():
             self.stdin.input = c
             if echo or self.verbose:
                 self.message(c, indent=0)
         wx.CallAfter(_send)
@@ -246,15 +236,15 @@
         try:
             frame = inspect.currentframe().f_back
             self.set_trace(frame)
             obj(*args, **kwargs)
         except BdbQuit:
             pass
         except Exception as e:
-            ## Note: CallAfter to avoid crashing by a kill-focus event.
+            ## Note: post-call to avoid crashing by a kill-focus event.
             wx.CallAfter(wx.MessageBox,
                          "Debugger is closed.\n\n{}".format(e))
         finally:
             self.set_quit()
             return
     
     def run(self, cmd):
@@ -272,25 +262,36 @@
         try:
             frame = inspect.currentframe().f_back
             self.set_trace(frame)
             exec(cmd, globals, locals)
         except BdbQuit:
             pass
         except Exception as e:
-            ## Note: CallAfter to avoid crashing by a kill-focus event.
+            ## Note: post-call to avoid crashing by a kill-focus event.
             wx.CallAfter(wx.MessageBox,
                          "Debugger is closed.\n\n{}".format(e))
         finally:
             self.set_quit()
             return
     
     ## --------------------------------
     ## Actions for handler
     ## --------------------------------
     
+    def _markbp(self, lineno, style):
+        """Add a marker to lineno, with the following style markers:
+        [1] white-arrow for breakpoints
+        [2] red-arrow for exception
+        """
+        if self.editor:
+            if lineno:
+                self.editor.buffer.MarkerAdd(lineno - 1, style)
+            else:
+                self.editor.buffer.MarkerDeleteAll(style)
+    
     def find_editor(self, f):
         """Find parent editor which has the specified f:object,
         where `f` can be filename or code object.
         """
         for editor in self.parent.get_all_pages(type(self.editor)):
             buf = editor.find_buffer(f)
             if buf:
@@ -319,23 +320,26 @@
         if m:
             module = import_module(m.group(1))
             filename = inspect.getfile(module)
         
         editor = self.find_editor(code) or self.find_editor(filename)
         if not editor:
             editor = self.parent.Log
-            if filename != editor.buffer.filename:
-                ## editor.load_cache(filename)
-                wx.CallAfter(editor.load_cache, filename)
+            ## Note: Need a post-call for a thread debugging.
+            wx.CallAfter(editor.load_cache, filename)
         self.editor = editor
+        
+        if not self.interactive_shell.HasFocus():
+            self.editor.buffer.SetFocus()
+        
         for ln in self.get_file_breaks(filename):
-            self.stamp_marker(ln, 1) # (>>) bp:white-arrow
+            self._markbp(ln, 1) # (>>) bp:white-arrow
         
         def _mark():
-            buffer = editor.buffer
+            buffer = self.editor.buffer
             if filename == buffer.filename:
                 if code != self.code:
                     buffer.markline = firstlineno - 1 # (o) entry:marker
                     buffer.goto_marker(1)
                     buffer.recenter(3)
                 buffer.goto_line(lineno - 1)
                 buffer.pointer = lineno - 1 # (->) pointer:marker
@@ -454,15 +458,15 @@
             return
         if not frame:
             frame = inspect.currentframe().f_back
         self.handler('debug_begin', frame)
         Pdb.set_trace(self, frame)
     
     def set_break(self, filename, lineno, *args, **kwargs):
-        self.stamp_marker(lineno, 1)
+        self._markbp(lineno, 1)
         return Pdb.set_break(self, filename, lineno, *args, **kwargs)
     
     def set_quit(self):
         try:
             Pdb.set_quit(self)
         finally:
             if self.parent: # Check if Destroy has begun.
@@ -524,29 +528,29 @@
     @echo
     def user_exception(self, frame, exc_info):
         """--Exception--
         
         (override) Update exception:markers.
         """
         t, v, tb = exc_info
-        self.stamp_marker(tb.tb_lineno, 2)
+        self._markbp(tb.tb_lineno, 2)
         self.message(tb.tb_frame, indent=0)
         Pdb.user_exception(self, frame, exc_info)
     
     @echo
     def bp_commands(self, frame):
         """--Break--
         
         (override) Update breakpoint:markers every time the frame changes.
         """
         filename = frame.f_code.co_filename
         breakpoints = self.get_file_breaks(filename)
-        self.stamp_marker(None, 1)
+        self._markbp(None, 1)
         for lineno in breakpoints:
-            self.stamp_marker(lineno, 1)
+            self._markbp(lineno, 1)
         return Pdb.bp_commands(self, frame)
     
     @echo
     def preloop(self):
         """Hook method executed once when the cmdloop() method is called."""
         Pdb.preloop(self)
         self.handler('debug_next', self.curframe)
```

## Comparing `mwxlib-0.85.2.dist-info/LICENSE` & `mwxlib-0.85.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.85.2.dist-info/METADATA` & `mwxlib-0.85.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.85.2
+Version: 0.85.3
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.85.2.dist-info/RECORD` & `mwxlib-0.85.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=GjPK6XqLZANqXS0jY1YJyMo-UJrH60u-qkKA6ESw3QA,44266
-mwx/framework.py,sha256=oX3wi5-6UDS5qYpnsnaHlD22QT8W-cOuv41mh7pvUZg,72505
+mwx/framework.py,sha256=skYQkfX-Z1aAWJ5omiGmjXGHgKFcL2I_ZUw2s5pC9CI,72480
 mwx/graphman.py,sha256=vQAO19MyRFdAAQVyaGzEn-WJy5yrkQwtWNr7UKcHgT8,68631
 mwx/images.py,sha256=Xyvsq9m_R8JYERHA4Z3YznnUXbXkR7eUG7Cia1v1k2c,45726
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=vVlBulRQDyYonI9EKfqp-3SpNbGyIJQ6ldkw6bZlalo,27598
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=AZ2pv7-UBLqr7fAUW4lqaLfZT_UvLdyRSrtjqDCcN9c,139039
+mwx/nutshell.py,sha256=_GMnufsr6HLpAIBiWN7QAnn_hZKsAiHJIsoCPAE7o3U,139026
 mwx/utilus.py,sha256=PDEJhTfDlFrcOe5w6zmU5EHmAfqIDOu74fKewi1rybY,37369
 mwx/wxmon.py,sha256=xfbpsFz18oX4Fyfx0MM2qrZid-fQuAsxxof41Yn23LI,11670
-mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
+mwx/wxpdb.py,sha256=BKr8HVJQx8uC-yPS6am3ifD_sl89Ar-xEBi5scf7vm8,19456
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=MVpG18Ha6zi68cpQZleRC4qlpCZBmi4ogr9tOybqNXk,8196
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.85.2.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.85.2.dist-info/METADATA,sha256=wC7bNTzD4qQH_t8lOBG8mpapSJYLf44UYlmgIDub2Mo,1893
-mwxlib-0.85.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.85.2.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.85.2.dist-info/RECORD,,
+mwxlib-0.85.3.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.85.3.dist-info/METADATA,sha256=PSmyDugHmJtio1oItQ5bb16Y3yJazM5RrEi2c-_rmM0,1893
+mwxlib-0.85.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.85.3.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.85.3.dist-info/RECORD,,
```

