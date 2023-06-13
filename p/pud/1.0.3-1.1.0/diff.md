# Comparing `tmp/pud-1.0.3-py3-none-any.whl.zip` & `tmp/pud-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 7314 bytes, number of entries: 14
+Zip file size: 8883 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 14:07 pud/__init__.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 12:58 pud/__main__.py
--rw-rw-rw-  2.0 fat     7365 b- defN 23-Jun-10 08:51 pud/app.py
--rw-rw-rw-  2.0 fat      779 b- defN 23-Jun-09 08:33 pud/entity.py
+-rw-rw-rw-  2.0 fat    10519 b- defN 23-Jun-13 07:13 pud/app.py
+-rw-rw-rw-  2.0 fat     1391 b- defN 23-Jun-13 04:43 pud/entity.py
 -rw-rw-rw-  2.0 fat      285 b- defN 23-Jun-10 06:16 pud/main.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-09 12:58 pud/options.py
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-10 08:45 pud/handlers/__init__.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-Jun-10 08:50 pud/handlers/directory.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1157 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1030 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/RECORD
-14 files, 14048 bytes uncompressed, 5624 bytes compressed:  60.0%
+-rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-10 09:01 pud/options.py
+-rw-rw-rw-  2.0 fat     1014 b- defN 23-Jun-13 06:29 pud/utils.py
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-13 06:22 pud/handlers/__init__.py
+-rw-rw-rw-  2.0 fat     1997 b- defN 23-Jun-13 07:14 pud/handlers/directory.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1157 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1101 b- defN 23-Jun-13 07:16 pud-1.1.0.dist-info/RECORD
+15 files, 19356 bytes uncompressed, 7093 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -12,32 +12,35 @@
 
 Filename: pud/main.py
 Comment: 
 
 Filename: pud/options.py
 Comment: 
 
+Filename: pud/utils.py
+Comment: 
+
 Filename: pud/handlers/__init__.py
 Comment: 
 
 Filename: pud/handlers/directory.py
 Comment: 
 
-Filename: pud-1.0.3.dist-info/LICENSE
+Filename: pud-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pud-1.0.3.dist-info/METADATA
+Filename: pud-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pud-1.0.3.dist-info/WHEEL
+Filename: pud-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pud-1.0.3.dist-info/entry_points.txt
+Filename: pud-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pud-1.0.3.dist-info/top_level.txt
+Filename: pud-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pud-1.0.3.dist-info/RECORD
+Filename: pud-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pud/app.py

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 import curses
 from pathlib import Path
 
-from .entity import Entity, GoBack
+from .entity import Entity
 from .handlers import DirectoryExplorer
+from .utils import get_dir_size, parse_bytes
 
 
 KEY_UP = (curses.KEY_UP, 450, ord('w'))
 KEY_DOWN = (curses.KEY_DOWN, 456, ord('s'))
-ENTER = (curses.KEY_ENTER, ord('\n'), ord('\r'))
+ENTER = (curses.KEY_ENTER, curses.KEY_RIGHT, 454, ord('\n'), ord('\r'), ord('d'))
+GET_INFO = (9,)
 SCROLL_UP = (65536,)
 SCROLL_DOWN = (2097152,)
+QUIT = (27, ord('q'))
+GO_BACK = (curses.KEY_LEFT, 452, 260, ord('b'), ord('a'))
 
 
 class App:
     """The main application for displaying folders and selecting directories.
 
     Attributes
     ----------
@@ -79,66 +83,150 @@
     def reset_state(self) -> None:
         """Resets the states."""
 
         self.idx = 0
         self.offset = 0
         self.screen_idx = 0
 
-    def get_files(self) -> tuple[tuple[int, GoBack | Entity], ...]:
+    def get_files(self) -> tuple[tuple[int, Entity], ...]:
         """Gets all the files from the current working directory and stores it in a list."""
 
-        back = [GoBack()]
         files = self.explorer.list_files()
 
         if files is None:
             files = []
             message = "Permission Denied."
             maxy, maxx = self.screen.getmaxyx()
             self.screen.addstr(maxy // 2, (maxx // 2) - (len(message) // 2), message)
 
+        elif len(files) == 0:
+            message = "Directory Empty."
+            self.maxy, maxx = self.screen.getmaxyx()
+            self.screen.addstr(self.maxy // 2, (maxx // 2) - (len(message) // 2), message)
+
         ret = sorted(files, key=lambda f: f.is_file)
-        return tuple(enumerate(back + ret))
+        return tuple(enumerate(ret))
+
+    def create_window(self) -> tuple["curses._CursesWindow", int, int]:
+        """Creates a new top level window."""
+
+        maxy, maxx = self.screen.getmaxyx()
+        size_y, size_x = maxy // 2, maxx // 2
+        win = curses.newwin(size_y, int(size_x * 1.50), size_y // 2, size_x // 4)
+        win.box()
+        win_maxy, win_maxx = win.getmaxyx()
+        return win, win_maxy, win_maxx
+
+    def show_help(self) -> None:
+        """Shows the help window."""
+
+        win, win_maxy, win_maxx = self.create_window()
+        win.box()
+
+        win.addstr(0, (win_maxx // 2) - 2, "Help", curses.A_STANDOUT)
+        action_col = win_maxx // 2
+
+        help_comb = [
+            ("up, w", "Move up"),
+            ("down, s", "Move down"),
+            ("enter, right, a", "Enter directory"),
+            ("b, left, d", "Go to parent directory"),
+            ("esc, q", "Exit")
+        ]
+
+        for y, (key, action) in zip(range(1, win_maxy - 1), help_comb):
+            win.addstr(y, 1, key)
+            win.addstr(y, action_col, action)
+
+        while True:
+            key = win.getch()
+
+            if key in QUIT:
+                win.erase()
+                break
+
+    def show_info(self, entity: Entity) -> None:
+        """Shows the info window."""
+
+        win, win_maxy, win_maxx = self.create_window()
+        item = Path(self.explorer.cwd, entity.name)
+
+        try:
+            if entity.is_file:
+                size = entity.size
+            else:
+                size = parse_bytes(get_dir_size(item))
+
+            infos = (
+                f"Path: {str(item)}",
+                f"Name: {entity.name}",
+                f"Type: {['Folder', 'File'][entity.is_file]}",
+                f"Size: {size}",
+                f"Last Modified: {entity.last_modified}",
+            )
+
+            win.addstr(0, (win_maxx // 2) - 2, "Info", curses.A_STANDOUT)
+
+            for y, info in zip(range(1, win_maxy - 1), infos):
+                win.addstr(y, 1, info)
+
+        except PermissionError:
+            message = "Permission Denied. Press Q to close."
+            win_maxy, win_maxx = win.getmaxyx()
+            win.addstr(win_maxy // 2, (win_maxx // 2) - (len(message) // 2), message)
+
+        while True:
+            key = win.getch()
+
+            if key in QUIT:
+                win.erase()
+                break
 
     def draw_screen(self) -> None:
         """Draws all the folders/files into the screen."""
 
         self.screen.clear()
 
         y = 0
         self.maxy, maxx = self.screen.getmaxyx()
         self.maxy -= 4
         files = self.get_files()
 
-        self.screen.addstr(y, 1, f"Current Directory: {self.explorer.cwd}")
-        y += 1
-        self.screen.addstr(y, 1, "Press CTRL + C or Esc or q to exit.")
+        self.screen.addstr(y, 1, "Press ? to show help window. Esc or q to exit.")
         y += 1
 
-        files = files[self.offset:self.maxy + self.offset]
+        self.screen.addstr(y, 1, f"Current Directory: {self.explorer.cwd}")
+        y += 2
+
+        self.screen.addstr(y, 4, "File Name")
+        self.screen.addstr(y, maxx // 3, "File Size")
+        self.screen.addstr(y, maxx // 2, "Last Modified")
+
+        files = files[self.offset:(self.maxy + self.offset) - 2]
         coords = []
 
         for idx, file in files:
             y += 1
 
+            if len(file.name) > 29:
+                file.name = f"{file.name[:29]}..."
+
             if self.idx == idx:
                 file_display = f"{self.cursor} {file}"
             else:
                 file_display = f"{' ' * len(self.cursor)} {file}"
 
             self.screen.addnstr(y, 1, file_display, maxx - 2)
+            self.screen.addnstr(y, maxx // 3, file.size, maxx - 2)
+            self.screen.addnstr(y, maxx // 2, file.last_modified, maxx - 2)
             coords.append((file.name, range(1, len(file_display)), y))
 
         self.coords = coords
         self.screen.refresh()
 
-    def get_key(self) -> int:
-        """Returns a pressed key."""
-
-        return self.screen.getch()
-
     def move_up(self) -> None:
         """Adjusts the indexes and offset if possible.
 
         This makes the cursor go up.
         """
 
         if self.idx > 0:
@@ -155,75 +243,84 @@
 
         This makes the cursor go down.
         """
 
         if self.idx < len(self.get_files()) - 1:
             self.idx += 1
 
-            if self.screen_idx >= self.maxy - 1:
+            if self.screen_idx >= self.maxy - 3:
                 self.offset += 1
 
-            if self.screen_idx < self.maxy - 1:
+            if self.screen_idx < self.maxy - 3:
                 self.screen_idx += 1
 
     def pop_cursor_stack(self):
         """Pops the cursor stack and returns it."""
 
         if len(self.cursor_stack) > 1:
             return self.cursor_stack.pop()
 
         return self.cursor_stack[0]
 
     def execute_by_key(self, key: int) -> None:
         """Executes an action based on the key.
 
         key:
-            The key returned by `get_key`.
+            The key returned by `getch`.
         """
 
-        if key in (27, ord('q')):  # Esc key or 'q'
+        if key in QUIT:  # Esc key or 'q'
             raise SystemExit()
 
+        if key in (ord('?'),):
+            self.show_help()
+
+        if key in GET_INFO:
+            self.show_info(self.get_files()[self.idx][1])
+
+        if key in GO_BACK:
+            self.explorer.go_back()
+
+            if self.keep_cursor_state:
+                offset, index, screen_index = self.pop_cursor_stack()
+
+                self.offset = offset
+                self.idx = index
+                self.screen_idx = screen_index
+
         if key in KEY_UP:
             self.move_up()
 
         if key in KEY_DOWN:
             self.move_down()
 
         if key in ENTER:
-            if self.idx == 0:
-                self.explorer.go_back()
+            files = self.get_files()
 
-                if self.keep_cursor_state:
-                    offset, index, screen_index = self.pop_cursor_stack()
+            if not files:
+                return
 
-                    self.offset = offset
-                    self.idx = index
-                    self.screen_idx = screen_index
+            selected = files[self.idx][1].name
 
-            else:
-                files = self.get_files()
-                selected = files[self.idx][1].name
-
-                entered = self.explorer.enter(selected)
+            entered = self.explorer.enter(selected)
 
-                if not entered:
-                    return
+            if not entered:
+                return
 
-                state = (0, 0, 0)
+            state = (0, 0, 0)
 
-                if self.keep_cursor_state:
-                    state = (
-                        self.offset,
-                        self.idx,
-                        self.screen_idx
-                    )
+            if self.keep_cursor_state:
+                state = (
+                    self.offset,
+                    self.idx,
+                    self.screen_idx
+                )
 
-                self.cursor_stack.append(state)
-                self.reset_state()
+            self.cursor_stack.append(state)
+            self.reset_state()
 
     def handle_mouse_event(self) -> None:
         """Handles a mouse event."""
 
         _, x, y, _, bstate = curses.getmouse()
 
         is_double_click = bstate & curses.BUTTON1_DOUBLE_CLICKED
@@ -250,14 +347,14 @@
             self.move_down()
 
     def _run(self):
         """Starts the loop to run the app."""
 
         while True:
             self.draw_screen()
-            key = self.get_key()
+            key = self.screen.getch()
 
             if key == curses.KEY_MOUSE:
                 self.handle_mouse_event()
                 continue
 
             self.execute_by_key(key)
```

## pud/entity.py

```diff
@@ -1,38 +1,63 @@
-class GoBack:
-    name = "Back"
-
-    def __repr__(self) -> str:
-        return "<<< Go Back"
+from datetime import datetime
 
 
 class Entity:
     """Represents an entity to display on the screen.
 
     Attributes
     ----------
     name:
         The name of the entity.
 
+    size:
+        The human readable size of the entity.
+
     is_file:
         Indicates if this entity is a file or not.
+
+    last_modified:
+        The human readable representation of the date
+        when this entity was last modified.
     """
 
-    def __init__(self, name: str, is_file: bool):
+    def __init__(
+        self,
+        name: str,
+        size: str,
+        is_file: bool,
+        last_modified: datetime,
+    ):
         self._name = name
+        self._size = size
         self._is_file = is_file
+        self._last_modified = last_modified
 
         if self._is_file:
             self.emoji = "📄"
         else:
             self.emoji = "📁"
 
     @property
     def name(self) -> str:
         return self._name
 
+    @name.setter
+    def name(self, new_name: str):
+        self._name = new_name
+
+    @property
+    def size(self) -> str:
+        if self.is_file:
+            return self._size
+        return ""
+
     @property
     def is_file(self) -> bool:
         return self._is_file
 
+    @property
+    def last_modified(self) -> str:
+        return self._last_modified
+
     def __repr__(self) -> str:
-        return f"{self.emoji} {self.name}"
+        return f"{self.emoji} {self.name if self.is_file else '/' + self.name}"
```

## pud/handlers/directory.py

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import os
+from datetime import datetime
 from pathlib import Path
 
 from ..entity import Entity
+from ..utils import parse_bytes
 
 
 class DirectoryExplorer:
     """The directory handler responsible for entering and leaving directories.
 
     Attributes
     ----------
     cwd:
         The current working directory.
     """
+
     def __init__(self, cwd: Path) -> None:
         self.cwd = cwd
 
     def enter(self, name: str) -> bool:
         """Enters a folder or a file.
 
         Paremeters
@@ -50,15 +53,28 @@
         self.enter(self.cwd.parent)
         self.refresh_cwd()
 
     def list_files(self) -> list[Entity] | None:
         """Lists all the files in the current directory."""
 
         try:
-            files = [Entity(entity.name, entity.is_file()) for entity in self.cwd.iterdir()]
+            files = []
+
+            for entity in self.cwd.iterdir():
+                stats = entity.stat()
+                last_modified = datetime.fromtimestamp(stats.st_mtime)
+                files.append(
+                    Entity(
+                        entity.name,
+                        parse_bytes(stats.st_size),
+                        entity.is_file(),
+                        last_modified.strftime("%x %I:%M:%S")
+                    )
+                )
+
         except PermissionError:
             files = None
 
         return files
 
     def refresh_cwd(self):
         """Refreshes the current directory."""
```

## Comparing `pud-1.0.3.dist-info/LICENSE` & `pud-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pud-1.0.3.dist-info/METADATA` & `pud-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pud
-Version: 1.0.3
+Version: 1.1.0
 Summary: A command-line tool for navigating directories.
 Home-page: https://github.com/Jedddy/pud
 Author: Jedddy
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `pud-1.0.3.dist-info/RECORD` & `pud-1.1.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 pud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pud/__main__.py,sha256=X86mONAr_BaFTmbpJgWB4SAQ3SW7AICSzrbLkyDJob0,100
-pud/app.py,sha256=ODBDVIUmY0rTxER5JgFXbbVwOlBnJ3j_FZe427Bl9Mc,7365
-pud/entity.py,sha256=T_JEtQdEZEo3vDEx5pYj6q4dwXsSFjSw2tyLzo60XUM,779
+pud/app.py,sha256=x1tjRnu2fGCGzXohna1r7UvBhdga5lQEmxifpQNcqi0,10519
+pud/entity.py,sha256=qEJYsGS386IasyHdcL5KS8X9rulR9Y05f3TyuQ-MbeQ,1391
 pud/main.py,sha256=YajWrXJIvtbQY4wM1EqyfzrUk0eMHymWB0CW7k3xbc0,285
 pud/options.py,sha256=NHGSE_KIl9gvUKbj1wlVVsVR_d8kuQy5n3T6W--1nZ8,545
+pud/utils.py,sha256=aaYQwGJfNcxS2EClvLBOFX0zASUTypCKVbLU28Bs_rs,1014
 pud/handlers/__init__.py,sha256=Grm4Xu5XbBij463ZRqW3rJGffsYOH2bS_8pNKCzDxww,42
-pud/handlers/directory.py,sha256=FE-UROTFsA_zjdfb7Han24ZwTYj_5qIOtmpv4P9miuM,1540
-pud-1.0.3.dist-info/LICENSE,sha256=v0PHLuz3Fx7aA5ulQVj5i2V9OObeeStZrZ1ZDb65ChE,1070
-pud-1.0.3.dist-info/METADATA,sha256=lA9Z7WNypS2hc4AqUyUVF4RwWW-YmZLUFNNDwEmsZFs,1157
-pud-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pud-1.0.3.dist-info/entry_points.txt,sha256=ZICpIyMhM1UpeUR8s2Lt4pe9BBo7XHAUwBDPodR6Ltw,39
-pud-1.0.3.dist-info/top_level.txt,sha256=bzTwibMohuSeyMWwBz7PqNY87HyQ-ywUmdG_wog_UV8,4
-pud-1.0.3.dist-info/RECORD,,
+pud/handlers/directory.py,sha256=U3Mp1uyfIbes24Ny-2MEJmpeisdR14bzEACgByr0uCE,1997
+pud-1.1.0.dist-info/LICENSE,sha256=v0PHLuz3Fx7aA5ulQVj5i2V9OObeeStZrZ1ZDb65ChE,1070
+pud-1.1.0.dist-info/METADATA,sha256=V4LAjHvs-K1TUwH5rYXkVqEVmZPnGJMx3oiG1xrrSs0,1157
+pud-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pud-1.1.0.dist-info/entry_points.txt,sha256=ZICpIyMhM1UpeUR8s2Lt4pe9BBo7XHAUwBDPodR6Ltw,39
+pud-1.1.0.dist-info/top_level.txt,sha256=bzTwibMohuSeyMWwBz7PqNY87HyQ-ywUmdG_wog_UV8,4
+pud-1.1.0.dist-info/RECORD,,
```

