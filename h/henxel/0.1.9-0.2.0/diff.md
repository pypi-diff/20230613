# Comparing `tmp/henxel-0.1.9.tar.gz` & `tmp/henxel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.1.9.tar", last modified: Sun Jun  4 11:13:06 2023, max compression
+gzip compressed data, was "henxel-0.2.0.tar", last modified: Tue Jun 13 18:16:03 2023, max compression
```

## Comparing `henxel-0.1.9.tar` & `henxel-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.959526 henxel-0.1.9/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.1.9/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-05-18 15:46:16.000000 henxel-0.1.9/MANIFEST.in
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-04 11:13:06.959526 henxel-0.1.9/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4429 2023-06-04 10:58:22.000000 henxel-0.1.9/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-06-04 10:54:28.000000 henxel-0.1.9/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-06-04 11:13:06.959526 henxel-0.1.9/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/henxel/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    98446 2023-06-04 10:53:55.000000 henxel-0.1.9/src/henxel/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-05-24 09:37:41.000000 henxel-0.1.9/src/henxel/changefont.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.1.9/src/henxel/editor.png
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7223 2023-06-04 10:51:13.000000 henxel-0.1.9/src/henxel/fdialog.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7837 2023-06-04 10:51:13.000000 henxel-0.1.9/src/henxel/help.txt
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-04 11:13:06.955526 henxel-0.1.9/src/henxel.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      302 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-06-04 11:13:06.000000 henxel-0.1.9/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-13 18:16:03.697047 henxel-0.2.0/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.2.0/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-06-13 18:05:14.000000 henxel-0.2.0/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-13 18:16:03.697047 henxel-0.2.0/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4429 2023-06-13 18:05:01.000000 henxel-0.2.0/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-06-13 18:04:24.000000 henxel-0.2.0/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-06-13 18:16:03.701047 henxel-0.2.0/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-13 18:16:03.689047 henxel-0.2.0/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-13 18:16:03.697047 henxel-0.2.0/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    97889 2023-06-13 18:01:41.000000 henxel-0.2.0/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-05-24 09:37:41.000000 henxel-0.2.0/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.2.0/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7223 2023-06-13 16:52:27.000000 henxel-0.2.0/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8402 2023-06-13 18:04:04.000000 henxel-0.2.0/src/henxel/help.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2137 2023-06-13 18:01:41.000000 henxel-0.2.0/src/henxel/wordexpand.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-06-13 18:16:03.697047 henxel-0.2.0/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-06-13 18:16:03.000000 henxel-0.2.0/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      327 2023-06-13 18:16:03.000000 henxel-0.2.0/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-06-13 18:16:03.000000 henxel-0.2.0/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-06-13 18:16:03.000000 henxel-0.2.0/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.1.9/LICENSE` & `henxel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `henxel-0.1.9/PKG-INFO` & `henxel-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.9
+Version: 0.2.0
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `henxel-0.1.9/README.md` & `henxel-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `henxel-0.1.9/setup.cfg` & `henxel-0.2.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = henxel
-version = 0.1.9
+version = 0.2.0
 author = SamuelKos
 author_email = koskinens371@gmail.com
 description = GUI-editor for Python development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SamuelKos/henxel
 project_urls =
```

### Comparing `henxel-0.1.9/src/henxel/__init__.py` & `henxel-0.2.0/src/henxel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 import sys
 
 # used in syntax highlight
 import tokenize
 import io
 
 # from current directory
+from . import wordexpand
 from . import changefont
 from . import fdialog
 
 # for executing edited file in the same env than this editor, which is nice:
 # It means you have your installed dependencies available. By self.run()
 import subprocess
 
@@ -170,15 +171,14 @@
 		# get current git-branch
 		try:
 			self.branch = subprocess.run('git branch --show-current'.split(),
 					check=True, capture_output=True).stdout.decode().strip()
 		except Exception as e:
 			pass
 		
-		self.replace_overlap_index = None
 		self.search_idx = ('1.0', '1.0')
 		self.search_matches = 0
 		self.old_word = ''
 		self.new_word = ''
 		
 		self.errlines = list()
 		
@@ -294,15 +294,17 @@
 		
 		self.contents = tkinter.Text(self, blockcursor=True, undo=True, maxundo=-1, autoseparators=True,
 					tabstyle='wordprocessor', highlightthickness=0, bd=4, pady=4, padx=10)
 		
 		self.scrollbar = tkinter.Scrollbar(self, orient=tkinter.VERTICAL, highlightthickness=0,
 					bd=0, command = self.contents.yview)
 
-
+		self.expander = wordexpand.ExpandWord(self.contents)
+		self.contents.bind( "<Alt-e>", self.expander.expand_word_event)
+		
 		# Widgets are initiated, now more configuration
 		################################################
 		# Needed in update_linenums(), there is more info.
 		self.update_idletasks()
 		# if self.y_extra_offset > 0, it needs attention
 		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
 		# Needed in update_linenums() and sbset_override()
@@ -320,14 +322,17 @@
 		self.contents.bind( "<Control-i>", self.move_right)
 		
 		self.contents.bind( "<Alt-f>", self.font_choose)
 		self.contents.bind( "<Alt-x>", self.toggle_syntax)
 		self.contents.bind( "<Return>", self.return_override)
 		
 		self.contents.bind( "<Control-d>", self.del_tab)
+		self.contents.bind( "<Control-q>", lambda event: self.del_tab(event, **{'save':False}) )
+		
+		
 		self.contents.bind( "<Shift-Return>", self.comment)
 		self.contents.bind( "<Shift-BackSpace>", self.uncomment)
 		self.contents.bind( "<Tab>", self.tab_override)
 		self.contents.bind( "<ISO_Left_Tab>", self.unindent)
 		self.contents.bind( "<Control-a>", self.select_all)
 		self.contents.bind( "<Control-z>", self.undo_override)
 		self.contents.bind( "<Control-Z>", self.redo_override)
@@ -516,14 +521,15 @@
 		
 		self.contents.tag_config('bools', foreground=magenta)
 		self.contents.tag_config('strings', foreground=green)
 		self.contents.tag_config('selfs', foreground=gray)
 		self.contents.tag_config('mismatch', background='brown1', foreground='white')
 		
 		# search tags have highest priority
+		self.contents.tag_config('replaced', background='yellow', foreground='black')
 		self.contents.tag_config('match', background='lightyellow', foreground='black')
 		self.contents.tag_config('focus', background='lightgreen', foreground='black')
 		self.contents.tag_raise('match')
 		self.contents.tag_raise('focus')
 		
 		
 		self.oldline = ''
@@ -680,15 +686,14 @@
 					linestart = '%s linestart' % line_idx
 					
 					tmp = self.contents.get( linestart, lineend )
 					
 					if self.oldline != tmp or self.oldlinenum != linenum:
 					
 						#print('sync')
-						#print('sync')
 						self.oldline = tmp
 						self.oldlinenum = linenum
 						self.update_tokens(start=linestart, end=lineend, line=tmp)
 				
 
 ############## Linenumbers Begin
 
@@ -833,21 +838,21 @@
 		self.contents.edit_reset()
 		self.contents.edit_modified(0)
 		
 		self.update_title()
 		return 'break'
 		
 		
-	def del_tab(self, event=None):
+	def del_tab(self, event=None, save=True):
 
 		if ((len(self.tabs) == 1) and self.tabs[self.tabindex].type == 'newtab') or (self.state != 'normal'):
 			self.bell()
 			return 'break'
 
-		if self.tabs[self.tabindex].type == 'normal':
+		if self.tabs[self.tabindex].type == 'normal' and save:
 			self.save(activetab=True)
 			
 		self.tabs.pop(self.tabindex)
 			
 		if (len(self.tabs) == 0):
 			newtab = Tab()
 			self.tabs.append(newtab)
@@ -3461,14 +3466,15 @@
 	def stop_search(self, event=None):
 		self.contents.config(state='normal')
 		self.entry.config(state='normal')
 		self.btn_open.config(state='normal')
 		self.btn_save.config(state='normal')
 		self.bind("<Button-3>", lambda event: self.raise_popup(event))
 		self.contents.tag_remove('focus', '1.0', tkinter.END)
+		self.contents.tag_remove('replaced', '1.0', tkinter.END)
 			
 		# Leave tags on, if replace_all, Esc clears.
 		if self.state == 'replace_all':
 		
 			self.bind("<Escape>", self.clear_search_tags)
 			
 		else:
@@ -3480,15 +3486,14 @@
 		self.entry.delete(0, tkinter.END)
 	
 		if self.tabs[self.tabindex].filepath:
 			self.entry.insert(0, self.tabs[self.tabindex].filepath)
 	
 		self.new_word = ''
 		self.search_matches = 0
-		self.replace_overlap_index = None
 		self.update_title()
 		
 		if self.state in [ 'replace_all', 'replace' ]:
 		
 				self.state = 'normal'
 				
 				
@@ -3571,14 +3576,16 @@
 		self.state = state
 		self.btn_open.config(state='disabled')
 		self.btn_save.config(state='disabled')
 		self.entry.bind("<Return>", self.start_search)
 		self.bind("<Escape>", self.stop_search)
 		self.bid1 = self.contents.bind("<Control-n>", func=self.skip_bindlevel )
 		self.bid2 = self.contents.bind("<Control-p>", func=self.skip_bindlevel )
+		self.bid3 = self.contents.bind("<ButtonRelease-1>", func=self.update_curpos, add=True )
+		
 		self.title('Replace this:')
 		self.entry.delete(0, tkinter.END)
 		
 		# autofill from clipboard
 		try:
 			tmp = self.clipboard_get()
 			if 80 > len(tmp) > 0:
@@ -3607,51 +3614,39 @@
 		self.contents.config(state='normal')
 		self.search_matches = 0
 		wordlen = len(self.old_word)
 		wordlen2 = len(self.new_word)
 		pos = '1.0'
 		self.contents.tag_remove('match', '1.0', tkinter.END)
 		
-		# Next while-loop tags matches again, this is the main reason why
-		# there is a problem if new_word contains old_word:it will be rematched.
-		# This is why when there is a match, we move
-		# replace_overlap_index characters back and check if there already is
-		# new_word. If so, it means there have already happened a replacement
-		# and therefore search pos must be recalculated over new_word.
-		
 		while True:
 			pos = self.contents.search(self.old_word, pos, tkinter.END)
 			if not pos: break
 			
-			if self.replace_overlap_index != None:
-				# find the startpos (pos2) and lastpos of new_word:
-				tmp = int(pos.split('.')[1]) - self.replace_overlap_index
-				pos2 = pos.split('.')[0] +'.'+ str(tmp)
-				lastpos = "%s + %dc" % (pos2, wordlen2)
-				
-				if self.contents.get(pos2, lastpos) == self.new_word:
-					# skip this match
-					pos = "%s + %dc" % (pos2, wordlen2+1)
-				else:
-					lastpos = "%s + %dc" % (pos, wordlen)
-					self.contents.tag_add('match', pos, lastpos)
-					pos = "%s + %dc" % (pos, wordlen+1)
-					self.search_matches += 1
-			
-			# this is the normal case:
+			if 'replaced' in self.contents.tag_names(pos):
+				# replaced already, skip
+				pos = "%s + %dc" % ( self.contents.tag_prevrange('replaced', pos)[1], wordlen2+1 )
+				
 			else:
 				lastpos = "%s + %dc" % (pos, wordlen)
 				self.contents.tag_add('match', pos, lastpos)
 				pos = "%s + %dc" % (pos, wordlen+1)
 				self.search_matches += 1
-
+			
+			
 		self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
 		self.contents.tag_remove('match', self.search_idx[0], self.search_idx[1])
 		self.contents.delete(self.search_idx[0], self.search_idx[1])
 		self.contents.insert(self.search_idx[0], self.new_word)
+		
+		# tag replacement to avoid rematching same place
+		p = "%s + %dc" % (self.search_idx[0], wordlen2)
+		self.contents.tag_add('replaced', self.search_idx[0], p)
+		
+		
 		self.contents.config(state='disabled')
 		
 		self.search_matches -= 1
 		
 		if self.search_matches == 0:
 			self.stop_search()
 
@@ -3687,28 +3682,21 @@
 	def start_replace(self, event=None):
 		self.new_word = self.entry.get()
 		
 		if self.old_word == self.new_word:
 			return
 		else:
 		
-			self.replace_overlap_index = None
 			self.bind("<Control-n>", self.show_next)
 			self.bind("<Control-p>", self.show_prev)
 			
 			# prevent focus messing
 			self.entry.bind("<Return>", self.do_nothing)
 			self.entry.config(state='disabled')
 			self.focus_set()
-			
-			# Check if new_word contains old_word, if so:
-			# record its overlap-index, which we need in do_single_replace()
-			# (explanation for why this is needed is given there)
-			if self.old_word in self.new_word:
-				self.replace_overlap_index = self.new_word.index(self.old_word)
 				
 			if self.state == 'replace':
 				self.bind( "<Return>", self.do_single_replace)
 				self.title('Replacing %s matches of %s with: %s' % (str(self.search_matches), self.old_word, self.new_word) )
 			elif self.state == 'replace_all':
 				self.bind( "<Return>", self.do_replace_all)
 				self.title('Replacing ALL %s matches of %s with: %s' % (str(self.search_matches), self.old_word, self.new_word) )
```

### Comparing `henxel-0.1.9/src/henxel/changefont.py` & `henxel-0.2.0/src/henxel/changefont.py`

 * *Files identical despite different names*

### Comparing `henxel-0.1.9/src/henxel/fdialog.py` & `henxel-0.2.0/src/henxel/fdialog.py`

 * *Files identical despite different names*

### Comparing `henxel-0.1.9/src/henxel/help.txt` & `henxel-0.2.0/src/henxel/help.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 		Ctrl-Z  Redo
 		
 		Alt-f   Font setting
 		Alt-s   Color setting
 		Alt-t   Toggle color setting
 		Alt-l   Toggle linenumbers
 		Alt-x   Toggle syntax highlight
-		
+		Alt-e   expand word
 		Alt-n   Open new tab			Try this: Alt-n-Return
-		Ctrl-d  Close current tab
+		
+		Ctrl-d  Close current tab and save it
+		Ctrl-q  Close current tab without saving it
 		Alt-w   Walk tabs forward
 		Alt-q   Walk tabs backwards
 		
 		Ctrl-o  Insert linebreak at cursor
 		Ctrl-i  Move cursor right
 		Ctrl-b  Move cursor left
 		Ctrl-n  Move cursor down
@@ -151,15 +153,31 @@
 		This ensures indentation of whole block. If you do not do this,
 		and select for example from 'def' - word, which has indentation,
 		then indentation of this first line is wrong when pasted, compared
 		to other lines. But editor moves cursor at the start of block so
 		you can start fixing indenting that function definition line or
 		similar.
 	
+	
+	How to: expand word
+	  - When starting to write object-name that has been used earlier near
+		current position, like if previous line was:
+		
+			var = self.functionabc()
 		
+		then when continuing at the next line:
+			
+			var2 = self.func
+			
+		and pressing Alt-e it should expand to functionabc. Pressing again
+		searches backwards next word with func in its name, and when no
+		matches are found, it starts to search onwards to the file-end and
+		after that another round starts.
+	
+	
 	How to: hide blinking cursor
 	  - Sometimes one wants to focus on the code and blinking cursor is
 		not helping with that. Since there is no timer to turn it off one
 		have to click on linenumber-widget to hide the cursor.
 	
 	
 	How to: change indent-depth
```

### Comparing `henxel-0.1.9/src/henxel.egg-info/PKG-INFO` & `henxel-0.2.0/src/henxel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.1.9
+Version: 0.2.0
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

