# Comparing `tmp/negar-gui-0.7.6.tar.gz` & `tmp/negar-gui-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negar-gui-0.7.6.tar", last modified: Mon May 15 16:20:31 2023, max compression
+gzip compressed data, was "negar-gui-0.7.7.tar", last modified: Tue Jun 13 07:38:06 2023, max compression
```

## Comparing `negar-gui-0.7.6.tar` & `negar-gui-0.7.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/
--rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.6/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.6/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-05-15 16:20:31.819549 negar-gui-0.7.6/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.6/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/
--rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/Ui_hwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.6/negar_gui/Ui_mwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.6/negar_gui/Ui_uwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)      257 2023-05-15 13:26:58.000000 negar-gui-0.7.6/negar_gui/constants.py
--rw-r--r--   0 javad     (1000) javad     (1000)    16208 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/gui.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/icons/
--rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.6/negar_gui/icons/logo.png
--rw-r--r--   0 javad     (1000) javad     (1000)    25360 2023-05-15 13:26:27.000000 negar-gui-0.7.6/negar_gui/main.py
--rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-05-15 13:23:51.000000 negar-gui-0.7.6/negar_gui/resource_rc.py
--rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.6/negar_gui/style.qss
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui/ts/
--rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.6/negar_gui/ts/fa.qm
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-05-15 16:20:31.819549 negar-gui-0.7.6/negar_gui.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       84 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-05-15 16:20:31.000000 negar-gui-0.7.6/negar_gui.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-05-15 16:20:31.819549 negar-gui-0.7.6/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1153 2023-04-01 17:20:04.000000 negar-gui-0.7.6/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/
+-rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.7/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.7/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-13 07:38:06.074695 negar-gui-0.7.7/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.7/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/Ui_hwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.7/negar_gui/Ui_mwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.7/negar_gui/Ui_uwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)      161 2023-06-13 07:28:43.000000 negar-gui-0.7.7/negar_gui/constants.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    14819 2023-06-13 06:56:14.000000 negar-gui-0.7.7/negar_gui/gui.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/icons/
+-rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.7/negar_gui/icons/logo.png
+-rw-r--r--   0 javad     (1000) javad     (1000)    25555 2023-06-13 07:07:34.000000 negar-gui-0.7.7/negar_gui/main.py
+-rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-06-13 07:26:58.000000 negar-gui-0.7.7/negar_gui/resource_rc.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/style.qss
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/ts/
+-rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.7/negar_gui/ts/fa.qm
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       91 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-06-13 07:38:06.074695 negar-gui-0.7.7/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1171 2023-06-13 07:27:29.000000 negar-gui-0.7.7/setup.py
```

### Comparing `negar-gui-0.7.6/LICENSE` & `negar-gui-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/PKG-INFO` & `negar-gui-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.6
+Version: 0.7.7
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿Negar-GUI
 ==============
 [![PyPI](https://img.shields.io/pypi/v/negar-gui?style=social)](https://pypi.org/project/negar-gui/)
 [![code size](https://img.shields.io/github/languages/code-size/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/archive/master.zip)
```

### Comparing `negar-gui-0.7.6/README.md` & `negar-gui-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/Ui_hwin.py` & `negar-gui-0.7.7/negar_gui/Ui_hwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/Ui_mwin.py` & `negar-gui-0.7.7/negar_gui/Ui_mwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/Ui_uwin.py` & `negar-gui-0.7.7/negar_gui/Ui_uwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/gui.py` & `negar-gui-0.7.7/negar_gui/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import sys
-from pyuca import Collator
 from pathlib import Path
+from pyuca import Collator
 from pyperclip import copy
 from PyQt5.QtGui import QIcon, QColor
 from PyQt5.QtCore import Qt, QAbstractTableModel, QSize
 from PyQt5.QtWidgets import (QApplication, QMainWindow, QPushButton, QTableView, QHeaderView, QCheckBox,
                             QSlider, QLabel, QTextEdit, QLineEdit, QGroupBox, QGridLayout, QTabWidget,
                             QWidget, QHBoxLayout, QVBoxLayout, QFileDialog)
 sys.path.append(Path(__file__).parent.parent.as_posix()) # https://stackoverflow.com/questions/16981921
@@ -15,15 +15,15 @@
 from negar_gui.constants import __version__, LOGO
 
 
 collator = Collator()
 
 class TableModel(QAbstractTableModel):
     def __init__(self, data):
-        super(TableModel, self).__init__()
+        super().__init__()
         self._data = data
 
     def data(self, index, role):
         if role == Qt.ItemDataRole.TextAlignmentRole:
             return Qt.AlignmentFlag.AlignVCenter
         if role == Qt.ItemDataRole.BackgroundRole:
             if index.row()%2:
@@ -32,35 +32,39 @@
             if index.row()%2:
                 return QColor('white')
         if role == Qt.ItemDataRole.DisplayRole:
             try:
                 return self._data[index.row()][index.column()]
             except:
                 return ''
+        return None
 
     def rowCount(self, index):
-        # The length of the outer list.
+        """The length of the outer list."""
+        del index
         return len(self._data)
 
     def columnCount(self, index):
-        # The following takes the first sub-list, and returns
-        # the length (only works if all rows are an equal length)
+        """The following takes the first sub-list, and returns
+        the length (only works if all rows are an equal length)"""
+        del index
         return len(self._data[0])
 
     def headerData(self, section, orientation, role):
         # section is the index of the column/row.
         if role == Qt.ItemDataRole.DisplayRole:
             if orientation == Qt.Orientation.Horizontal:
                 return ''
             if orientation == Qt.Orientation.Vertical:
                 return str(section+1)
+        return None
 
 class Form(QMainWindow):
     def __init__(self, parent = None):
-        super(Form, self).__init__(parent)
+        super().__init__(parent)
         self.editing_options = []
 
         self.table = QTableView(layoutDirection=Qt.LayoutDirection.RightToLeft,)
         self.setup_table()
 
         self.setupUi()
 
@@ -217,35 +221,25 @@
         self.autoedit_chkbox.stateChanged.connect(self.autoedit_handler)
 
         self.font_slider.valueChanged.connect(self._set_font_size)
         self.untouch_word.textChanged.connect(self.untouch_add_enabler)
         self.untouch_button.clicked.connect(self.untouch_add)
 
         # Option checkbox lists signal control
-        self.f_dashes.stateChanged.connect(self.option_control)
-        self.f_three_dots.stateChanged.connect(self.option_control)
-        self.f_english_quotes.stateChanged.connect(self.option_control)
-        self.f_hamzeh.stateChanged.connect(self.option_control)
-        self.hamzeh_yeh.stateChanged.connect(self.option_control)
-        self.f_spacing_bq.stateChanged.connect(self.option_control)
-        self.f_arab_num.stateChanged.connect(self.option_control)
-        self.f_eng_num.stateChanged.connect(self.option_control)
-        self.f_non_persian_ch.stateChanged.connect(self.option_control)
-        self.f_p_spacing.stateChanged.connect(self.option_control)
-        self.f_p_separate.stateChanged.connect(self.option_control)
-        self.f_s_spacing.stateChanged.connect(self.option_control)
-        self.f_s_separate.stateChanged.connect(self.option_control)
-        self.aggressive.stateChanged.connect(self.option_control)
-        self.clnup_kashidas.stateChanged.connect(self.option_control)
-        self.clnup_ex_marks.stateChanged.connect(self.option_control)
-        self.clnup_spacing.stateChanged.connect(self.option_control)
-        self.trim_lt_whitespaces.stateChanged.connect(self.option_control)
-        self.exaggeragin_zwnj.stateChanged.connect(self.option_control)
+        _options = [self.f_dashes, self.f_three_dots, self.f_english_quotes, self.f_hamzeh,
+                    self.hamzeh_yeh, self.f_spacing_bq, self.f_arab_num, self.f_eng_num,
+                    self.f_non_persian_ch, self.f_p_spacing, self.f_p_separate, self.f_s_spacing,
+                    self.f_s_separate, self.aggressive, self.clnup_kashidas, self.clnup_ex_marks,
+                    self.clnup_spacing, self.trim_lt_whitespaces, self.exaggeragin_zwnj
+                    ]
+        for opt in _options:
+            opt.stateChanged.connect(self.option_control)
 
     def keyPressEvent(self, event):
+        """KeyPress event handler"""
         if event.key() == Qt.Key.Key_Escape:
             self.save_to_clipboard()
             self.close()
         elif event.key() == Qt.Key.Key_F1:
             self.input_editor.clear()
             self.input_editor.setText(INFO)
         else:
@@ -290,72 +284,50 @@
     def text_box_reset(self):
         """Clears input/output editor boxes"""
         self.input_editor.clear()
         self.output_editor.clear()
 
     def option_control(self):
         """Enable/Disable Editing features"""
-        if not self.f_dashes.isChecked():
-            self.editing_options.append("fix-dashes")
-        if not self.f_three_dots.isChecked():
-            self.editing_options.append("fix-three-dots")
-        if not self.f_english_quotes.isChecked():
-            self.editing_options.append("fix-english-quotes")
-        if not self.f_hamzeh.isChecked():
-            self.editing_options.append("fix-hamzeh")
-        if not self.hamzeh_yeh.isChecked():
-            self.editing_options.append("hamzeh-with-yeh")
-        if not self.f_spacing_bq.isChecked():
-            self.editing_options.append("fix-spacing-bq")
-        if not self.f_arab_num.isChecked():
-            self.editing_options.append("fix-arabic-num")
-        if not self.f_eng_num.isChecked():
-            self.editing_options.append("fix-english-num")
-        if not self.f_non_persian_ch.isChecked():
-            self.editing_options.append("fix-non-persian-chars")
-        if not self.f_p_spacing.isChecked():
-            self.editing_options.append("fix-p-spacing")
-        if not self.f_p_separate.isChecked():
-            self.editing_options.append("fix-p-separate")
-        if not self.f_s_spacing.isChecked():
-            self.editing_options.append("fix-s-spacing")
-        if not self.f_s_separate.isChecked():
-            self.editing_options.append("fix-s-separate")
-        if not self.aggressive.isChecked():
-            self.editing_options.append("aggressive")
-        if not self.clnup_kashidas.isChecked():
-            self.editing_options.append("cleanup-kashidas")
-        if not self.clnup_ex_marks.isChecked():
-            self.editing_options.append("cleanup-ex-marks")
-        if not self.clnup_spacing.isChecked():
-            self.editing_options.append("cleanup-spacing")
-        if not self.trim_lt_whitespaces.isChecked():
-            self.editing_options.append("trim-lt-whitespaces")
-        if not self.exaggeragin_zwnj.isChecked():
-            self.editing_options.append("exaggerating-zwnj")
+        options = [(self.f_dashes, "fix-dashes"), (self.f_three_dots, "fix-three-dots"),
+                    (self.f_english_quotes, "fix-english-quotes"), (self.f_hamzeh, "fix-hamzeh"),
+                    (self.hamzeh_yeh, "hamzeh-with-yeh"), (self.f_spacing_bq, "fix-spacing-bq"),
+                    (self.f_arab_num, "fix-arabic-num"), (self.f_eng_num, "fix-english-num"),
+                    (self.f_non_persian_ch, "fix-non-persian-chars"), (self.f_p_spacing, "fix-p-spacing"),
+                    (self.f_p_separate, "fix-p-separate"), (self.f_s_spacing, "fix-s-spacing"),
+                    (self.f_s_separate, "fix-s-separate"), (self.aggressive, "aggressive"),
+                    (self.clnup_kashidas, "cleanup-kashidas"), (self.clnup_ex_marks, "cleanup-ex-marks"),
+                    (self.clnup_spacing, "cleanup-spacing"), (self.trim_lt_whitespaces, "trim-lt-whitespaces"),
+                    (self.exaggeragin_zwnj, "exaggerating-zwnj")]
+        for obj, opt in options:
+            if not obj.isChecked(): self.editing_options.append(opt)
 
     def file_dialog(self):
+        """Open file for importing text."""
         fname, _ = QFileDialog.getOpenFileName(self, 'Open File - A Plain Text')
         try:
-            with open(fname, 'r', encoding="utf8") as f:
-                self.input_editor.setText(f.read())
+            with open(fname, 'r', encoding="utf8") as file_:
+                self.input_editor.setText(file_.read())
         except:
             pass
 
     def edit_text(self):
+        """Edit input text"""
         self.output_editor.clear()
-        run_PE = PersianEditor(self.input_editor.toPlainText(), *self.editing_options)
-        self.output_editor.append(run_PE.cleanup())
+        persian_editor = PersianEditor(self.input_editor.toPlainText(), *self.editing_options)
+        self.output_editor.append(persian_editor.cleanup())
 
     def save_to_clipboard(self):
-        sanitizedText = self.output_editor.toPlainText()
-        if sanitizedText:
-            copy(sanitizedText)
+        """Save edited text to clipboard"""
+        sanitized_text = self.output_editor.toPlainText()
+        if sanitized_text:
+            copy(sanitized_text)
 
 def main():
+    """Program entry point"""
     app = QApplication(sys.argv)
     run = Form()
     run.show()
     run.input_editor.setFocus() # set focus on input box
     sys.exit(app.exec())
 
 if __name__ == "__main__":
```

### Comparing `negar-gui-0.7.6/negar_gui/icons/logo.png` & `negar-gui-0.7.7/negar_gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/main.py` & `negar-gui-0.7.7/negar_gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 Options:
     -h, --help          Show this screen.
     -v, --version       Show version and exit
 '''
 
 import re
 import sys
-from docopt import docopt
 import asyncio
-import requests
-from threading import Thread
 from pathlib import Path
+from threading import Thread
 import tempfile
+from docopt import docopt
+import requests
 from pyuca import Collator
 from pyperclip import copy as pyclipcopy
 from qrcode import QRCode, ERROR_CORRECT_L
 from PyQt5.QtCore import QTranslator, QUrl, Qt, QAbstractTableModel, QTimer
 from PyQt5.QtWidgets import QApplication, QMainWindow, QFileDialog, QHeaderView, QDialog
 from PyQt5.QtGui import QDesktopServices, QIcon, QColor, QPixmap
 import qdarktheme
 
-sys.path.append(Path(__file__).parent.parent.as_posix()) # https://stackoverflow.com/questions/16981921
+# https://stackoverflow.com/questions/16981921
+sys.path.append(Path(__file__).parent.parent.as_posix())
 from negar.virastar import PersianEditor, UnTouchable
 from negar.constants import INFO, __version__ as negar__version
 from negar_gui.constants import __version__, LOGO
 from negar_gui.Ui_mwin import Ui_MainWindow
 from negar_gui.Ui_uwin import Ui_uwWindow
 from negar_gui.Ui_hwin import Ui_Dialog
 
@@ -48,37 +49,29 @@
 
 collator = Collator()
 
 def init_decorator(func):
     def wrapper(*args, **kwargs):
         func(*args, **kwargs)
         self, parent = args[0], kwargs.pop('parent', None)
-        # it adjusts Frame Size maximized if its height or width would be bigger than its counterpart on the real screen
+        # Maximize Frame Size if either height or width exceeds real screen dimensionsq
         screen = QApplication.desktop().screenGeometry()
         h, w = screen.height(), screen.width()
         if self.width() > w or self.height() > h:
             self.showMaximized()
         # set layout direction automatically
         if parent:
             try:
                 self.centralwidget.setLayoutDirection(parent.layoutDirection())
             except: # QDialog  has no centralwidget
                 pass
         # connect widgets to their proper slot
         self.connectSlots()
     return wrapper
 
-def checkScreenSize(window):
-    """it adjusts Frame Size maximized
-    if its height or width would be bigger than its counterpart on the real screen"""
-    screen = QApplication.desktop().screenGeometry()
-    h, w = screen.height(), screen.width()
-    if window.width() > w or window.height() > h:
-        window.showMaximized()
-
 class TableModel(QAbstractTableModel):
     def __init__(self, data):
         super(TableModel, self).__init__()
         self._data = data
 
     def data(self, index, role):
         if role == Qt.ItemDataRole.TextAlignmentRole:
@@ -92,35 +85,38 @@
         if role == Qt.ItemDataRole.DisplayRole:
             try:
                 return self._data[index.row()][index.column()]
             except:
                 return ''
 
     def rowCount(self, index):
-        # The length of the outer list.
+        """The length of the outer list."""
+        del index
         return len(self._data)
 
     def columnCount(self, index):
-        # The following takes the first sub-list, and returns
-        # the length (only works if all rows are an equal length)
+        """The following takes the first sub-list, and returns
+        the length (only works if all rows are an equal length)"""
+        del index
         return len(self._data[0])
 
     def headerData(self, section, orientation, role):
-        # section is the index of the column/row.
+        """section is the index of the column/row."""
         if role == Qt.ItemDataRole.DisplayRole:
             if orientation == Qt.Orientation.Horizontal:
                 return ''
             if orientation == Qt.Orientation.Vertical:
                 return str(section+1)
+        return None
 
 class UntouchWindow(QMainWindow, Ui_uwWindow):
     @init_decorator
     def __init__(self, parent=None):
         self.parent = parent
-        super(UntouchWindow, self).__init__(parent)
+        super().__init__(parent)
         self.setupUi(self)
         self.setup_table()
         # if parent: self.centralwidget.setLayoutDirection(parent.layoutDirection())
 
     def setup_table(self, col=8):
         self.untouch_table.horizontalHeader().setSectionResizeMode(QHeaderView.ResizeMode.Stretch)
         data = sorted(list(UnTouchable().get()), key=collator.sort_key)
@@ -129,15 +125,15 @@
         self.untouch_table.setModel(model)
 
     def connectSlots(self):
         self.untouch_word.textChanged.connect(self.untouch_add_enabler)
         self.untouch_button.clicked.connect(self.untouch_add)
 
     def untouch_add_enabler(self):
-        """Checks untouchable word text input to enable the `Add` button if just one word is typed."""
+        """Enable `Add` button when a single word is entered in the untouchable text input."""
         word_list = self.untouch_word.text().split()
         self.untouch_button.setEnabled(len(word_list) == 1)
 
     def untouch_add(self):
         """Adds a new word into untouchable words"""
         word = [self.untouch_word.text().strip()]
         UnTouchable.add(word)
@@ -152,23 +148,24 @@
                 self.showNormal()
             else:
                 self.showMaximized()
         else:
             super().keyPressEvent(event)
 
     def closeEvent(self, event):
+        del event
         if self.parent:
             self.parent.show()
             self.parent.edit_text()
 
 class HelpWindow(QDialog, Ui_Dialog):
     @init_decorator
     def __init__(self, parent=None, title=None, label=None):
         self.parent = parent
-        super(HelpWindow, self).__init__(parent)
+        super().__init__(parent)
         self.setupUi(self)
         self.setWindowTitle(title)
         if isinstance(label, str):
             self.label.setText(label)
         if isinstance(label, QPixmap):
             self.label.setPixmap(label)
             # self.setFixedSize(QSize(600,600))
@@ -182,39 +179,41 @@
         else:
             super().keyPressEvent(event)
 
 
 class MyWindow(QMainWindow, Ui_MainWindow):
     @init_decorator
     def __init__(self, parent=None):
-        super(MyWindow, self).__init__(parent)
+        super().__init__(parent)
         self.setupUi(self)
         self.input_editor.setStyleSheet("border: 1px solid #d89e76;")
         self.output_editor.setStyleSheet("border: 1px solid #d89e76;")
         self.setWindowIcon(QIcon(LOGO))
         self.input_editor.setFocus(True)
         #  Translator
         self.trans = QTranslator()
         # destination language
         self.dest = "en"
         # ui language : 0->en, 1->fa
         self.lang = 'English'
         self.editing_options = []
         self.clipboard = QApplication.clipboard()
         self.fileDialog = QFileDialog()
+        self.filename = None # will be defined later
         self._statusBar()
         # Checks for new release
         Thread(target=lambda: asyncio.run(self.updateCheck()), daemon=True).start()
 
     async def updateCheck(self):
         nurl  = 'https://raw.github.com/shahinism/python-negar/master/negar/constants.py'
         ngurl = 'https://raw.github.com/javadr/negar-gui/master/negar_gui/constants.py'
         async def get(link):
             with requests.get(link) as response:
-                return re.search(r'(__version__ = "(\d\.\d(\.\d+)?)")', response.text, re.M).group(2)
+                VERSION_PATTERN = r'(__version__ = "(\d\.\d(\.\d+)?)")'
+                return re.search(VERSION_PATTERN, response.text, re.M).group(2)
         try:
             requests.get('https://github.com') # check the internet connection
             negar_t = asyncio.create_task(get(nurl))
             negargui_t = asyncio.create_task(get(ngurl))
             negar_v = await negar_t
             negargui_v = await negargui_t
         except:
@@ -247,52 +246,72 @@
             lambda: (self.font_slider.setValue(self.font_slider.value()-1), self._set_font_size())
         )
         self.actionPersian.triggered.connect(lambda: self.changeLanguage('Persian'))
         self.actionEnglish.triggered.connect(lambda: self.changeLanguage('English'))
 
         self.actionNegar_Help.triggered.connect(lambda: self.input_editor.setText(INFO) )
         self.actionAbout_Negar.setShortcut("CTRL+H")
-        self.actionAbout_Negar.triggered.connect(
-            lambda: (HelpWindow(parent=self, title='About Negar', label=self.edit_text(INFO)).show())
+        self.actionAbout_Negar.triggered.connect(lambda:
+            (HelpWindow(parent=self, title='About Negar', label=self.edit_text(INFO)).show())
         )
         self.actionAbout_Negar_GUI.triggered.connect(
             lambda: QDesktopServices.openUrl(QUrl("https://github.com/javadr/negar-gui"))
         )
         self.actionDonate.triggered.connect(
             lambda: QDesktopServices.openUrl(QUrl("https://github.com/javadr/negar-gui#donation"))
         )
         self.actionReport_Bugs.triggered.connect(
             lambda: QDesktopServices.openUrl(QUrl("https://github.com/javadr/negar-gui/issues"))
         )
-        self.actionFix_Dashes.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_three_dots.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_English_quotes.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_hamzeh.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionUse_Persian_yeh_to_show_hamzeh.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_spacing_braces_and_quotes.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_Arabic_numbers.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_English_numbers.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_non_Persian_chars.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_prefix_spacing.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_prefix_separating.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_suffix_spacing.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_suffix_separating.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionFix_aggressive_punctuation.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionCleanup_kashidas.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionCleanup_extra_marks.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionCleanup_spacing.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionTrim_Leading_Trailing_Whitespaces.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-        self.actionExaggerating_ZWNJ.triggered.connect(lambda: (self.option_control(), self.autoedit_handler()))
-
-        self.actionUntouchable_Words.triggered.connect(lambda: (UntouchWindow(parent=self).show(), MainWindow.hide()))
-        self.actionCopy.triggered.connect(self.copySlot)
-        self.copy_btn.clicked.connect(self.copySlot)
+        self.actionFix_Dashes.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_three_dots.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_English_quotes.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_hamzeh.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionUse_Persian_yeh_to_show_hamzeh.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_spacing_braces_and_quotes.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_Arabic_numbers.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_English_numbers.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_non_Persian_chars.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_prefix_spacing.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_prefix_separating.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_suffix_spacing.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_suffix_separating.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionFix_aggressive_punctuation.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionCleanup_kashidas.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionCleanup_extra_marks.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionCleanup_spacing.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionTrim_Leading_Trailing_Whitespaces.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionExaggerating_ZWNJ.triggered.connect(
+            lambda: (self.option_control(), self.autoedit_handler()))
+        self.actionUntouchable_Words.triggered.connect(
+            lambda: (UntouchWindow(parent=self).show(), MAIN_WINDOW.hide()))
+        self.actionCopy.triggered.connect(self.copy_slot)
+        self.copy_btn.clicked.connect(self.copy_slot)
 
         self.actionInteractive_Clipboard.triggered.connect(lambda:
-            self.clipboard.dataChanged.connect(self.onClipboardChanged) if self.actionInteractive_Clipboard.isChecked()
+            self.clipboard.dataChanged.connect(self.onClipboardChanged)
+            if self.actionInteractive_Clipboard.isChecked()
             else self.clipboard.dataChanged.disconnect(self.onClipboardChanged))
         self.actionQr_Code.triggered.connect(self.qrcode)
 
         # Change GridLayout Orientation
         def grid_layout(layout='h'):
             if layout=='v':
                 self.gridLayout.setHorizontalSpacing(5)
@@ -313,16 +332,18 @@
                 (1, 0, 1, 2),  # Position: 1x0 1 rowspan 2 colspan
                 (2, 0, 1, 2),  # Position: 2x0 1 rowspan 2 colspan
                 (3, 0, 1, 2),  # Position: 3x0 1 rowspan 2 colspan
             )
             for i, widget in enumerate(widgets):
                 self.gridLayout.addWidget(widget, *elements[i])
 
-        self.vertical_btn.clicked.connect(lambda: (self.actionSide_by_Side_View.setChecked(True), grid_layout('v')) )
-        self.horizontal_btn.clicked.connect(lambda: (self.actionSide_by_Side_View.setChecked(False), grid_layout('h')) )
+        self.vertical_btn.clicked.connect(
+            lambda: (self.actionSide_by_Side_View.setChecked(True), grid_layout('v')) )
+        self.horizontal_btn.clicked.connect(
+            lambda: (self.actionSide_by_Side_View.setChecked(False), grid_layout('h')) )
         self.actionSide_by_Side_View.triggered.connect(lambda:
             grid_layout('v') if self.actionSide_by_Side_View.isChecked() else grid_layout('h'))
 
         def grid_full_input():
             widgets = (self.output_editor_label, self.output_editor)
             for widget in widgets:
                 self.gridLayout.removeWidget(widget)
@@ -342,17 +363,17 @@
             },) )
         self.action_Light.triggered.connect(lambda: qdarktheme.setup_theme("light") )
         self.action_Auto.triggered.connect(lambda: qdarktheme.setup_theme("auto") )
 
     def qrcode(self):
         if len(self.output_editor.toPlainText().strip())==0:
             if self.lang == 'Persian':
-                statusBar_Timeout(self, 'هیچ متنی برای نمایش از طریق کد QR وجود ندارد!')
+                statusbar_timeout(self, 'هیچ متنی برای نمایش از طریق کد QR وجود ندارد!')
             else: # English
-                statusBar_Timeout(self, 'There is no text to be fed to the QR Code!')
+                statusbar_timeout(self, 'There is no text to be fed to the QR Code!')
             return
         qr = QRCode(
             version = 1,
             error_correction = ERROR_CORRECT_L,
             box_size = 10,
             border = 4
         )
@@ -366,54 +387,55 @@
         w = min(screen.height(), screen.width())
         if w-90 < img.size[0]:
             pixmap = pixmap.scaled(w-90, w-90, Qt.KeepAspectRatio)
         HelpWindow(parent=self, title='QR Code', label=pixmap).show()
         (Path(temp_path)/'negar-gui_qrcode.png').unlink()
 
     def _statusBar(self, notification='', timeout=0):
-        self.statusBar.showMessage(f'Negar v{negar__version} [[Negar-GUI v{__version__}]] {notification}', timeout)
+        message = f'Negar v{negar__version} [[Negar-GUI v{__version__}]] {notification}'
+        self.statusBar.showMessage(message, timeout)
 
     def openFileSlot(self):
         filename, _ = self.fileDialog.getOpenFileName(self, "Open File - A Plain Text", ".")
         if filename:
             with open(filename, encoding="utf-8") as f:
                 try:
                     self.input_editor.setPlainText(str(f.read()))
                     self.filename = Path(filename)
-                    MainWindow.setWindowTitle(f"Negar - {self.filename.name}")
-                    statusBar_Timeout(self,'File Opened.')
+                    MAIN_WINDOW.setWindowTitle(f"Negar - {self.filename.name}")
+                    statusbar_timeout(self,'File Opened.')
                 except Exception as e:
                     self.input_editor.setPlainText(e.args[1])
 
     def saveFileSlot(self):
         if not self.output_editor.toPlainText():
             return
         if hasattr(self, 'filename') and self.filename:
             with open(self.filename, "w", encoding="utf-8") as f:
                 try:
                     f.write(self.output_editor.toPlainText())
-                    statusBar_Timeout(self,'File Saved.')
+                    statusbar_timeout(self,'File Saved.')
                 except Exception as e:
                     self.output_editor.setPlainText(e.args[1])
         else:
             self.exportFileSlot()
 
     def exportFileSlot(self):
         if not self.output_editor.toPlainText():
             return
         filename, _ = self.fileDialog.getSaveFileName(self, "Save File", ".")
         if filename:
             with open(filename, "w", encoding="utf-8") as f:
                 try:
                     f.write(self.output_editor.toPlainText())
                     self.filename = Path(filename)
-                    MainWindow.setWindowTitle(f"Negar - {self.filename.name}")
-                    statusBar_Timeout(self,'File Saved.')
-                except Exception as e:
-                    self.output_editor.setPlainText(e.args[1])
+                    MAIN_WINDOW.setWindowTitle(f"Negar - {self.filename.name}")
+                    statusbar_timeout(self,'File Saved.')
+                except Exception as exception:
+                    self.output_editor.setPlainText(exception.args[1])
 
     def changeLanguage(self, lang):
         """
         change ui language
         """
         if lang=='Persian' and self.lang!='Persian':
             self.lang = 'Persian'
@@ -437,30 +459,31 @@
     # def retranslateUi(self, MyWindow):
         # super(MyWindow, self).retranslateUi()
         # _translate = QtCore.QCoreApplication.translate
         # print(dir(self))
         # MyWindow.fileDialog.setText(_translate(self.fileDialog.name(), "Open File - A Plain Text"))
         # pass
 
-    def copySlot(self):
-        s = self.output_editor.toPlainText()
-        if s:
-            QApplication.clipboard().setText(s)
-        return s
+    def copy_slot(self):
+        output = self.output_editor.toPlainText()
+        if output:
+            QApplication.clipboard().setText(output)
+        return output
 
     def onClipboardChanged(self):
         text = self.clipboard.text()
         if text:
             self.input_editor.setPlainText(text)
             self._set_font_size()
 
     def closeEvent(self, event):
+        del event
         # event = QEvent(QEvent.Clipboard)
         # QApplication.sendEvent(QApplication.clipboard(), event)
-        pyclipcopy(self.copySlot())
+        pyclipcopy(self.copy_slot())
 
     def keyPressEvent(self, event):
         if event.key() == Qt.Key.Key_Escape:
             self.close()
         elif event.key() == Qt.Key.Key_F11:
             if self.isMaximized():
                 self.showNormal()
@@ -469,15 +492,15 @@
         else:
             super().keyPressEvent(event)
 
     def wheelEvent(self, event):
         modifiers = QApplication.keyboardModifiers()
         if modifiers == Qt.ControlModifier:
             delta_notches = int(event.angleDelta().y() / 120)
-            self.font_slider.setValue(self.font_slider.value()+delta_notches),
+            self.font_slider.setValue(self.font_slider.value()+delta_notches)
             self._set_font_size()
 
     def autoedit_handler(self):
         """Edits the input text automatically if `autoedit` is checked."""
         if self.autoedit_chkbox.isChecked():
             self.edit_btn.setEnabled(False)
             self.input_editor.textChanged.connect(self.edit_text)
@@ -493,16 +516,16 @@
         self.output_editor.setFontPointSize(size)
         lines = self.input_editor.toPlainText()
         self.input_editor.clear()
         self.input_editor.append(lines)
         self.edit_text()
 
     def option_control(self):
-        self.editing_options = []
         """Enable/Disable Editing features"""
+        self.editing_options = []
         if not self.actionFix_Dashes.isChecked():
             self.editing_options.append("fix-dashes")
         if not self.actionFix_three_dots.isChecked():
             self.editing_options.append("fix-three-dots")
         if not self.actionFix_English_quotes.isChecked():
             self.editing_options.append("fix-english-quotes")
         if not self.actionFix_hamzeh.isChecked():
@@ -537,36 +560,36 @@
             self.editing_options.append("trim-lt-whitespaces")
         if not self.actionExaggerating_ZWNJ.isChecked():
             self.editing_options.append("exaggerating-zwnj")
 
     def edit_text(self, text=None):
         if not text:
             self.output_editor.clear()
-            run_PE = PersianEditor(self.input_editor.toPlainText(), *self.editing_options)
-            self.output_editor.append(run_PE.cleanup())
+            persian_editor = PersianEditor(self.input_editor.toPlainText(), *self.editing_options)
+            self.output_editor.append(persian_editor.cleanup())
         else:
             return PersianEditor(text, *self.editing_options).cleanup()
 
 
-def statusBar_Timeout(self, notification, timeout=5000): # Timeout in milliseconds
+def statusbar_timeout(self, notification, timeout=5000): # Timeout in milliseconds
     self.statusBar.showMessage(notification, timeout)
     timer = QTimer()
     timer.setSingleShot( True )
     timer.timeout.connect( self.statusBar.clearMessage )
     timer.start(timeout)
 
 def main(args=docopt(__doc__)):
-
+    """Program entry point"""
     if args['--version']:
         print (f"negar-gui, Version {__version__}")
         sys.exit()
 
-    global MainWindow
+    global MAIN_WINDOW
     qdarktheme.enable_hi_dpi()
     app = QApplication(sys.argv)
     qdarktheme.setup_theme("dark")
-    MainWindow = MyWindow()
-    MainWindow.show()
+    MAIN_WINDOW = MyWindow()
+    MAIN_WINDOW.show()
     sys.exit(app.exec_())
 
 if __name__ == "__main__":
     main()
```

### Comparing `negar-gui-0.7.6/negar_gui/resource_rc.py` & `negar-gui-0.7.7/negar_gui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/style.qss` & `negar-gui-0.7.7/negar_gui/style.qss`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui/ts/fa.qm` & `negar-gui-0.7.7/negar_gui/ts/fa.qm`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.6/negar_gui.egg-info/PKG-INFO` & `negar-gui-0.7.7/negar_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.6
+Version: 0.7.7
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿Negar-GUI
 ==============
 [![PyPI](https://img.shields.io/pypi/v/negar-gui?style=social)](https://pypi.org/project/negar-gui/)
 [![code size](https://img.shields.io/github/languages/code-size/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/archive/master.zip)
```

### Comparing `negar-gui-0.7.6/setup.py` & `negar-gui-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,26 @@
     name="negar-gui",
     version=version,
     author="Javad Razavian",
     author_email="javadr@gmail.com",
     include_package_data=True,
     packages=['negar_gui',],
     install_requires=[
-        'python-negar>=1.1.4',
+        'python-negar>=1.2.2',
         'PyQt5',
         'pyperclip',
         'pyuca',
         'regex',
         'requests',
         'qrcode',
+        'docopt',
         'Image',
         'pyqtdarktheme'
     ],
-    python_requires=">=3.5",
+    python_requires=">=3.6",
     package_dir={'negar_gui': 'negar_gui'},
     description="Graphical User Interface for Negar -- Persian Text Editor",
     license="GPLv3",
     keywords="Spellcheck Persian Text-Editor",
     url="http://github.com/javadr/negar-gui",
     entry_points={
         'console_scripts': [
```

