# Comparing `tmp/guitk-0.4.2.tar.gz` & `tmp/guitk-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitk-0.4.2.tar", max compression
+gzip compressed data, was "guitk-0.4.3.tar", max compression
```

## Comparing `guitk-0.4.2.tar` & `guitk-0.4.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.4.2/LICENSE
--rw-r--r--   0        0        0    10040 2023-06-12 13:30:09.123098 guitk-0.4.2/README.md
--rw-r--r--   0        0        0     2880 2023-06-12 13:30:09.124344 guitk-0.4.2/guitk/__init__.py
--rw-r--r--   0        0        0    12161 2023-06-05 13:44:42.707599 guitk-0.4.2/guitk/__main__.py
--rw-r--r--   0        0        0     1968 2023-06-05 13:44:42.707839 guitk-0.4.2/guitk/_debug.py
--rw-r--r--   0        0        0     2430 2023-06-05 13:44:42.708070 guitk-0.4.2/guitk/_on.py
--rw-r--r--   0        0        0    10707 2023-06-05 13:44:42.708422 guitk-0.4.2/guitk/basewidget.py
--rw-r--r--   0        0        0      317 2023-06-12 13:27:03.430985 guitk-0.4.2/guitk/constants.py
--rw-r--r--   0        0        0    24190 2023-06-05 13:44:42.709103 guitk-0.4.2/guitk/containers.py
--rw-r--r--   0        0        0     1306 2023-06-05 13:44:42.709339 guitk-0.4.2/guitk/debugwindow.py
--rw-r--r--   0        0        0     2437 2023-06-11 15:11:10.947825 guitk-0.4.2/guitk/events.py
--rw-r--r--   0        0        0    22563 2023-06-05 13:44:42.709859 guitk-0.4.2/guitk/frame.py
--rw-r--r--   0        0        0     4723 2023-06-05 13:44:42.710063 guitk-0.4.2/guitk/image.py
--rw-r--r--   0        0        0     5510 2023-06-05 13:44:42.710655 guitk-0.4.2/guitk/layout.py
--rw-r--r--   0        0        0    17405 2023-06-12 13:27:03.431329 guitk-0.4.2/guitk/menu.py
--rw-r--r--   0        0        0     2873 2023-06-05 13:44:42.711259 guitk-0.4.2/guitk/redirect.py
--rw-r--r--   0        0        0     1618 2023-06-05 13:44:42.711438 guitk-0.4.2/guitk/spacer.py
--rw-r--r--   0        0        0    11449 2023-06-05 13:44:42.711640 guitk-0.4.2/guitk/tk_text.py
--rw-r--r--   0        0        0     2523 2023-06-05 13:44:42.712010 guitk-0.4.2/guitk/tkroot.py
--rw-r--r--   0        0        0     8686 2023-06-05 13:44:42.712276 guitk-0.4.2/guitk/tooltips.py
--rw-r--r--   0        0        0    13189 2023-06-11 02:55:57.103304 guitk-0.4.2/guitk/ttk_button.py
--rw-r--r--   0        0        0     5088 2023-06-05 13:44:42.712731 guitk-0.4.2/guitk/ttk_checkbutton.py
--rw-r--r--   0        0        0     5717 2023-06-05 13:44:42.713001 guitk-0.4.2/guitk/ttk_combobox.py
--rw-r--r--   0        0        0    10384 2023-06-05 13:44:42.713197 guitk-0.4.2/guitk/ttk_entry.py
--rw-r--r--   0        0        0     7596 2023-06-05 13:44:42.713434 guitk-0.4.2/guitk/ttk_label.py
--rw-r--r--   0        0        0     8873 2023-06-05 13:44:42.713652 guitk-0.4.2/guitk/ttk_notebook.py
--rw-r--r--   0        0        0     8883 2023-06-05 13:44:42.714581 guitk-0.4.2/guitk/ttk_panedwindow.py
--rw-r--r--   0        0        0     4898 2023-06-05 13:44:42.714718 guitk-0.4.2/guitk/ttk_progressbar.py
--rw-r--r--   0        0        0     6148 2023-06-05 13:44:42.714850 guitk-0.4.2/guitk/ttk_radiobutton.py
--rw-r--r--   0        0        0     7161 2023-06-05 13:44:42.714992 guitk-0.4.2/guitk/ttk_scale.py
--rw-r--r--   0        0        0     2943 2023-06-05 13:44:42.715116 guitk-0.4.2/guitk/ttk_separator.py
--rw-r--r--   0        0        0     7801 2023-06-05 13:44:42.715319 guitk-0.4.2/guitk/ttk_spinbox.py
--rw-r--r--   0        0        0    12619 2023-06-05 13:44:42.715472 guitk-0.4.2/guitk/ttk_treeview.py
--rw-r--r--   0        0        0      771 2023-06-05 13:44:42.715589 guitk-0.4.2/guitk/types.py
--rw-r--r--   0        0        0     2527 2023-06-05 13:44:42.715787 guitk-0.4.2/guitk/utils.py
--rw-r--r--   0        0        0     9333 2023-06-05 13:44:42.716003 guitk-0.4.2/guitk/widget.py
--rw-r--r--   0        0        0    19055 2023-06-12 13:27:03.431732 guitk-0.4.2/guitk/window.py
--rw-r--r--   0        0        0      804 2023-06-12 13:30:09.124615 guitk-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    10884 1970-01-01 00:00:00.000000 guitk-0.4.2/setup.py
--rw-r--r--   0        0        0    10612 1970-01-01 00:00:00.000000 guitk-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.4.3/LICENSE
+-rw-r--r--   0        0        0     9921 2023-06-13 04:50:05.012686 guitk-0.4.3/README.md
+-rw-r--r--   0        0        0     2880 2023-06-13 04:49:55.834428 guitk-0.4.3/guitk/__init__.py
+-rw-r--r--   0        0        0    12978 2023-06-13 04:49:09.140363 guitk-0.4.3/guitk/__main__.py
+-rw-r--r--   0        0        0     1968 2023-06-13 04:47:03.739131 guitk-0.4.3/guitk/_debug.py
+-rw-r--r--   0        0        0     2430 2023-06-05 13:44:42.708070 guitk-0.4.3/guitk/_on.py
+-rw-r--r--   0        0        0    10707 2023-06-05 13:44:42.708422 guitk-0.4.3/guitk/basewidget.py
+-rw-r--r--   0        0        0      317 2023-06-12 13:27:03.430985 guitk-0.4.3/guitk/constants.py
+-rw-r--r--   0        0        0    24190 2023-06-05 13:44:42.709103 guitk-0.4.3/guitk/containers.py
+-rw-r--r--   0        0        0     1306 2023-06-05 13:44:42.709339 guitk-0.4.3/guitk/debugwindow.py
+-rw-r--r--   0        0        0     2437 2023-06-11 15:11:10.947825 guitk-0.4.3/guitk/events.py
+-rw-r--r--   0        0        0    22563 2023-06-05 13:44:42.709859 guitk-0.4.3/guitk/frame.py
+-rw-r--r--   0        0        0     4723 2023-06-05 13:44:42.710063 guitk-0.4.3/guitk/image.py
+-rw-r--r--   0        0        0     5510 2023-06-05 13:44:42.710655 guitk-0.4.3/guitk/layout.py
+-rw-r--r--   0        0        0    17405 2023-06-12 13:27:03.431329 guitk-0.4.3/guitk/menu.py
+-rw-r--r--   0        0        0     2873 2023-06-05 13:44:42.711259 guitk-0.4.3/guitk/redirect.py
+-rw-r--r--   0        0        0     1618 2023-06-05 13:44:42.711438 guitk-0.4.3/guitk/spacer.py
+-rw-r--r--   0        0        0    11449 2023-06-05 13:44:42.711640 guitk-0.4.3/guitk/tk_text.py
+-rw-r--r--   0        0        0     2523 2023-06-05 13:44:42.712010 guitk-0.4.3/guitk/tkroot.py
+-rw-r--r--   0        0        0     8686 2023-06-05 13:44:42.712276 guitk-0.4.3/guitk/tooltips.py
+-rw-r--r--   0        0        0    13189 2023-06-11 02:55:57.103304 guitk-0.4.3/guitk/ttk_button.py
+-rw-r--r--   0        0        0     5088 2023-06-05 13:44:42.712731 guitk-0.4.3/guitk/ttk_checkbutton.py
+-rw-r--r--   0        0        0     5717 2023-06-05 13:44:42.713001 guitk-0.4.3/guitk/ttk_combobox.py
+-rw-r--r--   0        0        0    11106 2023-06-13 04:42:37.907403 guitk-0.4.3/guitk/ttk_entry.py
+-rw-r--r--   0        0        0     7596 2023-06-05 13:44:42.713434 guitk-0.4.3/guitk/ttk_label.py
+-rw-r--r--   0        0        0     8873 2023-06-05 13:44:42.713652 guitk-0.4.3/guitk/ttk_notebook.py
+-rw-r--r--   0        0        0     8883 2023-06-05 13:44:42.714581 guitk-0.4.3/guitk/ttk_panedwindow.py
+-rw-r--r--   0        0        0     4898 2023-06-05 13:44:42.714718 guitk-0.4.3/guitk/ttk_progressbar.py
+-rw-r--r--   0        0        0     6148 2023-06-05 13:44:42.714850 guitk-0.4.3/guitk/ttk_radiobutton.py
+-rw-r--r--   0        0        0     7161 2023-06-05 13:44:42.714992 guitk-0.4.3/guitk/ttk_scale.py
+-rw-r--r--   0        0        0     2943 2023-06-05 13:44:42.715116 guitk-0.4.3/guitk/ttk_separator.py
+-rw-r--r--   0        0        0     7801 2023-06-05 13:44:42.715319 guitk-0.4.3/guitk/ttk_spinbox.py
+-rw-r--r--   0        0        0    12619 2023-06-05 13:44:42.715472 guitk-0.4.3/guitk/ttk_treeview.py
+-rw-r--r--   0        0        0      771 2023-06-05 13:44:42.715589 guitk-0.4.3/guitk/types.py
+-rw-r--r--   0        0        0     2527 2023-06-05 13:44:42.715787 guitk-0.4.3/guitk/utils.py
+-rw-r--r--   0        0        0     9333 2023-06-05 13:44:42.716003 guitk-0.4.3/guitk/widget.py
+-rw-r--r--   0        0        0    19055 2023-06-13 04:34:20.216968 guitk-0.4.3/guitk/window.py
+-rw-r--r--   0        0        0      804 2023-06-13 04:49:55.834612 guitk-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    10764 1970-01-01 00:00:00.000000 guitk-0.4.3/setup.py
+-rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 guitk-0.4.3/PKG-INFO
```

### Comparing `guitk-0.4.2/LICENSE` & `guitk-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/README.md` & `guitk-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,17 @@
         # optionally provide a unique key to each element to easily reference the element later
         # use a HLayout or VLayout class to define the layout of the window
         # HLayout arranges widgets horizontally, VLayout arranges widgets vertically
         with ui.VLayout():
             # use a VLayout to stack the widgets vertically
             # standard tkinter layout options such as sticky and weight are supported
             ui.Label("What's your name?", sticky="ew", anchor="center", weightx=1)
-            # most widgets emit events; Entry has events turned off by default so enable with events=True
             # each widget can be assigned a key, which should be unique, to easily reference the widget later
             # set focus=True so the Entry box has focus when the window is displayed
-            ui.Entry(key="entry_name", events=True, focus=True, weightx=1, sticky="ew")
+            ui.Entry(key="entry_name", focus=True, weightx=1, sticky="ew")
             ui.Label("", width=40, key="output")
             with ui.HStack():
                 # align these two buttons in a horizontal row using HStack
                 ui.Button("Ok")
                 ui.Button("Quit")
 
     # Every Window class has 3 special methods that can be overridden to provide custom behavior
```

### Comparing `guitk-0.4.2/guitk/__init__.py` & `guitk-0.4.3/guitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from .ttk_scale import Scale
 from .ttk_separator import HSeparator, VSeparator
 from .ttk_spinbox import Spinbox, SpinBox
 from .ttk_treeview import Listbox, ListBox, Treeview, TreeView
 from .widget import Widget, widget_class_factory
 from .window import Window
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 __author__ = "Rhet Turnbull"
 
 __all__ = [
     "BaseWidget",
     "BrowseDirectoryButton",
     "BrowseFileButton",
     "Button",
```

### Comparing `guitk-0.4.2/guitk/__main__.py` & `guitk-0.4.3/guitk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,28 +49,33 @@
             values=(str(f), f.stat().st_size),
         )
     tree.widget.selection_set(pyfiles)
 
 
 class Demo(Window):
     def config(self):
+        self.title = "GUTk Demo"
+        self.create_layout()
+        self.create_menubar()
+
+    def create_layout(self):
         with VLayout():
             with HStack(halign=tk.CENTER):
                 Label("This is a demo of GUITk widgets and layouts")
             HSeparator()
             with Notebook(sticky="nsew", weightx=1):
                 with VTab("Tab 1"):
                     with HStack():
                         LabelEntry("File:", key="file")
                         BrowseFileButton(target_key="file")
                         LabelEntry("Directory:", key="directory")
                         BrowseDirectoryButton(target_key="directory")
                         Button("Debug Window", key="debug_window")
                     with HStack():
-                        LabelEntry("Enter some text:", key="entry", events=True)
+                        LabelEntry("Enter some text:", key="entry", keyrelease=True)
                         Label("You entered:")
                         Label("", key="label_entered")
                     with HStack():
                         LinkLabel("This Label is a link", key="link", sticky="ns").font(
                             underline=True
                         ).style(foreground="blue")
                         CheckButton(
@@ -166,14 +171,34 @@
                     VSeparator()
                     with VStack(valign=tk.BOTTOM, expand=False):
                         Checkbutton("Enable", key="check_enable")
                         Checkbutton("Echo", key="check_echo")
                         Button("stdout")
                         Button("stderr")
 
+    def create_menubar(self):
+        """create the menu"""
+        with MenuBar():
+            with Menu("File"):
+                Command("Open", shortcut="Ctrl+O")
+                Command("Save")
+                Command("Save As")
+                Command("Exit", command=self.quit)
+            with Menu("Edit"):
+                Command("Cut")
+                Command("Copy")
+                Command("Paste")
+            with Menu("SubMenus"):
+                with Menu("SubMenu 1"):
+                    Command("Command 1")
+                    Command("Command 2")
+                with Menu("SubMenu 2"):
+                    Command("Command 3")
+                    Command("Command 4")
+
     def setup(self):
         """gets called right after __init__"""
         print(f"Setting up: {self.__dict__}")
 
         # check the Enable checkbutton for enabled output redirect
         self.get("check_enable").widget.invoke()
```

### Comparing `guitk-0.4.2/guitk/_debug.py` & `guitk-0.4.3/guitk/_debug.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/_on.py` & `guitk-0.4.3/guitk/_on.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/basewidget.py` & `guitk-0.4.3/guitk/basewidget.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/containers.py` & `guitk-0.4.3/guitk/containers.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/debugwindow.py` & `guitk-0.4.3/guitk/debugwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/events.py` & `guitk-0.4.3/guitk/events.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/frame.py` & `guitk-0.4.3/guitk/frame.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/image.py` & `guitk-0.4.3/guitk/image.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/layout.py` & `guitk-0.4.3/guitk/layout.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/menu.py` & `guitk-0.4.3/guitk/menu.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/redirect.py` & `guitk-0.4.3/guitk/redirect.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/spacer.py` & `guitk-0.4.3/guitk/spacer.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/tk_text.py` & `guitk-0.4.3/guitk/tk_text.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/tkroot.py` & `guitk-0.4.3/guitk/tkroot.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/tooltips.py` & `guitk-0.4.3/guitk/tooltips.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_button.py` & `guitk-0.4.3/guitk/ttk_button.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_checkbutton.py` & `guitk-0.4.3/guitk/ttk_checkbutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_combobox.py` & `guitk-0.4.3/guitk/ttk_combobox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_entry.py` & `guitk-0.4.3/guitk/ttk_entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         key: Hashable | None = None,
         default: str | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
         padx: PadType | None = None,
         pady: PadType | None = None,
-        events: bool = False,
+        events: bool = True,
+        keyrelease: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
         weightx: int | None = None,
         weighty: int | None = None,
         focus: bool = False,
@@ -65,24 +66,29 @@
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             default (str | None, optional): Default text for the entry box. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
             padx (PadType | None, optional): X padding. Defaults to None.
             pady (PadType | None, optional): Y padding. Defaults to None.
-            events (bool, optional): Enable events for this widget. Defaults to False.
+            events (bool, optional): Enable events for this widget. Defaults to True.
+            keyrelease (bool, optional): If True, generate events on key release. Defaults to False.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
             weightx (int | None, optional): Weight for horizontal resizing. Defaults to None.
             weighty (int | None, optional): Weight for vertical resizing. Defaults to None.
             focus (bool, optional): If True, widget has focus. Defaults to False.
                 Only one widget in a window can have focus.HLayout
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
+
+        Note:
+            Emits EventType.EntryReturn event on return key press.
+            If keyrelease is True, emits EventType.KeyRelease event on every key release.
         """
         super().__init__(
             key=key,
             disabled=disabled,
             columnspan=columnspan,
             rowspan=rowspan,
             padx=padx,
@@ -98,14 +104,15 @@
         self.widget_type = "ttk.Entry"
         default = default or ""
         self._value.set(default)
         self.key = key or "Entry"
         self.columnspan = columnspan
         self.rowspan = rowspan
         self.hscrollbar = hscrollbar
+        self.keyrelease = keyrelease
         self.kwargs = kwargs
 
     def _create_widget(self, parent, window: Window, row, col):
         # build arg list for ttk.Entry
         kwargs_entry = {
             k: v for k, v in self.kwargs.items() if k in _valid_ttk_entry_attributes
         }
@@ -117,16 +124,17 @@
             **kwargs_entry,
         )
         self._grid(
             row=row, column=col, rowspan=self.rowspan, columnspan=self.columnspan
         )
 
         # bind key release event
-        event = Event(self, window, self.key, EventType.KeyRelease)
-        self.widget.bind("<KeyRelease>", window._make_callback(event))
+        if self.keyrelease:
+            event = Event(self, window, self.key, EventType.KeyRelease)
+            self.widget.bind("<KeyRelease>", window._make_callback(event))
 
         # bind return key event
         entry_return_key = Event(self, window, self.key, EventType.EntryReturn)
         self.widget.bind("<Return>", window._make_callback(entry_return_key))
 
         if self._command:
             self.events = True
@@ -192,15 +200,16 @@
         key: Hashable | None = None,
         default: str | None = None,
         disabled: bool = False,
         columnspan: int | None = None,
         rowspan: int | None = None,
         padx: PadType | None = None,
         pady: PadType | None = None,
-        events: bool = False,
+        events: bool = True,
+        keyrelease: bool = False,
         sticky: str | None = None,
         tooltip: TooltipType = None,
         command: CommandType | None = None,
         hscrollbar: bool = False,
         weightx: int | None = None,
         weighty: int | None = None,
         focus: bool = False,
@@ -213,33 +222,39 @@
             key (Hashable, optional): Unique key for this widget. Defaults to None.
             default (str | None, optional): Default text for the entry box. Defaults to None.
             disabled (bool, optional): If True, widget is disabled. Defaults to False.
             columnspan (int | None, optional): Number of columns to span. Defaults to None.
             rowspan (int | None, optional): Number of rows to span. Defaults to None.
             padx (PadType | None, optional): X padding. Defaults to None.
             pady (PadType | None, optional): Y padding. Defaults to None.
-            events (bool, optional): Enable events for this widget. Defaults to False.
+            events (bool, optional): Enable events for this widget. Defaults to True.
+            keyrelease (bool, optional): If True, emits EventType.KeyRelease event on every key release.
             sticky (str | None, optional): Sticky direction for widget layout. Defaults to None.
             tooltip (TooltipType | None, optional): Tooltip text or callback to generate tooltip text. Defaults to None.
             command (CommandType | None, optional): Command callback. Defaults to None.
             hscrollbar (bool, optional): Show horizontal scrollbar. Defaults to False.
             weightx (int | None, optional): Weight for horizontal resizing. Defaults to None.
             weighty (int | None, optional): Weight for vertical resizing. Defaults to None.
             focus (bool, optional): If True, widget will have focus. Defaults to False. Only one widget can have focus.
             **kwargs: Additional keyword arguments are passed to ttk.Entry.
+
+        Note:
+            Emits EventType.EntryReturn event on return key press.
+            If keyrelease is True, emits EventType.KeyRelease event on every key release.
         """
         super().__init__(
             key=key,
             default=default,
             disabled=disabled,
             columnspan=columnspan,
             rowspan=rowspan,
             padx=padx,
             pady=pady,
             events=events,
+            keyrelease=keyrelease,
             sticky=sticky,
             tooltip=tooltip,
             command=command,
             hscrollbar=hscrollbar,
             focus=focus,
             weightx=weightx,
             weighty=weighty,
```

### Comparing `guitk-0.4.2/guitk/ttk_label.py` & `guitk-0.4.3/guitk/ttk_label.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_notebook.py` & `guitk-0.4.3/guitk/ttk_notebook.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_panedwindow.py` & `guitk-0.4.3/guitk/ttk_panedwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_progressbar.py` & `guitk-0.4.3/guitk/ttk_progressbar.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_radiobutton.py` & `guitk-0.4.3/guitk/ttk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_scale.py` & `guitk-0.4.3/guitk/ttk_scale.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_separator.py` & `guitk-0.4.3/guitk/ttk_separator.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_spinbox.py` & `guitk-0.4.3/guitk/ttk_spinbox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/ttk_treeview.py` & `guitk-0.4.3/guitk/ttk_treeview.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/types.py` & `guitk-0.4.3/guitk/types.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/utils.py` & `guitk-0.4.3/guitk/utils.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/widget.py` & `guitk-0.4.3/guitk/widget.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/guitk/window.py` & `guitk-0.4.3/guitk/window.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.2/pyproject.toml` & `guitk-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guitk"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python."
 authors = ["Rhet Turnbull <rturnbull+git@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `guitk-0.4.2/setup.py` & `guitk-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['guitk']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'guitk',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.',
-    'long_description': '<!--* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->\n\n# Python GUI Toolkit for TK (GUITk)\n\n## Synopsis\n\nGUITk is a declarative framework for building nice-looking, cross-platform GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html) inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui).\n\nGUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.\n\nGUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.\n\nGUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!\n\nDocumentation is available at [GUITk](https://rhettbull.github.io/guitk/).\n\n## Code Example\n\n### Simple HLayout\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello.py HelloWindow docs/images/hello.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello.py.png "Hello World example")\n\n```python\n"""Simple Hello World example using guitk """\n\nimport guitk as ui\n\n\n# subclass guitk.Window as the starting point for your app\'s main window\nclass HelloWindow(ui.Window):\n    def config(self):\n        """Configure the window"""\n\n        # set the window title\n        self.title = "Hello, World"\n\n        # define a layout for the window\n        # the layout manager will automatically add widgets to the window\n        with ui.HLayout():\n            ui.Label("What\'s your name?")\n            ui.Entry(key="name", focus=True)\n            ui.Button("Ok")\n\n    @ui.on(key="Ok")\n    def on_ok(self, event: ui.Event):\n        """Handle the Ok button click"""\n        print("Hello, ", self.get("name").value)\n\n\n# run your event loop\nif __name__ == "__main__":\n    HelloWindow().run()\n```\n\n## Motivation\n\nThe goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.\n\nThough you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman\'s excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.\n\n## Installation\n\n* `python3 -m pip install guitk`\n\n## Anatomy of a guitk program\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello2.py HelloWorld docs/images/hello2.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello2.py.png "Hello World example")\n\n```python\n"""Hello World example using guitk """\n\nimport guitk as ui\n\n\nclass HelloWorld(ui.Window):\n    # subclass guitk.Window as the starting point for your app\'s main window\n    def config(self):\n        # Your Window class needs to define a config() method that describes the layout, title, etc for your app\n        # config() is called by the Window class when the Window is being created\n\n        # Title for the window\n        self.title = "Hello, World"\n\n        # optionally set size as a tuple of (width, height)\n        self.size = (320, 240)\n\n        # you can also use self.geometry for consistency with tkinter\n        # self.geometry = "320x240"\n\n        # Define the window\'s contents\n        # guitk.Label corresponds to a tkinter.ttk.Label, etc.\n        # optionally provide a unique key to each element to easily reference the element later\n        # use a HLayout or VLayout class to define the layout of the window\n        # HLayout arranges widgets horizontally, VLayout arranges widgets vertically\n        with ui.VLayout():\n            # use a VLayout to stack the widgets vertically\n            # standard tkinter layout options such as sticky and weight are supported\n            ui.Label("What\'s your name?", sticky="ew", anchor="center", weightx=1)\n            # most widgets emit events; Entry has events turned off by default so enable with events=True\n            # each widget can be assigned a key, which should be unique, to easily reference the widget later\n            # set focus=True so the Entry box has focus when the window is displayed\n            ui.Entry(key="entry_name", events=True, focus=True, weightx=1, sticky="ew")\n            ui.Label("", width=40, key="output")\n            with ui.HStack():\n                # align these two buttons in a horizontal row using HStack\n                ui.Button("Ok")\n                ui.Button("Quit")\n\n    # Every Window class has 3 special methods that can be overridden to provide custom behavior\n    # you do not need to provide any of these methods if you do not need to customize the default behavior\n    # (the default behavior is to do nothing)\n    # These special methods are: setup(), teardown(), and handle_event()\n\n    def setup(self):\n        """Perform any initialization needed before the Window is displayed"""\n        # your setup() method is called by the Window class after config() just before the Window is displayed\n        # use this to initialize any internal state you need\n        # you do not need to provide a setup() method if no initialization is needed\n        print("setup")\n\n    def teardown(self):\n        """Perform any cleanup needed before destroying the window"""\n        # your teardown() method is called by the Window class after the Window is closed\n        # use this to clean up before the Window is destroyed\n        # you do not need to provide a teardown() method if no cleanup is needed\n        print("teardown")\n\n    def handle_event(self, event: ui.Event):\n        """handle_event() is called by the Window class when an event occurs"""\n        # you do not need to provide a handle_event() method if you prefer to use\n        # the @on decorator to bind functions to events (see below)\n        # handle_event() is a useful place to put code that needs to run for every event\n        # or for use during debugging\n        print(f"handle_event: {event}")\n\n    @ui.on(key="Quit")\n    def on_quit(self):\n        # return the value of the Entry box\n        self.quit(self["entry_name"].value)\n\n    @ui.on(key="Ok")\n    @ui.on(event_type=ui.EventType.EntryReturn)\n    def on_ok(self):\n        # User pressed the OK button or the Return key inside the Entry box\n        # the @on decorator can be used to bind a function to an event\n        # @on can be repeated to bind the function to multiple events\n        # set the output Label to the value of the Entry box\n        # individual widgets can be accessed by their key; the window object acts as a dictionary of widgets\n        greeting = f"Hello {self[\'entry_name\'].value}! Thanks for trying guitk."\n\n        # if you prefer, you can use get() instead of the dictionary syntax\n        self.get("output").value = greeting\n\n\nif __name__ == "__main__":\n    # instantiate your Window class and run it\n    name = HelloWorld().run()\n    print(f"Hello {name}")\n```\n\n## Documentation\n\nNot much documentation at this point but there\'s a start [here](https://rhettbull.github.io/guitk/).  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.\n\n## Testing\n\nThere are currently no automated tests as I haven\'t figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.\n\nYou can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.\n\n## Contributors\n\nContributions welcome! If this project interests you, open an Issue or send a PR!\n\n## TODO\n\n* [x] Basic prototype\n* [x] Frame\n* [x] Label\n* [x] Entry\n* [x] Button\n* [x] Checkbutton\n* [x] Radiobutton\n* [x] Text\n* [x] ScrolledText\n* [x] Treeview\n* [x] Listbox\n* [x] Combobox\n* [x] Spinner\n* [x] Other widgets\n* [x] Menus\n* [x] Tooltips\n* [ ] Documentation\n* [x] Add docstrings\n* [x] Add type hints to public API\n* [ ] Tests\n\n## License\n\nLicensed under the MIT License.\n\n## See Also\n\n* [Textual](https://github.com/Textualize/textual) - An amazing Python framework for building user interfaces in the terminal.\n* [PySimpleGUI](https://www.PySimpleGUI.org) - A Python GUI Framework.\n* [applepy](https://github.com/eduardohleite/applepy) - A declarative GUI framework for developing native macOS applications in Python 3.\n',
+    'long_description': '<!--* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->\n\n# Python GUI Toolkit for TK (GUITk)\n\n## Synopsis\n\nGUITk is a declarative framework for building nice-looking, cross-platform GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html) inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui).\n\nGUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.\n\nGUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.\n\nGUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!\n\nDocumentation is available at [GUITk](https://rhettbull.github.io/guitk/).\n\n## Code Example\n\n### Simple HLayout\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello.py HelloWindow docs/images/hello.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello.py.png "Hello World example")\n\n```python\n"""Simple Hello World example using guitk """\n\nimport guitk as ui\n\n\n# subclass guitk.Window as the starting point for your app\'s main window\nclass HelloWindow(ui.Window):\n    def config(self):\n        """Configure the window"""\n\n        # set the window title\n        self.title = "Hello, World"\n\n        # define a layout for the window\n        # the layout manager will automatically add widgets to the window\n        with ui.HLayout():\n            ui.Label("What\'s your name?")\n            ui.Entry(key="name", focus=True)\n            ui.Button("Ok")\n\n    @ui.on(key="Ok")\n    def on_ok(self, event: ui.Event):\n        """Handle the Ok button click"""\n        print("Hello, ", self.get("name").value)\n\n\n# run your event loop\nif __name__ == "__main__":\n    HelloWindow().run()\n```\n\n## Motivation\n\nThe goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.\n\nThough you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman\'s excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.\n\n## Installation\n\n* `python3 -m pip install guitk`\n\n## Anatomy of a guitk program\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello2.py HelloWorld docs/images/hello2.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello2.py.png "Hello World example")\n\n```python\n"""Hello World example using guitk """\n\nimport guitk as ui\n\n\nclass HelloWorld(ui.Window):\n    # subclass guitk.Window as the starting point for your app\'s main window\n    def config(self):\n        # Your Window class needs to define a config() method that describes the layout, title, etc for your app\n        # config() is called by the Window class when the Window is being created\n\n        # Title for the window\n        self.title = "Hello, World"\n\n        # optionally set size as a tuple of (width, height)\n        self.size = (320, 240)\n\n        # you can also use self.geometry for consistency with tkinter\n        # self.geometry = "320x240"\n\n        # Define the window\'s contents\n        # guitk.Label corresponds to a tkinter.ttk.Label, etc.\n        # optionally provide a unique key to each element to easily reference the element later\n        # use a HLayout or VLayout class to define the layout of the window\n        # HLayout arranges widgets horizontally, VLayout arranges widgets vertically\n        with ui.VLayout():\n            # use a VLayout to stack the widgets vertically\n            # standard tkinter layout options such as sticky and weight are supported\n            ui.Label("What\'s your name?", sticky="ew", anchor="center", weightx=1)\n            # each widget can be assigned a key, which should be unique, to easily reference the widget later\n            # set focus=True so the Entry box has focus when the window is displayed\n            ui.Entry(key="entry_name", focus=True, weightx=1, sticky="ew")\n            ui.Label("", width=40, key="output")\n            with ui.HStack():\n                # align these two buttons in a horizontal row using HStack\n                ui.Button("Ok")\n                ui.Button("Quit")\n\n    # Every Window class has 3 special methods that can be overridden to provide custom behavior\n    # you do not need to provide any of these methods if you do not need to customize the default behavior\n    # (the default behavior is to do nothing)\n    # These special methods are: setup(), teardown(), and handle_event()\n\n    def setup(self):\n        """Perform any initialization needed before the Window is displayed"""\n        # your setup() method is called by the Window class after config() just before the Window is displayed\n        # use this to initialize any internal state you need\n        # you do not need to provide a setup() method if no initialization is needed\n        print("setup")\n\n    def teardown(self):\n        """Perform any cleanup needed before destroying the window"""\n        # your teardown() method is called by the Window class after the Window is closed\n        # use this to clean up before the Window is destroyed\n        # you do not need to provide a teardown() method if no cleanup is needed\n        print("teardown")\n\n    def handle_event(self, event: ui.Event):\n        """handle_event() is called by the Window class when an event occurs"""\n        # you do not need to provide a handle_event() method if you prefer to use\n        # the @on decorator to bind functions to events (see below)\n        # handle_event() is a useful place to put code that needs to run for every event\n        # or for use during debugging\n        print(f"handle_event: {event}")\n\n    @ui.on(key="Quit")\n    def on_quit(self):\n        # return the value of the Entry box\n        self.quit(self["entry_name"].value)\n\n    @ui.on(key="Ok")\n    @ui.on(event_type=ui.EventType.EntryReturn)\n    def on_ok(self):\n        # User pressed the OK button or the Return key inside the Entry box\n        # the @on decorator can be used to bind a function to an event\n        # @on can be repeated to bind the function to multiple events\n        # set the output Label to the value of the Entry box\n        # individual widgets can be accessed by their key; the window object acts as a dictionary of widgets\n        greeting = f"Hello {self[\'entry_name\'].value}! Thanks for trying guitk."\n\n        # if you prefer, you can use get() instead of the dictionary syntax\n        self.get("output").value = greeting\n\n\nif __name__ == "__main__":\n    # instantiate your Window class and run it\n    name = HelloWorld().run()\n    print(f"Hello {name}")\n```\n\n## Documentation\n\nNot much documentation at this point but there\'s a start [here](https://rhettbull.github.io/guitk/).  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.\n\n## Testing\n\nThere are currently no automated tests as I haven\'t figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.\n\nYou can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.\n\n## Contributors\n\nContributions welcome! If this project interests you, open an Issue or send a PR!\n\n## TODO\n\n* [x] Basic prototype\n* [x] Frame\n* [x] Label\n* [x] Entry\n* [x] Button\n* [x] Checkbutton\n* [x] Radiobutton\n* [x] Text\n* [x] ScrolledText\n* [x] Treeview\n* [x] Listbox\n* [x] Combobox\n* [x] Spinner\n* [x] Other widgets\n* [x] Menus\n* [x] Tooltips\n* [ ] Documentation\n* [x] Add docstrings\n* [x] Add type hints to public API\n* [ ] Tests\n\n## License\n\nLicensed under the MIT License.\n\n## See Also\n\n* [Textual](https://github.com/Textualize/textual) - An amazing Python framework for building user interfaces in the terminal.\n* [PySimpleGUI](https://www.PySimpleGUI.org) - A Python GUI Framework.\n* [applepy](https://github.com/eduardohleite/applepy) - A declarative GUI framework for developing native macOS applications in Python 3.\n',
     'author': 'Rhet Turnbull',
     'author_email': 'rturnbull+git@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `guitk-0.4.2/PKG-INFO` & `guitk-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guitk
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.
 License: MIT
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -117,18 +117,17 @@
         # optionally provide a unique key to each element to easily reference the element later
         # use a HLayout or VLayout class to define the layout of the window
         # HLayout arranges widgets horizontally, VLayout arranges widgets vertically
         with ui.VLayout():
             # use a VLayout to stack the widgets vertically
             # standard tkinter layout options such as sticky and weight are supported
             ui.Label("What's your name?", sticky="ew", anchor="center", weightx=1)
-            # most widgets emit events; Entry has events turned off by default so enable with events=True
             # each widget can be assigned a key, which should be unique, to easily reference the widget later
             # set focus=True so the Entry box has focus when the window is displayed
-            ui.Entry(key="entry_name", events=True, focus=True, weightx=1, sticky="ew")
+            ui.Entry(key="entry_name", focus=True, weightx=1, sticky="ew")
             ui.Label("", width=40, key="output")
             with ui.HStack():
                 # align these two buttons in a horizontal row using HStack
                 ui.Button("Ok")
                 ui.Button("Quit")
 
     # Every Window class has 3 special methods that can be overridden to provide custom behavior
```

