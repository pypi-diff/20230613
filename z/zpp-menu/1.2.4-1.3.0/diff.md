# Comparing `tmp/zpp_menu-1.2.4.tar.gz` & `tmp/zpp_menu-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpp_menu-1.2.4.tar", last modified: Tue Jun 13 07:45:26 2023, max compression
+gzip compressed data, was "zpp_menu-1.3.0.tar", last modified: Tue Jun 13 15:35:16 2023, max compression
```

## Comparing `zpp_menu-1.2.4.tar` & `zpp_menu-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:45:26.982000 zpp_menu-1.2.4/
--rw-rw-rw-   0        0        0     1106 2023-06-13 07:42:50.000000 zpp_menu-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     1467 2023-06-13 07:45:26.978000 zpp_menu-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      854 2022-12-02 09:20:50.000000 zpp_menu-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 07:45:26.981000 zpp_menu-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      758 2022-04-27 09:37:02.000000 zpp_menu-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:45:26.950000 zpp_menu-1.2.4/zpp_menu/
--rw-rw-rw-   0        0        0       19 2023-06-13 07:43:09.000000 zpp_menu-1.2.4/zpp_menu/__init__.py
--rw-rw-rw-   0        0        0    11932 2023-06-13 07:43:01.000000 zpp_menu-1.2.4/zpp_menu/menu.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:45:26.973000 zpp_menu-1.2.4/zpp_menu.egg-info/
--rw-rw-rw-   0        0        0     1467 2023-06-13 07:45:26.000000 zpp_menu-1.2.4/zpp_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-13 07:45:26.000000 zpp_menu-1.2.4/zpp_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:45:26.000000 zpp_menu-1.2.4/zpp_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 07:45:26.000000 zpp_menu-1.2.4/zpp_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 15:35:16.240000 zpp_menu-1.3.0/
+-rw-rw-rw-   0        0        0     1106 2023-06-13 07:42:50.000000 zpp_menu-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1467 2023-06-13 15:35:16.236000 zpp_menu-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2022-12-02 09:20:50.000000 zpp_menu-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:35:16.239000 zpp_menu-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 15:35:16.207000 zpp_menu-1.3.0/zpp_menu/
+-rw-rw-rw-   0        0        0       19 2023-06-13 07:43:09.000000 zpp_menu-1.3.0/zpp_menu/__init__.py
+-rw-rw-rw-   0        0        0    14658 2023-06-13 15:32:05.000000 zpp_menu-1.3.0/zpp_menu/menu.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:35:16.232000 zpp_menu-1.3.0/zpp_menu.egg-info/
+-rw-rw-rw-   0        0        0     1467 2023-06-13 15:35:15.000000 zpp_menu-1.3.0/zpp_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-13 15:35:16.000000 zpp_menu-1.3.0/zpp_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:35:15.000000 zpp_menu-1.3.0/zpp_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 15:35:15.000000 zpp_menu-1.3.0/zpp_menu.egg-info/top_level.txt
```

### Comparing `zpp_menu-1.2.4/LICENSE` & `zpp_menu-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpp_menu-1.2.4/PKG-INFO` & `zpp_menu-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpp_menu
-Version: 1.2.4
+Version: 1.3.0
 Summary: Générateur d'un menu à touches fléchées
 Home-page: https://github.com/ZephyrOff/py-zpp_menu
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_menu
 Keywords: menu terminal zephyroff
 Platform: ALL
```

### Comparing `zpp_menu-1.2.4/README.md` & `zpp_menu-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zpp_menu-1.2.4/zpp_menu/menu.py` & `zpp_menu-1.3.0/zpp_menu/menu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+
 import os
+from glob import glob
 
 if os.name=="nt":
     from msvcrt import getch,kbhit
 else:
     import sys,tty,os,termios
 
 ########################### Getch ###########################
@@ -43,20 +45,18 @@
         if os.name=="nt":
             self.terminal_mode()
 
         self.color = {"black": "0","red": "1","green": "2","yellow": "3","blue": "4","magenta": "5","cyan": "6","light_gray": "7","dark_gray": "8","light_red": "9","light_green": "10","light_yellow": "11","light_blue": "12","light_magenta": "13","light_cyan": "14","white": "15","grey_0": "16","navy_blue": "17","dark_blue": "18","blue_3a": "19","blue_3b": "20","blue_1": "21","dark_green": "22","deep_sky_blue_4a": "23","deep_sky_blue_4b": "24","deep_sky_blue_4c": "25","dodger_blue_3": "26","dodger_blue_2": "27","green_4": "28","spring_green_4": "29","turquoise_4": "30","deep_sky_blue_3a": "31","deep_sky_blue_3b": "32","dodger_blue_1": "33","green_3a": "34","spring_green_3a": "35","dark_cyan": "36","light_sea_green": "37","deep_sky_blue_2": "38","deep_sky_blue_1": "39","green_3b": "40","spring_green_3b": "41","spring_green_2a": "42","cyan_3": "43","dark_turquoise": "44","turquoise_2": "45","green_1": "46","spring_green_2b": "47","spring_green_1": "48","medium_spring_green": "49","cyan_2": "50","cyan_1": "51","dark_red_1": "52","deep_pink_4a": "53","purple_4a": "54","purple_4b": "55","purple_3": "56","blue_violet": "57","orange_4a": "58","grey_37": "59","medium_purple_4": "60","slate_blue_3a": "61","slate_blue_3b": "62","royal_blue_1": "63","chartreuse_4": "64","dark_sea_green_4a": "65","pale_turquoise_4": "66","steel_blue": "67","steel_blue_3": "68","cornflower_blue": "69","chartreuse_3a": "70","dark_sea_green_4b": "71","cadet_blue_2": "72","cadet_blue_1": "73","sky_blue_3": "74","steel_blue_1a": "75","chartreuse_3b": "76","pale_green_3a": "77","sea_green_3": "78","aquamarine_3": "79","medium_turquoise": "80","steel_blue_1b": "81","chartreuse_2a": "82","sea_green_2": "83","sea_green_1a": "84","sea_green_1b": "85","aquamarine_1a": "86","dark_slate_gray_2": "87","dark_red_2": "88","deep_pink_4b": "89","dark_magenta_1": "90","dark_magenta_2": "91","dark_violet_1a": "92","purple_1a": "93","orange_4b": "94","light_pink_4": "95","plum_4": "96","medium_purple_3a": "97","medium_purple_3b": "98","slate_blue_1": "99","yellow_4a": "100","wheat_4": "101","grey_53": "102","light_slate_grey": "103","medium_purple": "104","light_slate_blue": "105","yellow_4b": "106","dark_olive_green_3a": "107","dark_green_sea": "108","light_sky_blue_3a": "109","light_sky_blue_3b": "110","sky_blue_2": "111","chartreuse_2b": "112","dark_olive_green_3b": "113","pale_green_3b": "114","dark_sea_green_3a": "115","dark_slate_gray_3": "116","sky_blue_1": "117","chartreuse_1": "118","light_green_2": "119","light_green_3": "120","pale_green_1a": "121","aquamarine_1b": "122","dark_slate_gray_1": "123","red_3a": "124","deep_pink_4c": "125","medium_violet_red": "126","magenta_3a": "127","dark_violet_1b": "128","purple_1b": "129","dark_orange_3a": "130","indian_red_1a": "131","hot_pink_3a": "132","medium_orchid_3": "133","medium_orchid": "134","medium_purple_2a": "135","dark_goldenrod": "136","light_salmon_3a": "137","rosy_brown": "138","grey_63": "139","medium_purple_2b": "140","medium_purple_1": "141","gold_3a": "142","dark_khaki": "143","navajo_white_3": "144","grey_69": "145","light_steel_blue_3": "146","light_steel_blue": "147","yellow_3a": "148","dark_olive_green_3": "149","dark_sea_green_3b": "150","dark_sea_green_2": "151","light_cyan_3": "152","light_sky_blue_1": "153","green_yellow": "154","dark_olive_green_2": "155","pale_green_1b": "156","dark_sea_green_5b": "157","dark_sea_green_5a": "158","pale_turquoise_1": "159","red_3b": "160","deep_pink_3a": "161","deep_pink_3b": "162","magenta_3b": "163","magenta_3c": "164","magenta_2a": "165","dark_orange_3b": "166","indian_red_1b": "167","hot_pink_3b": "168","hot_pink_2": "169","orchid": "170","medium_orchid_1a": "171","orange_3": "172","light_salmon_3b": "173","light_pink_3": "174","pink_3": "175","plum_3": "176","violet": "177","gold_3b": "178","light_goldenrod_3": "179","tan": "180","misty_rose_3": "181","thistle_3": "182","plum_2": "183","yellow_3b": "184","khaki_3": "185","light_goldenrod_2a": "186","light_yellow_3": "187","grey_84": "188","light_steel_blue_1": "189","yellow_2": "190","dark_olive_green_1a": "191","dark_olive_green_1b": "192","dark_sea_green_1": "193","honeydew_2": "194","light_cyan_1": "195","red_1": "196","deep_pink_2": "197","deep_pink_1a": "198","deep_pink_1b": "199","magenta_2b": "200","magenta_1": "201","orange_red_1": "202","indian_red_1c": "203","indian_red_1d": "204","hot_pink_1a": "205","hot_pink_1b": "206","medium_orchid_1b": "207","dark_orange": "208","salmon_1": "209","light_coral": "210","pale_violet_red_1": "211","orchid_2": "212","orchid_1": "213","orange_1": "214","sandy_brown": "215","light_salmon_1": "216","light_pink_1": "217","pink_1": "218","plum_1": "219","gold_1": "220","light_goldenrod_2b": "221","light_goldenrod_2c": "222","navajo_white_1": "223","misty_rose1": "224","thistle_1": "225","yellow_1": "226","light_goldenrod_1": "227","khaki_1": "228","wheat_1": "229","cornsilk_1": "230","grey_100": "231","grey_3": "232","grey_7": "233","grey_11": "234","grey_15": "235","grey_19": "236","grey_23": "237","grey_27": "238","grey_30": "239","grey_35": "240","grey_39": "241","grey_42": "242","grey_46": "243","grey_50": "244","grey_54": "245","grey_58": "246","grey_62": "247","grey_66": "248","grey_70": "249","grey_74": "250","grey_78": "251","grey_82": "252","grey_85": "253","grey_89": "254","grey_93": "255"}
         self.mode = {"bold": "1",1: "1","dim": "2",2: "2","italic": "3",3: "3","underlined": "4",4: "4","blink": "5",5: "5","reverse": "7",7: "7","hidden": "8",8: "8","strikethrough": "9",9: "9","reset": "0",0: "0","res_bold": "21",21: "21","res_dim": "22",22: "22","res_underlined": "24",24: "24","res_blink": "25",25: "25","res_reverse": "27",27: "27","res_hidden": "28",28: "28"}
 
     def terminal_mode(self):
-        from ctypes import windll, c_int, byref
-        stdout_handle = windll.kernel32.GetStdHandle(c_int(-11))
-        mode = c_int(0)
-        windll.kernel32.GetConsoleMode(c_int(stdout_handle), byref(mode))
-        mode = c_int(mode.value | 4)
-        windll.kernel32.SetConsoleMode(c_int(stdout_handle), mode)
+        import ctypes
+
+        kernel32 = ctypes.windll.kernel32
+        kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), 7)
 
     def attribute(self):
         if self.idc=='None' or self.idc==None:
             return ""
         else:
             if self.idc in self.mode:
                 return self.ESC + self.mode[self.idc] + self.END
@@ -96,22 +96,16 @@
 def bg(color):
     return ColorClass(color).background()
 
 ########################### Cursor ##########################
 def com(val):
     print("\033"+val,end="")
 
-def cursorUp(x=1):
-    com("["+str(x)+"A")
-
-def cursorDown(x=1):
-    com("["+str(x)+"B")
-
-def cursorReset():
-    com("[0G")
+def cursorTo(x=0):
+    com("["+str(x)+";0H")
 
 def cursorSave():
     com("7")
 
 def cursorRestore():
     com("8")
 
@@ -120,77 +114,153 @@
 
 def cursorShow():
     com("[?25h")
 
 def EraseLine():
     com("[2K")
 
-############################ MENU ###########################
+def clear():
+    cursorTo(0)
+    print("\033[2J",end="")
+
+def cursorReset():
+    com("[0G")
+
+############################ Menu ###########################
 class MenuClass():
     def __init__(self,Title, Options, Background, Foreground, Pointer, Padding):
         if isinstance(Options,list):
             self.MenuMax = len(Options)-1
             self.Selected = 0
             self.Background = Background
             self.Foreground = Foreground
             self.Title = Title
+            self.title_size = len(Title.split("\n"))
             self.Options = Options
 
+            self.column, line = os.get_terminal_size()
+
             cursorHide()
 
+            self.path = self.Title
+
             self.edgeY = Padding
             self.pointer = Pointer
 
+
     def __del__(self):
         cursorShow()
+        clear()
+
+    def print_index(self, before, element, foreground=None, background=None):
+        max = os.get_terminal_size().columns-len(before)
+        size = len(before) + len(element)
+
+        if size<max:
+            if foreground!=None:
+                print(before + fg(foreground)+bg(background)+element+attr(0))
+            else:
+                print(before + element)
+        else:
+            if foreground!=None:
+                print(before + fg(foreground)+bg(background)+element[0:max-1]+attr(0))
+            else:
+                print(before + element[0:max-1])   
+
 
     def show(self):
+            clear()
+            tmax = (os.get_terminal_size().lines)-self.title_size
             print(self.Title)
+
+            cursorTo(self.title_size+1)
+
             for i,element in enumerate(self.Options):
-                if i==self.Selected:
-                    print(" "*self.edgeY + self.pointer + fg(self.Foreground)+bg(self.Background)+element+attr(0))
-                else:
-                    print(" "*(self.edgeY+len(self.pointer)) + element)
+                if i<tmax-1:
+                    size = len(" "*(self.edgeY+len(self.pointer)) + element)
+                    if i==self.Selected:
+                        self.print_index(" "*(self.edgeY+len(self.pointer)), element, self.Foreground, self.Background)
+                    else:
+                        self.print_index(" "*(self.edgeY+len(self.pointer)), element)
+            
+            if tmax<self.MenuMax:
+                self.size = tmax-2
+            else:
+                self.size = self.MenuMax
 
+            self.Selected = 0
+            self.cursor = 2
             while True:
                 k = getkey()
-                if k=="up":
+                if k=="up" and len(self.Options)>1:
                     self.Rewrite_line()
                     if self.Selected-1<0:
                         self.Selected=self.MenuMax
-                        cursorDown(self.MenuMax)
+                        self.cursor = self.size+2
+                        self.Rewrite_screen("bottom")
                     else:
                         self.Selected-=1
-                        cursorUp(1)
+                        if self.cursor==2 and self.Selected>=0:
+                            self.Rewrite_screen("up")
+                        else:
+                            self.cursor-=1
                     self.Rewrite_Selected()
-                elif k=="down":
+                elif k=="down" and len(self.Options)>1:
                     self.Rewrite_line()
                     if self.Selected+1>self.MenuMax:
                         self.Selected=0
-                        cursorUp(self.MenuMax)
+                        self.cursor=2
+                        self.Rewrite_screen("top")
                     else:
                         self.Selected+=1
-                        cursorDown(1)
+                        if self.cursor==self.size+2 and self.cursor<self.MenuMax and self.Selected<self.MenuMax+1:
+                            self.Rewrite_screen("down")
+                        else:
+                            self.cursor+=1
+                        cursorTo(self.cursor+self.title_size)
                     self.Rewrite_Selected()
                 elif k=="enter":
                     return self.Selected
+    
+    def Rewrite_screen(self,direction):
+        clear()
+        print(self.Title)
+        cursorTo(self.title_size+1)
+
+        if direction=="down":
+            list_f = self.Options[self.Selected-self.size:self.Selected+1]
+        elif direction=="up":
+            list_f = self.Options[self.Selected:self.Selected+self.size+1]
+        elif direction=="top":
+            list_f = self.Options[0:self.size+1]
+        elif direction=="bottom":
+            list_f = self.Options[self.Selected-self.size:self.Selected]
+
+        for i in list_f:
+            size = len(" "*(self.edgeY+len(self.pointer))+i)
+            if i==self.Options[self.Selected]:
+                self.print_index(" "*(self.edgeY+len(self.pointer)), i, self.Foreground, self.Background)
+            else:
+                self.print_index(" "*(self.edgeY+len(self.pointer)), i)
 
     def Rewrite_line(self):
         cursorSave()
+        cursorTo(self.title_size+self.cursor-1)
         EraseLine()
-        cursorUp((self.MenuMax-self.Selected)+1)
-        print(" "*(self.edgeY+len(self.pointer)) + self.Options[self.Selected],end="")
+        size = len(" "*(self.edgeY+len(self.pointer)) + self.Options[self.Selected])
+        self.print_index(" "*(self.edgeY+len(self.pointer)), self.Options[self.Selected])
 
     def Rewrite_Selected(self):
+        cursorTo(self.title_size+self.cursor-1)
         EraseLine()
-        cursorReset()
-        print(" "*self.edgeY + self.pointer + fg(self.Foreground)+bg(self.Background)+self.Options[self.Selected]+attr(0))
+        size = len(" "*self.edgeY + self.pointer + self.Options[self.Selected])
+        self.print_index(" "*self.edgeY + self.pointer, self.Options[self.Selected], self.Foreground, self.Background)
         cursorRestore()
 
 def Menu(Title, Options, Background="", Foreground="yellow", Pointer="", Padding=2, Selected=None):
     if Selected==None:
         return MenuClass(Title, Options, Background, Foreground, Pointer, Padding).show()
     else:
         mc = MenuClass(Title, Options, Background, Foreground, Pointer, Padding)
         if isinstance(Selected, int) and Selected<len(Options):
             mc.Selected = Selected
-        return mc.show()
+        return mc.show()
```

### Comparing `zpp_menu-1.2.4/zpp_menu.egg-info/PKG-INFO` & `zpp_menu-1.3.0/zpp_menu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpp-menu
-Version: 1.2.4
+Version: 1.3.0
 Summary: Générateur d'un menu à touches fléchées
 Home-page: https://github.com/ZephyrOff/py-zpp_menu
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_menu
 Keywords: menu terminal zephyroff
 Platform: ALL
```

